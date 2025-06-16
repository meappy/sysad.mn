---
layout: default
title: Gerald Sim - Technology Professional
---

<div class="hero-section">
  <div class="site-title">sysad.mn</div>
  <div class="hero-content">
    <div class="hero-text">
      <h1 class="hero-tagline" id="rotating-tagline">All things Automation</h1>
      <p class="hero-quote">I'm not your typical systems administrator</p>
      <p class="quote-author">— Gerald Sim</p>
    </div>
  </div>
  <div class="hero-decoration">
    <div class="floating-element"></div>
    <div class="floating-element"></div>
    <div class="floating-element"></div>
  </div>
</div>

<section class="expertise-section">
  <div class="section-container">
    <h2 class="section-title">What I Do</h2>
    
    <div class="expertise-cards">
      <div class="expertise-card" data-tilt>
        <div class="card-header">
          <div class="card-icon">🚀</div>
          <h3>Infrastructure Automation</h3>
        </div>
        <div class="card-content">
          <p>Building scalable, reliable systems with modern DevOps practices and Infrastructure as Code</p>
          <div class="card-tags">
            <span class="tag">Terraform</span>
            <span class="tag">Ansible</span>
            <span class="tag">Docker</span>
            <span class="tag">Helm</span>
          </div>
        </div>
      </div>

      <div class="expertise-card" data-tilt>
        <div class="card-header">
          <div class="card-icon">⚡</div>
          <h3>Site Reliability Engineering</h3>
        </div>
        <div class="card-content">
          <p>Building resilient systems with automation and self-healing capabilities to eliminate those dreaded 3am wake-up calls</p>
          <div class="card-tags">
            <span class="tag">Prometheus</span>
            <span class="tag">Grafana</span>
            <span class="tag">K8s</span>
          </div>
        </div>
      </div>

      <div class="expertise-card" data-tilt>
        <div class="card-header">
          <div class="card-icon">🤖</div>
          <h3>AI Tooling</h3>
        </div>
        <div class="card-content">
          <p>Leveraging AI and automation tools to streamline development and operational workflows</p>
          <div class="card-tags">
            <span class="tag">Claude</span>
            <span class="tag">GPT</span>
            <span class="tag">Cursor</span>
            <span class="tag">Workflows</span>
          </div>
        </div>
      </div>

      <div class="expertise-card" data-tilt>
        <div class="card-header">
          <div class="card-icon">🔄</div>
          <h3>DevOps Practices</h3>
        </div>
        <div class="card-content">
          <p>Bridging development and operations with CI/CD pipelines and automated workflows</p>
          <div class="card-tags">
            <span class="tag">GitHub Actions</span>
            <span class="tag">Azure DevOps</span>
          </div>
        </div>
      </div>

      <div class="expertise-card" data-tilt>
        <div class="card-header">
          <div class="card-icon">☁️</div>
          <h3>Cloud Architecture</h3>
        </div>
        <div class="card-content">
          <p>Designing cloud-native solutions for scalability, security, and cost optimization</p>
          <div class="card-tags">
            <span class="tag">AWS</span>
            <span class="tag">Azure</span>
            <span class="tag">GCP</span>
          </div>
        </div>
      </div>

    </div>
  </div>
</section>

<section class="tetris-section">
  <div class="section-container">
    <h2 class="section-title">Terminal Tetris</h2>
    <p class="section-subtitle">Because even sysadmins need a break from fixing production</p>
    
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
            <button id="down-btn" class="mobile-btn">↓</button>
          </div>
          <div class="mobile-controls-right">
            <button id="left-btn" class="mobile-btn">←</button>
            <button id="right-btn" class="mobile-btn">→</button>
            <button id="drop-btn" class="mobile-btn">⬇</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="contact-section">
  <div class="section-container">
    <h2 class="section-title">Get In Touch</h2>
    <p class="section-subtitle">Interested in automation, infrastructure, or just want to chat about tech?</p>
    
    <div class="contact-actions">
      <a href="/assets/cv/gerald-sim-cv.pdf" class="contact-item cv-download" target="_blank">
        <span class="contact-icon">📄</span>
        <span class="contact-label">Download CV</span>
      </a>
      
      <a href="https://www.linkedin.com/in/geraldsim/" class="contact-item linkedin" target="_blank">
        <span class="contact-icon">in</span>
        <span class="contact-label">LinkedIn</span>
      </a>
      
      <a href="https://github.com/meappy" class="contact-item github" target="_blank">
        <span class="contact-icon">gh</span>
        <span class="contact-label">GitHub</span>
      </a>
    </div>
  </div>
