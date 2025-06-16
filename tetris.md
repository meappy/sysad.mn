---
layout: default
title: Terminal Tetris - Gerald Sim
---

<div class="ear-mark-link">
  <a href="/" class="ear-mark">Home</a>
</div>

<div class="hero-section tetris-hero">
  <div class="hero-content">
    <div class="hero-text">
      <h1 class="hero-tagline">Terminal Tetris</h1>
      <p class="hero-quote">Because even sysadmins need a break from fixing production</p>
    </div>
  </div>
</div>

<section class="tetris-section">
  <div class="section-container">
    <div class="tetris-container">
      <div class="tetris-game">
        <canvas id="tetris-canvas" width="320" height="640"></canvas>
        <div class="game-info">
          <div class="score-board">
            <div class="score-item">
              <span class="label">Score:</span>
              <span id="score">0</span>
            </div>
            <div class="score-item">
              <span class="label">Lines:</span>
              <span id="lines">0</span>
            </div>
            <div class="score-item">
              <span class="label">Level:</span>
              <span id="level">1</span>
            </div>
          </div>
          <div class="game-controls">
            <button id="start-btn" class="game-btn">Start</button>
            <button id="pause-btn" class="game-btn">Pause</button>
            <button id="reset-btn" class="game-btn">Reset</button>
          </div>
          <div class="instructions">
            <h4>Controls:</h4>
            <p>← → Move</p>
            <p>↓ Soft Drop</p>
            <p>↑ Rotate</p>
            <p>Space Hard Drop</p>
          </div>
          <div class="mobile-controls-left">
            <button id="rotate-btn" class="mobile-btn">↻</button>
            <button id="drop-btn" class="mobile-btn">⬇</button>
          </div>
          <div class="mobile-controls-right">
            <button id="left-btn" class="mobile-btn">←</button>
            <button id="right-btn" class="mobile-btn">→</button>
            <button id="down-btn" class="mobile-btn">↓</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
/* Global base styles matching main page */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  overflow-x: hidden;
  width: 100%;
}

