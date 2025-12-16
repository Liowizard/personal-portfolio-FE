<script setup lang="ts">
</script>

<template>
  <div class="hero">
    <div class="intro">
      <div>Hello,</div>
      <div>
        This is <span class="name">Ajesh M</span>,
      </div>
      <div>
        I'm a Professional <span class="role">Software Developer</span>.
      </div>

      <!-- Social Links in a straight line -->
      <div class="social-links">
        <a href="https://github.com/yourusername" target="_blank" rel="noopener">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.387.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61-.546-1.387-1.333-1.757-1.333-1.757-1.09-.744.083-.729.083-.729 1.205.084 1.84 1.236 1.84 1.236 1.07 1.835 2.807 1.305 3.492.998.108-.775.418-1.305.762-1.605-2.665-.3-5.467-1.332-5.467-5.93 0-1.31.467-2.38 1.235-3.22-.123-.303-.536-1.523.117-3.176 0 0 1.008-.322 3.3 1.23a11.52 11.52 0 013-.404c1.02.005 2.045.137 3 .404 2.29-1.552 3.297-1.23 3.297-1.23.655 1.653.242 2.873.12 3.176.77.84 1.232 1.91 1.232 3.22 0 4.61-2.807 5.625-5.48 5.92.43.372.823 1.103.823 2.222 0 1.606-.015 2.898-.015 3.293 0 .322.216.694.825.576C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/>
          </svg>
        </a>

        <a href="https://linkedin.com/in/yourusername" target="_blank" rel="noopener">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
            <path d="M4.98 3.5C4.98 4.88 3.88 6 2.5 6S0 4.88 0 3.5 1.12 1 2.5 1s2.48 1.12 2.48 2.5zM0 8h5v16H0V8zm7.5 0h4.75v2.16h.07c.66-1.25 2.27-2.57 4.68-2.57 5 0 5.92 3.29 5.92 7.57V24h-5V14.14c0-2.34-.04-5.34-3.25-5.34-3.25 0-3.75 2.54-3.75 5.17V24h-5V8z"/>
          </svg>
        </a>

        <a href="mailto:your@email.com" target="_blank" rel="noopener">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 13.065l-12-7.065v14h24v-14l-12 7.065zm0-2.13l12-7.065h-24l12 7.065z"/>
          </svg>
        </a>
      </div>

      <div class="button-group">
        <button class="contact-button">
          Contact Me
          <svg class="icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
            <path d="M2.01 21l20.99-9L2.01 3v7l15 2-15 2z"/>
          </svg>
        </button>

        <button class="cv-button">
          Download CV
          <svg class="icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor">
            <path d="M5 20h14v-2H5v2zm7-18v12l4-4h-3V4h-2v6H8l4 4z"/>
          </svg>
        </button>
      </div>
    </div>

    <div class="code">
      <div class="code-header">
        <span class="dot red"></span>
        <span class="dot yellow"></span>
        <span class="dot green"></span>
      </div>
      <pre><code><span class="keyword">const</span> coder = {
    <span class="property">name</span>: <span class="string">'Ajesh M'</span>,
    <span class="property">skills</span>: [<span class="string">'React'</span>, <span class="string">'NextJS'</span>,<span class="string">'Redux'</span>, <span class="string">'Express'</span>,<span class="string">'AWS'</span>,
        <span class="string">'NestJS'</span>, <span class="string">'MySql'</span>,<span class="string">'MongoDB'</span>, <span class="string">'Docker'</span>],
    <span class="property">hardWorker</span>: <span class="boolean">true</span>,
    <span class="property">quickLearner</span>: <span class="boolean">true</span>,
    <span class="property">problemSolver</span>: <span class="boolean">true</span>,
    <span class="property">hireable</span>: <span class="keyword">function</span>() {
        <span class="keyword">return</span> (
        this.hardWorker &&
        this.problemSolver &&
        this.skills.length >= <span class="number">5</span>
    );
  }
};
</code></pre>
    </div>
  </div>
</template>