</section>

<style>
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
    radial-gradient(circle at 20% 30%, rgba(59, 130, 246, 0.15) 0%, transparent 50%),
    radial-gradient(circle at 80% 60%, rgba(139, 92, 246, 0.12) 0%, transparent 50%),
    radial-gradient(circle at 40% 80%, rgba(100, 255, 218, 0.08) 0%, transparent 50%),
    radial-gradient(circle at 90% 20%, rgba(59, 130, 246, 0.1) 0%, transparent 50%),
    radial-gradient(circle at 10% 90%, rgba(139, 92, 246, 0.1) 0%, transparent 50%);
  animation: lavaLamp 20s ease-in-out infinite;
  pointer-events: none;
  z-index: -1;
}

/* Hero Section */
.hero-section {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: relative;
  padding: 2rem;
}

.site-title {
  position: absolute;
  top: 2rem;
  font-size: clamp(1.2rem, 3vw, 1.6rem);
  color: #ffffff;
  font-weight: 700;
  letter-spacing: 2px;
  text-transform: uppercase;
  font-family: 'SF Mono', 'Monaco', 'Cascadia Code', 'Roboto Mono', Consolas, 'Courier New', monospace;
  animation: fadeInUp 1s ease-out;
  text-shadow: 0 0 20px rgba(255, 255, 255, 0.3);
}

.hero-content {
  max-width: 800px;
  text-align: center;
  z-index: 2;
  position: relative;
}