body {
  background: linear-gradient(135deg, #0f0f23 0%, #1a1a2e 50%, #16213e 100%);
  color: #e0e0e0;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  line-height: 1.6;
  overflow-x: hidden;
  position: relative;
  width: 100%;
}

body::before {
  content: '';
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: 
    radial-gradient(circle at 20% 30%, rgba(59, 130, 246, 0.08) 0%, transparent 50%),
    radial-gradient(circle at 80% 60%, rgba(139, 92, 246, 0.06) 0%, transparent 50%),
    radial-gradient(circle at 40% 80%, rgba(100, 255, 218, 0.04) 0%, transparent 50%),
    radial-gradient(circle at 90% 20%, rgba(59, 130, 246, 0.05) 0%, transparent 50%),
    radial-gradient(circle at 10% 90%, rgba(139, 92, 246, 0.05) 0%, transparent 50%);
  animation: lavaLamp 20s ease-in-out infinite;
  pointer-events: none;
  z-index: -1;
}


@keyframes lavaLamp {
  0%, 100% {
    background: 
      radial-gradient(circle at 20% 30%, rgba(59, 130, 246, 0.08) 0%, transparent 50%),
      radial-gradient(circle at 80% 60%, rgba(139, 92, 246, 0.06) 0%, transparent 50%),
      radial-gradient(circle at 40% 80%, rgba(100, 255, 218, 0.04) 0%, transparent 50%),
      radial-gradient(circle at 90% 20%, rgba(59, 130, 246, 0.05) 0%, transparent 50%),
      radial-gradient(circle at 10% 90%, rgba(139, 92, 246, 0.05) 0%, transparent 50%);
  }
  25% {
    background: 
      radial-gradient(circle at 30% 50%, rgba(59, 130, 246, 0.10) 0%, transparent 55%),
      radial-gradient(circle at 70% 40%, rgba(139, 92, 246, 0.08) 0%, transparent 55%),
      radial-gradient(circle at 60% 70%, rgba(100, 255, 218, 0.05) 0%, transparent 55%),
      radial-gradient(circle at 85% 30%, rgba(59, 130, 246, 0.06) 0%, transparent 55%),
      radial-gradient(circle at 15% 80%, rgba(139, 92, 246, 0.04) 0%, transparent 55%);
  }
  50% {
    background: 
      radial-gradient(circle at 60% 70%, rgba(59, 130, 246, 0.06) 0%, transparent 50%),
      radial-gradient(circle at 30% 20%, rgba(139, 92, 246, 0.10) 0%, transparent 50%),
      radial-gradient(circle at 80% 50%, rgba(100, 255, 218, 0.06) 0%, transparent 50%),
      radial-gradient(circle at 70% 80%, rgba(59, 130, 246, 0.04) 0%, transparent 50%),
      radial-gradient(circle at 20% 60%, rgba(139, 92, 246, 0.08) 0%, transparent 50%);
  }
  75% {
    background: 
      radial-gradient(circle at 80% 40%, rgba(59, 130, 246, 0.09) 0%, transparent 52%),
      radial-gradient(circle at 20% 80%, rgba(139, 92, 246, 0.05) 0%, transparent 52%),
      radial-gradient(circle at 50% 30%, rgba(100, 255, 218, 0.07) 0%, transparent 52%),
      radial-gradient(circle at 10% 40%, rgba(59, 130, 246, 0.06) 0%, transparent 52%),
      radial-gradient(circle at 90% 70%, rgba(139, 92, 246, 0.06) 0%, transparent 52%);
  }
}

/* Ear mark style */
.ear-mark-link {
  position: fixed;
  top: 0;
  right: 0;
  z-index: 1001;
}

.ear-mark {
  display: block;
  background: linear-gradient(135deg, #3b82f6, #8b5cf6);
  color: white;
  text-decoration: none;
  padding: 0.8rem 2rem 0.8rem 1rem;
  font-family: 'SF Mono', 'Monaco', 'Cascadia Code', 'Roboto Mono', Consolas, 'Courier New', monospace;
  font-weight: 600;
  font-size: 0.9rem;
  letter-spacing: 1px;
  text-transform: uppercase;
  position: relative;
  clip-path: polygon(0 0, calc(100% - 20px) 0, 100% 100%, 0 100%);
  transition: all 0.3s ease;
  box-shadow: 0 4px 12px rgba(59, 130, 246, 0.3);
}

.ear-mark:hover {
  background: linear-gradient(135deg, #2563eb, #7c3aed);
  transform: translateY(2px);
  box-shadow: 0 6px 20px rgba(59, 130, 246, 0.4);
}

/* Tetris page specific styles */
.tetris-hero {
  min-height: 40vh;
  padding: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: relative;
}

.tetris-hero .hero-content {
  max-width: 800px;
  text-align: center;
  z-index: 2;
  position: relative;
}

.tetris-hero .hero-tagline {
  font-size: clamp(2.5rem, 6vw, 3.5rem);
  text-align: center;
  margin-bottom: 3rem;
  color: #ffffff;
  font-weight: 700;
  animation: fadeInUp 1s ease-out 0.2s both;
}

.tetris-hero .hero-quote {
  font-size: clamp(1rem, 2.5vw, 1.2rem);
  margin-bottom: 0;
  color: #94a3b8;
  animation: fadeInUp 1s ease-out 0.4s both;
  font-weight: 400;
  line-height: 1.5;
  max-width: 600px;
  font-style: italic;
  opacity: 0.9;
  text-align: center;
  font-family: 'Playfair Display', 'Georgia', 'Times New Roman', serif;
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}


/* Tetris Section */
.tetris-section {
  min-height: 60vh;
}

.tetris-container {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  gap: 2rem;
  margin-top: 2rem;
}

.tetris-game {
  display: flex;
  gap: 2rem;
  align-items: flex-start;
}

#tetris-canvas {
  border: 2px solid #64ffda;
  border-radius: 8px;
  background: #000;
  box-shadow: 0 0 20px rgba(100, 255, 218, 0.3);
}

.game-info {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  min-width: 200px;
}

.score-board {
  background: rgba(26, 26, 26, 0.8);
  border: 1px solid rgba(100, 255, 218, 0.2);
  border-radius: 12px;
  padding: 1.5rem;
}

.score-item {
  display: flex;
  justify-content: space-between;
  margin-bottom: 0.5rem;
  font-family: 'SF Mono', 'Monaco', 'Cascadia Code', 'Roboto Mono', Consolas, 'Courier New', monospace;
}

.score-item .label {
  color: #94a3b8;
}

.score-item span:last-child {
  color: #64ffda;
  font-weight: bold;
}

.game-controls {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.game-btn {
  padding: 0.8rem 1.2rem;
  border: 2px solid #64ffda;
  background: transparent;
  color: #64ffda;
  border-radius: 8px;
  font-family: 'SF Mono', 'Monaco', 'Cascadia Code', 'Roboto Mono', Consolas, 'Courier New', monospace;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
}

.game-btn:hover {
  background: rgba(100, 255, 218, 0.1);
  transform: translateY(-2px);
}

.game-btn:active {
  transform: translateY(0);
}

.instructions {
  background: rgba(26, 26, 26, 0.8);
  border: 1px solid rgba(100, 255, 218, 0.2);
  border-radius: 12px;
  padding: 1.5rem;
}

.instructions h4 {
  color: #ffffff;
  margin-bottom: 1rem;
  font-size: 1.1rem;
}

.instructions p {
  color: #94a3b8;
  margin-bottom: 0.3rem;
  font-family: 'SF Mono', 'Monaco', 'Cascadia Code', 'Roboto Mono', Consolas, 'Courier New', monospace;
  font-size: 0.9rem;
}

.mobile-controls-left {
  display: none;
  position: fixed;
  left: 20px;
  top: 50%;
  transform: translateY(-50%);
  flex-direction: column;
  gap: 0.5rem;
  background: rgba(26, 26, 26, 0.95);
  border: 1px solid rgba(100, 255, 218, 0.3);
  border-radius: 12px;
  padding: 0.6rem;
  z-index: 1000;
  backdrop-filter: blur(10px);
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
}

.mobile-controls-right {
  display: none;
  position: fixed;
  right: 20px;
  top: 50%;
  transform: translateY(-50%);
  flex-direction: column;
  gap: 0.5rem;
  background: rgba(26, 26, 26, 0.95);
  border: 1px solid rgba(100, 255, 218, 0.3);
  border-radius: 12px;
  padding: 0.6rem;
  z-index: 1000;
  backdrop-filter: blur(10px);
  box-shadow: 0 4px 20px rgba(0, 0, 0, 0.3);
}

.mobile-controls-row {
  display: flex;
  justify-content: center;
  gap: 0.5rem;
}

.mobile-btn {
  width: 40px;
  height: 40px;
  border: 2px solid #64ffda;
  background: rgba(26, 26, 26, 0.8);
  color: #64ffda;
  border-radius: 8px;
  font-size: 1.1rem;
  font-weight: bold;
  cursor: pointer;
  transition: all 0.3s ease;
  user-select: none;
  -webkit-user-select: none;
  -webkit-tap-highlight-color: transparent;
  backdrop-filter: blur(5px);
}

.mobile-btn:hover,
.mobile-btn:active {
  background: rgba(100, 255, 218, 0.2);
  transform: scale(0.95);
}

.mobile-btn:focus {
  outline: none;
}

/* Responsive Design */
@media (max-width: 768px) {
  .tetris-container {
    flex-direction: column;
    align-items: center;
    overflow-x: hidden;
  }
  
  .tetris-game {
    flex-direction: column;
    align-items: center;
  }
  
  #tetris-canvas {
    width: 280px;
    height: 560px;
  }
  
  .game-info {
    width: 100%;
    max-width: 300px;
  }
  
  /* Show mobile controls on mobile */
  .mobile-controls-left {
    display: flex;
  }
  
  .mobile-controls-right {
    display: flex;
  }
  
  .instructions {
    display: none;
  }
  
}

@media (max-width: 480px) {
  .tetris-hero {
    padding: 1rem;
    overflow-x: hidden;
  }
  
  .section-container {
    padding: 2rem 1rem;
    overflow-x: hidden;
  }
  
  /* Force all elements to stay within viewport */
  html, body {
    overflow-x: hidden !important;
    width: 100% !important;
    max-width: 100% !important;
  }
  
  section {
    overflow-x: hidden !important;
    width: 100% !important;
    max-width: 100% !important;
  }
  
  * {
    max-width: 100% !important;
    box-sizing: border-box !important;
  }
  
  
  #tetris-canvas {
    width: 260px;
    height: 520px;
    margin: 0 auto;
  }
  
  .tetris-container {
    padding: 0 1rem;
    max-width: 100%;
  }
}

/* Footer Fix */
.site-footer {
  width: 100%;
  overflow-x: hidden;
}

.site-footer .container {
  width: 100%;
  max-width: 100%;
  padding: 0 1rem;
  box-sizing: border-box;
}
</style>

<script>
// Set initial tagline
document.addEventListener('DOMContentLoaded', function() {
  initTetris();
});

// Tetris Game Implementation
function initTetris() {
  const canvas = document.getElementById('tetris-canvas');
  if (!canvas) return;
  
  const ctx = canvas.getContext('2d');
  const gridWidth = 10;
  const gridHeight = 20;
  const cellSize = 32;
  
  let gameState = {
    grid: Array(gridHeight).fill().map(() => Array(gridWidth).fill(0)),
    currentPiece: null,
    currentX: 0,
    currentY: 0,
    score: 0,
    lines: 0,
    level: 1,
    gameRunning: false,
    gamePaused: false,
    dropTime: 0,
    dropInterval: 1000
  };
  
  // Tetris pieces (tetrominoes)
  const pieces = [
    // I-piece
    [
      [1, 1, 1, 1]
    ],
    // O-piece
    [
      [1, 1],
      [1, 1]
    ],
    // T-piece
    [
      [0, 1, 0],
      [1, 1, 1]
    ],
    // S-piece
    [
      [0, 1, 1],
      [1, 1, 0]
    ],
    // Z-piece
    [
      [1, 1, 0],
      [0, 1, 1]
    ],
    // J-piece
    [
      [1, 0, 0],
      [1, 1, 1]
    ],
    // L-piece
    [
      [0, 0, 1],
      [1, 1, 1]
    ]
  ];
  
  const colors = [
    '#64ffda', // cyan
    '#3b82f6', // blue
    '#8b5cf6', // purple
    '#f59e0b', // amber
    '#ef4444', // red
    '#10b981', // emerald
    '#f97316'  // orange
  ];
  
  function rotatePiece(piece) {
    const rows = piece.length;
    const cols = piece[0].length;
    const rotated = Array(cols).fill().map(() => Array(rows).fill(0));
    
    for (let row = 0; row < rows; row++) {
      for (let col = 0; col < cols; col++) {
        rotated[col][rows - 1 - row] = piece[row][col];
      }
    }
    
    return rotated;
  }
  
  function isValidMove(piece, x, y) {
    for (let py = 0; py < piece.length; py++) {
      for (let px = 0; px < piece[py].length; px++) {
        if (piece[py][px]) {
          const newX = x + px;
          const newY = y + py;
          
          if (newX < 0 || newX >= gridWidth || newY >= gridHeight) {
            return false;
          }
          
          if (newY >= 0 && gameState.grid[newY][newX]) {
            return false;
          }
        }
      }
    }
    return true;
  }
  
  function placePiece() {
    for (let py = 0; py < gameState.currentPiece.length; py++) {
      for (let px = 0; px < gameState.currentPiece[py].length; px++) {
        if (gameState.currentPiece[py][px]) {
          const x = gameState.currentX + px;
          const y = gameState.currentY + py;
          if (y >= 0) {
            gameState.grid[y][x] = gameState.currentPiece.colorIndex;
          }
        }
      }
    }
  }
  
  function clearLines() {
    let linesCleared = 0;
    for (let y = gridHeight - 1; y >= 0; y--) {
      if (gameState.grid[y].every(cell => cell !== 0)) {
        gameState.grid.splice(y, 1);
        gameState.grid.unshift(Array(gridWidth).fill(0));
        linesCleared++;
        y++; // Check the same line again
      }
    }
    
    if (linesCleared > 0) {
      gameState.lines += linesCleared;
      gameState.score += linesCleared * 100 * gameState.level;
      gameState.level = Math.floor(gameState.lines / 10) + 1;
      gameState.dropInterval = Math.max(100, 1000 - (gameState.level - 1) * 100);
      updateDisplay();
    }
  }
  
  function spawnPiece() {
    const pieceIndex = Math.floor(Math.random() * pieces.length);
    gameState.currentPiece = pieces[pieceIndex].map(row => [...row]);
    gameState.currentPiece.colorIndex = pieceIndex + 1;
    gameState.currentX = Math.floor(gridWidth / 2) - Math.floor(gameState.currentPiece[0].length / 2);
    gameState.currentY = 0;
    
    if (!isValidMove(gameState.currentPiece, gameState.currentX, gameState.currentY)) {
      gameOver();
    }
  }
  
  function gameOver() {
    gameState.gameRunning = false;
    document.getElementById('start-btn').textContent = 'Start';
    alert(`Game Over! Final Score: ${gameState.score}`);
  }
  
  function updateDisplay() {
    document.getElementById('score').textContent = gameState.score;
    document.getElementById('lines').textContent = gameState.lines;
    document.getElementById('level').textContent = gameState.level;
  }
  
  function draw() {
    // Clear canvas
    ctx.fillStyle = '#000';
    ctx.fillRect(0, 0, canvas.width, canvas.height);
    
    // Draw grid
    for (let y = 0; y < gridHeight; y++) {
      for (let x = 0; x < gridWidth; x++) {
        if (gameState.grid[y][x]) {
          ctx.fillStyle = colors[gameState.grid[y][x] - 1];
          ctx.fillRect(x * cellSize, y * cellSize, cellSize - 1, cellSize - 1);
        }
      }
    }
    
    // Draw current piece
    if (gameState.currentPiece) {
      ctx.fillStyle = colors[gameState.currentPiece.colorIndex - 1];
      for (let py = 0; py < gameState.currentPiece.length; py++) {
        for (let px = 0; px < gameState.currentPiece[py].length; px++) {
          if (gameState.currentPiece[py][px]) {
            const x = (gameState.currentX + px) * cellSize;
            const y = (gameState.currentY + py) * cellSize;
            ctx.fillRect(x, y, cellSize - 1, cellSize - 1);
          }
        }
      }
    }
  }
  
  function gameLoop(currentTime) {
    if (!gameState.gameRunning || gameState.gamePaused) {
      requestAnimationFrame(gameLoop);
      return;
    }
    
    if (currentTime - gameState.dropTime > gameState.dropInterval) {
      if (isValidMove(gameState.currentPiece, gameState.currentX, gameState.currentY + 1)) {
        gameState.currentY++;
      } else {
        placePiece();
        clearLines();
        spawnPiece();
      }
      gameState.dropTime = currentTime;
    }
    
    draw();
    requestAnimationFrame(gameLoop);
  }
  
  function startGame() {
    gameState.grid = Array(gridHeight).fill().map(() => Array(gridWidth).fill(0));
    gameState.score = 0;
    gameState.lines = 0;
    gameState.level = 1;
    gameState.gameRunning = true;
    gameState.gamePaused = false;
    gameState.dropInterval = 1000;
    updateDisplay();
    spawnPiece();
    document.getElementById('start-btn').textContent = 'Stop';
    requestAnimationFrame(gameLoop);
  }
  
  function togglePause() {
    if (gameState.gameRunning) {
      gameState.gamePaused = !gameState.gamePaused;
      document.getElementById('pause-btn').textContent = gameState.gamePaused ? 'Resume' : 'Pause';
    }
  }
  
  function resetGame() {
    gameState.gameRunning = false;
    gameState.gamePaused = false;
    gameState.grid = Array(gridHeight).fill().map(() => Array(gridWidth).fill(0));
    gameState.score = 0;
    gameState.lines = 0;
    gameState.level = 1;
    gameState.currentPiece = null;
    updateDisplay();
    draw();
    document.getElementById('start-btn').textContent = 'Start';
    document.getElementById('pause-btn').textContent = 'Pause';
  }
  
  // Event listeners
  document.getElementById('start-btn').addEventListener('click', () => {
    if (gameState.gameRunning) {
      resetGame();
    } else {
      startGame();
    }
  });
  
  document.getElementById('pause-btn').addEventListener('click', togglePause);
  document.getElementById('reset-btn').addEventListener('click', resetGame);
  
  // Mobile control handlers
  function handleMobileControl(action) {
    if (!gameState.gameRunning || gameState.gamePaused || !gameState.currentPiece) return;
    
    switch (action) {
      case 'left':
        if (isValidMove(gameState.currentPiece, gameState.currentX - 1, gameState.currentY)) {
          gameState.currentX--;
        }
        break;
      case 'right':
        if (isValidMove(gameState.currentPiece, gameState.currentX + 1, gameState.currentY)) {
          gameState.currentX++;
        }
        break;
      case 'down':
        if (isValidMove(gameState.currentPiece, gameState.currentX, gameState.currentY + 1)) {
          gameState.currentY++;
          gameState.score++;
          updateDisplay();
        }
        break;
      case 'rotate':
        const rotated = rotatePiece(gameState.currentPiece);
        rotated.colorIndex = gameState.currentPiece.colorIndex;
        if (isValidMove(rotated, gameState.currentX, gameState.currentY)) {
          gameState.currentPiece = rotated;
        }
        break;
      case 'drop':
        while (isValidMove(gameState.currentPiece, gameState.currentX, gameState.currentY + 1)) {
          gameState.currentY++;
          gameState.score += 2;
        }
        updateDisplay();
        break;
    }
  }
  
  // Add event listeners for mobile controls
  document.getElementById('left-btn').addEventListener('click', () => handleMobileControl('left'));
  document.getElementById('right-btn').addEventListener('click', () => handleMobileControl('right'));
  document.getElementById('down-btn').addEventListener('click', () => handleMobileControl('down'));
  document.getElementById('rotate-btn').addEventListener('click', () => handleMobileControl('rotate'));
  document.getElementById('drop-btn').addEventListener('click', () => handleMobileControl('drop'));
  
  // Add touch event listeners for better mobile responsiveness
  ['left-btn', 'right-btn', 'down-btn', 'rotate-btn', 'drop-btn'].forEach(id => {
    const btn = document.getElementById(id);
    const action = id.replace('-btn', '');
    
    btn.addEventListener('touchstart', (e) => {
      e.preventDefault();
      handleMobileControl(action);
    });
    
    btn.addEventListener('touchend', (e) => {
      e.preventDefault();
    });
  });
  
  // Keyboard controls
  document.addEventListener('keydown', (e) => {
    if (!gameState.gameRunning || gameState.gamePaused || !gameState.currentPiece) return;
    
    switch (e.code) {
      case 'ArrowLeft':
        if (isValidMove(gameState.currentPiece, gameState.currentX - 1, gameState.currentY)) {
          gameState.currentX--;
        }
        break;
      case 'ArrowRight':
        if (isValidMove(gameState.currentPiece, gameState.currentX + 1, gameState.currentY)) {
          gameState.currentX++;
        }
        break;
      case 'ArrowDown':
        if (isValidMove(gameState.currentPiece, gameState.currentX, gameState.currentY + 1)) {
          gameState.currentY++;
          gameState.score++;
          updateDisplay();
        }
        break;
      case 'ArrowUp':
        const rotated = rotatePiece(gameState.currentPiece);
        rotated.colorIndex = gameState.currentPiece.colorIndex;
        if (isValidMove(rotated, gameState.currentX, gameState.currentY)) {
          gameState.currentPiece = rotated;
        }
        break;
      case 'Space':
        while (isValidMove(gameState.currentPiece, gameState.currentX, gameState.currentY + 1)) {
          gameState.currentY++;
          gameState.score += 2;
        }
        updateDisplay();
        break;
    }
    e.preventDefault();
  });
  
  // Initialize display and canvas
  updateDisplay();
  draw();
}
</script>