<style scoped>
.hero {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  min-height: 55vh;
  padding: 1rem 1rem;
  color: #ffffff;
  flex-wrap: wrap;
  gap: 2rem;
}

.intro {
  flex: 1 1 300px; /* grow, shrink, min width */
  font-size: clamp(1.5rem, 2.5vw, 3rem);
  line-height: 1.3;
}

.name { color: #ed64a6; }
.role { color: #16f2b3; }

.social-links {
  margin-top: 1.5rem;
  display: flex;
  align-items: center;
  gap: 2rem;
  flex-wrap: wrap;
}

.social-links a {
  color: #ed64a6;
  width: 2rem;
  height: 2rem;
  transition: color 0.3s, transform 0.3s;
}

.social-links a:hover {
  color: #16f2b3;
  transform: scale(1.2);
}

.social-links svg { width: 100%; height: 100%; display: block; }

.code {
  flex: 1 1 300px;
  max-width: 100%;
  background: #020617;
  border-radius: 14px;
  box-shadow: 0 20px 50px rgba(0, 0, 0, 0.6);
  border: 1px solid #1e293b;
  overflow: hidden;
}

.code-header {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 12px 16px;
  border-bottom: 1px solid #1e293b;
  background: linear-gradient(180deg, #0f172a, #020617);
}

.dot { width: 14px; height: 14px; border-radius: 50%; }
.dot.red { background: #ff5f56; }
.dot.yellow { background: #ffbd2e; }
.dot.green { background: #27c93f; }

.code pre {
  margin: 0;
  padding: 1.5rem 1.8rem;
  font-family: "JetBrains Mono", "Fira Code", monospace;
  font-size: clamp(0.5rem, 0.9vw, 0.95rem);
  line-height: 1.6;
  color: #d4d4d4;
  overflow-x: auto;
}

.keyword { color: #569cd6; font-weight: 500; }
.string { color: #ce9178; }
.boolean { color: #b5cea8; }
.property { color: #9cdcfe; }
.number { color: #b5cea8; }

.button-group {
  display: flex;
  gap: 1.5rem;
  margin-top: 2rem;
  flex-wrap: wrap;
}

button {
  font-family: 'Poppins', sans-serif;
  font-weight: 600;
  font-size: 1rem;
  padding: 0.7rem 2rem;
  border-radius: 50px;
  border: 2px solid transparent;
  cursor: pointer;
  transition: all 0.3s ease;
  outline: none;
  display: flex;
  align-items: center;
  gap: 0.6rem;
  position: relative;
}

.contact-button {
  background: #ed64a6;
  color: #fff;
  border: 2px solid #ed64a6;
}

.contact-button:hover {
  background: #fff;
  color: #ed64a6;
  transform: scale(1.05);
  box-shadow: 0 8px 20px rgba(237, 100, 166, 0.4);
}

.cv-button {
  background: transparent;
  color: #ed64a6;
  border: 2px solid #ed64a6;
}

.cv-button:hover {
  background: #ed64a6;
  color: #fff;
  transform: scale(1.05);
  box-shadow: 0 8px 20px rgba(237, 100, 166, 0.4);
}

button svg.icon {
  width: 1.3rem;
  height: 1.3rem;
  fill: currentColor;
  transition: transform 0.3s ease;
}

button:hover svg.icon {
  animation: hoverIcon 0.5s ease-in-out forwards;
}

@keyframes hoverIcon {
  0% { transform: scale(1) rotate(0deg); }
  50% { transform: scale(0.6) rotate(-15deg) translateY(-2px); }
  100% { transform: scale(0.6) rotate(0deg) translateY(0); }
}

/* Mobile / small screens */
@media (max-width: 768px) {
  .hero {
    flex-direction: column;
    align-items: flex-start;
    /* padding: 1rem; */
    gap: 1.5rem;
  }

  .intro {
    font-size: 2rem;
  }

  .code pre {
    font-size: 0.43rem;
    padding: 1rem;
  }

  .button-group {
    flex-direction: column;
    gap: 1rem;
  }

  .social-links {
    gap: 1rem;
  }
}
</style>