.hero-tagline {
  font-size: clamp(3rem, 8vw, 5rem);
  font-weight: 700;
  margin-bottom: 2rem;
  background: linear-gradient(135deg, #64ffda, #3b82f6, #8b5cf6);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: fadeInUp 1s ease-out 0.2s both;
  min-height: 1.2em;
  transition: opacity 0.5s ease;
}

.hero-quote {
  font-size: clamp(1rem, 3vw, 1.3rem);
  color: #94a3b8;
  margin: 0 auto 1rem auto;
  animation: fadeInUp 1s ease-out 0.4s both;
  font-weight: 400;
  line-height: 1.5;
  max-width: 600px;
  font-style: italic;
  opacity: 0.9;
  text-align: center;
  font-family: 'Playfair Display', 'Georgia', 'Times New Roman', serif;
  position: relative;
  letter-spacing: 0.5px;
}

.hero-quote::before {
  content: '"';
  font-size: 4rem;
  color: rgba(100, 255, 218, 0.3);
  position: absolute;
  left: -2rem;
  top: -1rem;
  font-family: 'Georgia', serif;
  line-height: 1;
}

.hero-quote::after {
  content: '"';
  font-size: 4rem;
  color: rgba(100, 255, 218, 0.3);
  position: absolute;
  right: -2rem;
  bottom: -2rem;
  font-family: 'Georgia', serif;
  line-height: 1;
}

.quote-author {
  font-size: clamp(0.9rem, 2vw, 1.1rem);
  color: #64ffda;
  margin: 0 auto 3rem auto;
  animation: fadeInUp 1s ease-out 0.6s both;
  font-weight: 500;
  text-align: center;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  opacity: 0.8;
  letter-spacing: 1px;
}

.hero-actions {
  display: flex;
  gap: 1.5rem;
  justify-content: center;
  flex-wrap: wrap;
  animation: fadeInUp 1s ease-out 0.8s both;
}

.cv-button-container {
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 2rem;
}

.hand-drawn-arrow {
  width: 80px;
  height: 50px;
  position: absolute;
  top: -40px;
  left: -30px;
  transform: rotate(35deg);
  opacity: 0.7;
  animation: drawArrow 2s ease-in-out 2s both, wiggle 3s ease-in-out 4s infinite;
}

@keyframes drawArrow {
  0% {
    stroke-dasharray: 200;
    stroke-dashoffset: 200;
    opacity: 0;
  }
  100% {
    stroke-dasharray: 200;
    stroke-dashoffset: 0;
    opacity: 0.8;
  }
}

@keyframes wiggle {
  0%, 100% {
    transform: rotate(35deg);
  }
  25% {
    transform: rotate(40deg);
  }
  75% {
    transform: rotate(30deg);
  }
}

@keyframes lavaLamp {
  0%, 100% {
    background: 
      radial-gradient(circle at 20% 30%, rgba(59, 130, 246, 0.15) 0%, transparent 50%),
      radial-gradient(circle at 80% 60%, rgba(139, 92, 246, 0.12) 0%, transparent 50%),
      radial-gradient(circle at 40% 80%, rgba(100, 255, 218, 0.08) 0%, transparent 50%),
      radial-gradient(circle at 90% 20%, rgba(59, 130, 246, 0.1) 0%, transparent 50%),
      radial-gradient(circle at 10% 90%, rgba(139, 92, 246, 0.1) 0%, transparent 50%);
  }
  25% {
    background: 
      radial-gradient(circle at 30% 50%, rgba(59, 130, 246, 0.18) 0%, transparent 55%),
      radial-gradient(circle at 70% 40%, rgba(139, 92, 246, 0.15) 0%, transparent 55%),
      radial-gradient(circle at 60% 70%, rgba(100, 255, 218, 0.1) 0%, transparent 55%),
      radial-gradient(circle at 85% 30%, rgba(59, 130, 246, 0.12) 0%, transparent 55%),
      radial-gradient(circle at 15% 80%, rgba(139, 92, 246, 0.08) 0%, transparent 55%);
  }
  50% {
    background: 
      radial-gradient(circle at 60% 70%, rgba(59, 130, 246, 0.12) 0%, transparent 50%),
      radial-gradient(circle at 30% 20%, rgba(139, 92, 246, 0.18) 0%, transparent 50%),
      radial-gradient(circle at 80% 50%, rgba(100, 255, 218, 0.12) 0%, transparent 50%),
      radial-gradient(circle at 70% 80%, rgba(59, 130, 246, 0.08) 0%, transparent 50%),
      radial-gradient(circle at 20% 60%, rgba(139, 92, 246, 0.15) 0%, transparent 50%);
  }
  75% {
    background: 
      radial-gradient(circle at 80% 40%, rgba(59, 130, 246, 0.16) 0%, transparent 52%),
      radial-gradient(circle at 20% 80%, rgba(139, 92, 246, 0.10) 0%, transparent 52%),
      radial-gradient(circle at 50% 30%, rgba(100, 255, 218, 0.14) 0%, transparent 52%),
      radial-gradient(circle at 10% 40%, rgba(59, 130, 246, 0.12) 0%, transparent 52%),
      radial-gradient(circle at 90% 70%, rgba(139, 92, 246, 0.12) 0%, transparent 52%);
  }
}

.cta-button {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 1rem 2rem;
  border-radius: 50px;
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s ease;
  border: 2px solid transparent;
  min-width: 160px;
  justify-content: center;
}

.cta-button.primary {
  background: linear-gradient(135deg, #3b82f6, #8b5cf6);
  color: white;
}

.cta-button.primary:hover {
  transform: translateY(-3px);
  box-shadow: 0 10px 30px rgba(59, 130, 246, 0.4);
}

.cta-button.secondary {
  background: transparent;
  color: #64ffda;
  border-color: #64ffda;
}

.cta-button.secondary:hover {
  background: rgba(100, 255, 218, 0.1);
  transform: translateY(-3px);
}

/* Floating Elements - Now more subtle since we have lava lamp background */
.hero-decoration {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  pointer-events: none;
}

.floating-element {
  position: absolute;
  width: 60px;
  height: 60px;
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.05), rgba(139, 92, 246, 0.05));
  border-radius: 50%;
  animation: float 8s ease-in-out infinite;
}

