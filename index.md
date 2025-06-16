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

body {
  background: linear-gradient(135deg, #0f0f23 0%, #1a1a2e 50%, #16213e 100%);
  color: #e0e0e0;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  line-height: 1.6;
  overflow-x: hidden;
  position: relative;
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
  "Breaking Production Since Forever",
  "Debugging Life, One Server at a Time",
  "Turning Coffee into Uptime",
  "All things Automation"
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
});
</script>