.floating-element:nth-child(1) {
  top: 20%;
  left: 10%;
  animation-delay: 0s;
}

.floating-element:nth-child(2) {
  top: 60%;
  right: 10%;
  animation-delay: 3s;
}

.floating-element:nth-child(3) {
  bottom: 20%;
  left: 20%;
  animation-delay: 6s;
}

/* Section Styles */
.section-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 5rem 2rem;
}

.section-title {
  font-size: clamp(2.5rem, 6vw, 3.5rem);
  text-align: center;
  margin-bottom: 3rem;
  color: #ffffff;
}

.section-subtitle {
  font-size: 1.2rem;
  text-align: center;
  color: #94a3b8;
  margin-bottom: 3rem;
}

/* Expertise Section */
.expertise-section {
  background: rgba(0, 0, 0, 0.3);
  backdrop-filter: blur(10px);
}

.expertise-cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin-top: 3rem;
}

.expertise-card {
  background: rgba(26, 26, 26, 0.8);
  border: 1px solid rgba(100, 255, 218, 0.2);
  border-radius: 20px;
  padding: 2rem;
  transition: all 0.3s ease;
  backdrop-filter: blur(10px);
  cursor: pointer;
}

.expertise-card:hover {
  transform: translateY(-10px);
  border-color: #64ffda;
  box-shadow: 0 20px 40px rgba(100, 255, 218, 0.2);
}

.card-header {
  margin-bottom: 1.5rem;
}

.card-icon {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.card-header h3 {
  font-size: 1.5rem;
  color: #ffffff;
  margin-bottom: 1rem;
}

.card-content p {
  color: #94a3b8;
  margin-bottom: 1.5rem;
  line-height: 1.6;
}

.card-tags {
  display: flex;
  gap: 0.5rem;
  flex-wrap: wrap;
}

.tag {
  background: rgba(59, 130, 246, 0.2);
  color: #3b82f6;
  padding: 0.3rem 0.8rem;
  border-radius: 15px;
  font-size: 0.8rem;
  font-weight: 500;
}


/* Contact Section */
.contact-section {
  background: rgba(0, 0, 0, 0.4);
}

.contact-actions {
  display: flex;
  gap: 3rem;
  justify-content: center;
  flex-wrap: wrap;
  max-width: 700px;
  margin: 0 auto;
}

.contact-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
  text-decoration: none;
  color: #94a3b8;
  transition: all 0.3s ease;
  padding: 1.5rem;
  border-radius: 12px;
  min-width: 120px;
}

.contact-item:hover {
  color: #ffffff;
  transform: translateY(-3px);
}

.contact-item.cv-download:hover {
  background: rgba(59, 130, 246, 0.1);
  color: #3b82f6;
}

.contact-item.linkedin:hover {
  background: rgba(0, 119, 181, 0.1);
  color: #0077b5;
}

.contact-item.github:hover {
  background: rgba(255, 255, 255, 0.1);
  color: #ffffff;
}

.contact-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 60px;
  height: 60px;
  border: 2px solid currentColor;
  border-radius: 50%;
  font-size: 1.5rem;
  font-weight: 600;
  transition: all 0.3s ease;
}

.contact-item.cv-download .contact-icon {
  font-size: 1.8rem;
}

.contact-item.linkedin .contact-icon,
.contact-item.github .contact-icon {
  font-family: 'SF Mono', 'Monaco', 'Cascadia Code', 'Roboto Mono', Consolas, 'Courier New', monospace;
  text-transform: lowercase;
}

.contact-item:hover .contact-icon {
  background: currentColor;
  color: #0a0a0a;
  transform: scale(1.1);
}

.contact-label {
  font-size: 1rem;
  font-weight: 500;
  letter-spacing: 0.5px;
}

/* Animations */
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

@keyframes float {
  0%, 100% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-20px);
  }
}

/* Tetris Section */
.tetris-section {
  background: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(10px);
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

/* Responsive Design */
@media (max-width: 768px) {
  .section-container {
    padding: 3rem 1rem;
  }
  
  .expertise-cards {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  
  .contact-actions {
    gap: 2rem;
  }
  
  .hero-actions {
    flex-direction: column;
    align-items: center;
  }
  
  .cta-button {
    width: 200px;
  }
  
  .floating-element {
    width: 60px;
    height: 60px;
  }
  
  /* Tetris responsive */
  .tetris-container {
    flex-direction: column;
    align-items: center;
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
  .expertise-card,
  .contact-card {
    padding: 1.5rem;
  }
  
  .card-icon {
    font-size: 2.5rem;
  }
  
  .hero-section {
    padding: 1rem;
  }
  
  /* Additional mobile fixes */
  .hero-content {
    padding: 0 1rem;
  }
  
  .hero-quote::before,
  .hero-quote::after {
    display: none;
  }
  
  .site-footer {
    margin: 0;
    width: 100vw;
    max-width: 100vw;
    left: 0;
    right: 0;
  }
  
  /* Ensure all sections don't overflow */
  section {
    overflow-x: hidden;
    width: 100%;
  }
  
  /* Prevent any element from causing horizontal scroll */
  * {
    max-width: 100vw !important;
  }
}
</style>

<script>
// Rotating taglines
const taglines = [
  "SSH Into My World",
  "Born to Automate, Forced to Document", 
  "Infrastructure Therapist",
  "Living That Terminal Life",
  "Terminal Velocity Engineer",
  "Shell Shocked and Loving It",
  "Bash Me Baby One More Time",
  "Life in the Command Line",
  "Terminal Addiction Support Group",
  "Ctrl+C, Ctrl+V, Ctrl+Life",
  "It's Not a Bug, It's a Feature Request",
  "May the Logs Be With You",
  "Kubernetes and Chill",
  "Error 404: Sleep Not Found",
  "Professional Yak Shaver",
  "Sudo Make Me a Sandwich",
  "99 Problems But Uptime Ain't One",
  "Localhost Sweet Localhost",
  "The Empire Strikes Back(up)",
  "Game of Nodes",
  "Debugging Life, One Server at a Time",
  "Turning Coffee into Uptime",
  "All things Automation",
  "Chaos Engineering Enthusiast",
  "DevOps Sorcerer",
  "Cloud Native, Coffee Positive",
  "Terraform Destroyer of Worlds",
  "Pipeline Dreams and Docker Schemes",
  "Git Push and Pray",
  "Automate All The Things",
  "Scaling Mountains, Scaling Systems",
  "Zero Downtime Hero",
  "Container Orchestration Maestro",
  "Infrastructure as Code Poet",
  "Monitoring Everything That Moves",
  "YAML Engineer Extraordinaire",
  "Incident Response Ninja",
  "CI/CD Pipeline Plumber",
  "Serverless But Not Sleepless",
  "Making Servers Purr Since 2010",
  "Professional YAML Whisperer",
  "Deployment Velocity Maximizer",
  "SRE: Sleep Rarely Expected",
  "Ansible Playbook Author",
  "Prometheus Fire Stealer",
  "Grafana Dashboard Artist",
  "Load Balancer Juggler",
  "Microservices Wrangler",
  "Log Analysis Detective",
  "Performance Optimisation Wizard"
];

function rotateTagline() {
  const taglineElement = document.getElementById('rotating-tagline');
  if (taglineElement) {
    const randomTagline = taglines[Math.floor(Math.random() * taglines.length)];
    
    // Fade out
    taglineElement.style.opacity = '0';
    
    // Change text and fade in
    setTimeout(() => {
      taglineElement.textContent = randomTagline;
      taglineElement.style.opacity = '1';
    }, 250);
  }
}

// Set initial random tagline on page load
document.addEventListener('DOMContentLoaded', function() {
  rotateTagline();
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