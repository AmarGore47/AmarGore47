## Hi there 👋

<!--
**AmarGore47/AmarGore47** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
AMAR GORE
XR DEVELOPER

AR/VR • WebXR • Unity • AI • 3D

━━━━━━━━━━━━━━━━━━━━

ABOUT ME

B.Tech CSE (AR/VR) student building
immersive experiences and interactive applications.

━━━━━━━━━━━━━━━━━━━━

TECH STACK

Unity | C# | WebXR | Three.js
Blender | AR Foundation
OpenXR | MediaPipe | Git

━━━━━━━━━━━━━━━━━━━━

FEATURED PROJECTS

🥽 WebXR Experiences
🏏 AR Cricket
🎮 Unity Games
🌐 Interactive XR Projects
🤖 AI / Computer Vision
🎨 Projection Mapping

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AMAR GORE // SPATIAL WEBXR ARCHITECT</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;600;700&family=Orbitron:wght@500;700;900&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #050811;
      --cyan: #00f0ff;
      --magenta: #ff007f;
      --green: #00ff66;
      --purple: #7c3aed;
      --gold: #facc15;
      --glass: rgba(10, 16, 32, 0.75);
      --border: rgba(0, 240, 255, 0.25);
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Fira Code', monospace;
    }

    body {
      background-color: var(--bg);
      color: #e2e8f0;
      overflow-x: hidden;
      min-height: 100vh;
      background-image: 
        radial-gradient(circle at 50% 0%, rgba(124, 58, 237, 0.15), transparent 70%),
        radial-gradient(circle at 10% 80%, rgba(0, 240, 255, 0.1), transparent 50%);
    }

    /* Cyberpunk Scanline Effect */
    body::before {
      content: "";
      position: fixed;
      top: 0; left: 0; width: 100vw; height: 100vh;
      background: linear-gradient(rgba(18, 16, 16, 0) 50%, rgba(0, 0, 0, 0.25) 50%);
      background-size: 100% 4px;
      z-index: 99;
      pointer-events: none;
      opacity: 0.6;
    }

    #bg-canvas {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      z-index: 0;
      pointer-events: none;
    }

    .container {
      position: relative;
      z-index: 10;
      max-width: 1200px;
      margin: 0 auto;
      padding: 2rem 1.5rem;
    }

    header {
      text-align: center;
      padding: 3rem 1rem 2rem;
      position: relative;
    }

    .status-badge {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      background: rgba(0, 240, 255, 0.1);
      border: 1px solid var(--cyan);
      padding: 0.4rem 1.2rem;
      border-radius: 50px;
      font-size: 0.85rem;
      color: var(--cyan);
      letter-spacing: 2px;
      text-transform: uppercase;
      box-shadow: 0 0 15px rgba(0, 240, 255, 0.2);
      margin-bottom: 1.5rem;
      animation: pulse 2s infinite alternate;
    }

    @keyframes pulse {
      0% { box-shadow: 0 0 10px rgba(0, 240, 255, 0.2); }
      100% { box-shadow: 0 0 25px rgba(0, 240, 255, 0.6); }
    }

    .dot {
      width: 8px;
      height: 8px;
      background-color: var(--green);
      border-radius: 50%;
      box-shadow: 0 0 8px var(--green);
    }

    h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: clamp(2.2rem, 6vw, 4.2rem);
      font-weight: 900;
      background: linear-gradient(135deg, #ffffff 0%, var(--cyan) 50%, var(--magenta) 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      letter-spacing: 2px;
      text-shadow: 0 0 30px rgba(0, 240, 255, 0.3);
      margin-bottom: 0.5rem;
    }

    .subtitle {
      font-size: 1.1rem;
      color: #94a3b8;
      max-width: 700px;
      margin: 0 auto 2rem;
      line-height: 1.6;
    }

    .btn-group {
      display: flex;
      justify-content: center;
      gap: 1rem;
      flex-wrap: wrap;
    }

    .cyber-btn {
      position: relative;
      padding: 0.8rem 1.8rem;
      background: var(--glass);
      border: 1px solid var(--cyan);
      color: var(--cyan);
      font-family: 'Orbitron', sans-serif;
      font-size: 0.9rem;
      font-weight: 700;
      letter-spacing: 1px;
      cursor: pointer;
      text-decoration: none;
      overflow: hidden;
      transition: all 0.3s ease;
      backdrop-filter: blur(10px);
      clip-path: polygon(10px 0, 100% 0, 100% calc(100% - 10px), calc(100% - 10px) 100%, 0 100%, 0 10px);
    }

    .cyber-btn:hover {
      background: var(--cyan);
      color: var(--bg);
      box-shadow: 0 0 25px var(--cyan);
      transform: translateY(-2px);
    }

    .cyber-btn.magenta {
      border-color: var(--magenta);
      color: var(--magenta);
    }

    .cyber-btn.magenta:hover {
      background: var(--magenta);
      color: #fff;
      box-shadow: 0 0 25px var(--magenta);
    }

    /* Grid Sections */
    .section-title {
      font-family: 'Orbitron', sans-serif;
      font-size: 1.6rem;
      color: #fff;
      margin: 3rem 0 1.5rem;
      display: flex;
      align-items: center;
      gap: 1rem;
    }

    .section-title::after {
      content: "";
      flex: 1;
      height: 1px;
      background: linear-gradient(90deg, var(--cyan), transparent);
    }

    .project-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
      gap: 1.5rem;
    }

    .card {
      background: var(--glass);
      border: 1px solid var(--border);
      padding: 1.8rem;
      border-radius: 12px;
      backdrop-filter: blur(12px);
      transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
      position: relative;
      overflow: hidden;
    }

    .card::before {
      content: "";
      position: absolute;
      top: 0; left: 0; width: 4px; height: 100%;
      background: var(--cyan);
      transition: width 0.3s ease;
    }

    .card:hover {
      transform: translateY(-8px) scale(1.02);
      border-color: var(--cyan);
      box-shadow: 0 10px 30px rgba(0, 240, 255, 0.25);
    }

    .card:hover::before {
      width: 100%;
      opacity: 0.05;
    }

    .card-icon {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    .card-title {
      font-family: 'Orbitron', sans-serif;
      font-size: 1.3rem;
      color: #fff;
      margin-bottom: 0.6rem;
    }

    .card-desc {
      color: #94a3b8;
      font-size: 0.92rem;
      line-height: 1.6;
      margin-bottom: 1.2rem;
    }

    .card-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem;
      margin-bottom: 1.2rem;
    }

    .tag {
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid rgba(255, 255, 255, 0.1);
      padding: 0.2rem 0.6rem;
      border-radius: 4px;
      font-size: 0.75rem;
      color: var(--cyan);
    }

    /* Terminal Window */
    .terminal-container {
      background: rgba(5, 8, 17, 0.9);
      border: 1px solid var(--cyan);
      border-radius: 10px;
      overflow: hidden;
      margin: 3rem 0;
      box-shadow: 0 0 30px rgba(0, 240, 255, 0.15);
    }

    .terminal-header {
      background: rgba(0, 240, 255, 0.1);
      padding: 0.6rem 1rem;
      display: flex;
      align-items: center;
      gap: 0.5rem;
      border-bottom: 1px solid var(--border);
    }

    .term-btn {
      width: 12px;
      height: 12px;
      border-radius: 50%;
    }
    .red { background: #ff5f56; }
    .yellow { background: #ffbd2e; }
    .green { background: #27c93f; }

    .term-title {
      margin-left: auto;
      margin-right: auto;
      font-size: 0.8rem;
      color: #94a3b8;
      letter-spacing: 1px;
    }

    .terminal-body {
      padding: 1.2rem;
      min-height: 220px;
      max-height: 350px;
      overflow-y: auto;
      font-size: 0.9rem;
      line-height: 1.6;
    }

    .term-line {
      margin-bottom: 0.4rem;
    }

    .prompt {
      color: var(--cyan);
      font-weight: bold;
    }

    .input-line {
      display: flex;
      gap: 0.5rem;
      align-items: center;
    }

    #term-input {
      background: transparent;
      border: none;
      outline: none;
      color: var(--green);
      font-family: 'Fira Code', monospace;
      font-size: 0.9rem;
      flex: 1;
    }

    /* Interactive Slingshot Simulator Canvas */
    .sim-container {
      background: var(--glass);
      border: 1px solid var(--magenta);
      border-radius: 12px;
      padding: 1.5rem;
      margin-top: 2rem;
      text-align: center;
    }

    #sim-canvas {
      background: #090d1a;
      border: 1px solid rgba(255, 0, 127, 0.3);
      border-radius: 8px;
      width: 100%;
      max-width: 800px;
      height: 300px;
      cursor: crosshair;
      margin-top: 1rem;
    }

    footer {
      text-align: center;
      padding: 3rem 1rem 1rem;
      color: #64748b;
      font-size: 0.85rem;
    }

    footer a {
      color: var(--cyan);
      text-decoration: none;
    }
  </style>
</head>
<body>

  <!-- Background Particle Animation Canvas -->
  <canvas id="bg-canvas"></canvas>

  <div class="container">
    <header>
      <div class="status-badge">
        <span class="dot"></span> QUEST 3S WEBXR HAND-TRACKING MATRIX ACTIVE
      </div>
      <h1>AMAR GORE</h1>
      <p class="subtitle">
        B.Tech CSE (AR/VR Specialization) • WebXR & Spatial Computing Architect.<br/>
        Building bare-hand tracking 3D VR physics engines & interactive projection systems.
      </p>

      <div class="btn-group">
        <a href="https://github.com/AmarGore47/Vr_Game" target="_blank" class="cyber-btn">🥽 XR SLINGSHOT VR REPO</a>
        <a href="https://amar-gore-prortfolio.vercel.app" target="_blank" class="cyber-btn magenta">🎨 LIVE 3D PORTFOLIO</a>
        <button onclick="playCyberSound()" class="cyber-btn">🔊 SYNTH AUDIO SFX</button>
      </div>
    </header>

    <!-- Interactive Cyber Terminal -->
    <div class="terminal-container">
      <div class="terminal-header">
        <div class="term-btn red"></div>
        <div class="term-btn yellow"></div>
        <div class="term-btn green"></div>
        <div class="term-title">AMAR_GORE_CYBER_TERMINAL_v2.6</div>
      </div>
      <div class="terminal-body" id="term-body">
        <div class="term-line"><span class="prompt">system@amar-gore:~$</span> status</div>
        <div class="term-line" style="color: var(--green);">[OK] Hand Tracking Keypoints: 21 Landmarks active</div>
        <div class="term-line" style="color: var(--cyan);">[OK] Quest 3S WebXR Session: READY</div>
        <div class="term-line" style="color: var(--gold);">[HINT] Type 'help', 'projects', 'skills', or 'vr' below:</div>
        <div class="input-line">
          <span class="prompt">system@amar-gore:~$</span>
          <input type="text" id="term-input" placeholder="Type a command and press Enter..." autofocus />
        </div>
      </div>
    </div>

    <!-- Featured Spatial Projects Grid -->
    <h2 class="section-title">FEATURED SPATIAL PROJECTS</h2>
    <div class="project-grid">
      
      <div class="card">
        <div class="card-icon">🥽</div>
        <h3 class="card-title">XR Slingshot VR (Quest 3S)</h3>
        <p class="card-desc">
          Controller-free hand tracking Angry Birds VR slingshot game. Pinch thumb and index fingers to pull slingshot pouch and release with 3D physics!
        </p>
        <div class="card-tags">
          <span class="tag">A-Frame 1.6</span>
          <span class="tag">WebXR API</span>
          <span class="tag">Hand Tracking</span>
          <span class="tag">Web Audio Synthesizer</span>
        </div>
        <a href="https://github.com/AmarGore47/Vr_Game" target="_blank" class="cyber-btn" style="display: inline-block; padding: 0.5rem 1rem; font-size: 0.8rem;">LAUNCH REPO</a>
      </div>

      <div class="card">
        <div class="card-icon">🖐️</div>
        <h3 class="card-title">Hand-Tracking AR Cricket</h3>
        <p class="card-desc">
          Real-time webcam hand gesture tracking AR experience for playing cricket using computer vision & 3D WebGL collision detection.
        </p>
        <div class="card-tags">
          <span class="tag">MediaPipe</span>
          <span class="tag">WebXR</span>
          <span class="tag">Computer Vision</span>
          <span class="tag">JavaScript</span>
        </div>
        <a href="https://github.com/AmarGore47/Hand-tracking-AR-cricket-experience" target="_blank" class="cyber-btn" style="display: inline-block; padding: 0.5rem 1rem; font-size: 0.8rem;">LAUNCH REPO</a>
      </div>

      <div class="card">
        <div class="card-icon">📐</div>
        <h3 class="card-title">Floor Projection Interactive</h3>
        <p class="card-desc">
          Interactive motion-tracking floor projection mapping system capturing user footstep movement for real-time visual reactions.
        </p>
        <div class="card-tags">
          <span class="tag">Interactive Projection</span>
          <span class="tag">Motion Sensor</span>
          <span class="tag">Canvas 2D</span>
        </div>
        <a href="https://amargore47.github.io/floor-projection-interactive/" target="_blank" class="cyber-btn magenta" style="display: inline-block; padding: 0.5rem 1rem; font-size: 0.8rem;">LIVE DEMO</a>
      </div>

    </div>

    <!-- Mini Hand Tracking Slingshot Simulator Canvas -->
    <div class="sim-container">
      <h2 style="font-family: 'Orbitron', sans-serif; color: var(--magenta);">🖐️ INTERACTIVE 2D HAND-PINCH SLINGSHOT SIMULATOR</h2>
      <p style="color: #94a3b8; font-size: 0.9rem; margin-top: 0.5rem;">
        Click & Drag back on the bird inside the circle, then release to launch with physics!
      </p>
      <canvas id="sim-canvas"></canvas>
    </div>

    <footer>
      <p>Designed & Engineered by <a href="https://github.com/AmarGore47" target="_blank">Amar Gore</a> • Spatial WebXR Architect © 2026</p>
    </footer>
  </div>

  <script>
    /* Background Cyber Matrix Particles Canvas */
    const canvas = document.getElementById('bg-canvas');
    const ctx = canvas.getContext('2d');
    let width, height;

    function resize() {
      width = canvas.width = window.innerWidth;
      height = canvas.height = window.innerHeight;
    }
    window.addEventListener('resize', resize);
    resize();

    const particles = [];
    for(let i=0; i<70; i++) {
      particles.push({
        x: Math.random() * width,
        y: Math.random() * height,
        vx: (Math.random() - 0.5) * 0.8,
        vy: (Math.random() - 0.5) * 0.8,
        size: Math.random() * 2 + 1,
        color: Math.random() > 0.5 ? '#00f0ff' : '#ff007f'
      });
    }

    function animateParticles() {
      ctx.clearRect(0, 0, width, height);

      // Draw grid lines
      ctx.strokeStyle = 'rgba(0, 240, 255, 0.03)';
      ctx.lineWidth = 1;
      const gridSize = 60;
      for(let x=0; x<width; x+=gridSize) {
        ctx.beginPath(); ctx.moveTo(x, 0); ctx.lineTo(x, height); ctx.stroke();
      }
      for(let y=0; y<height; y+=gridSize) {
        ctx.beginPath(); ctx.moveTo(0, y); ctx.lineTo(width, y); ctx.stroke();
      }

      particles.forEach((p, idx) => {
        p.x += p.vx;
        p.y += p.vy;
        if(p.x < 0 || p.x > width) p.vx *= -1;
        if(p.y < 0 || p.y > height) p.vy *= -1;

        ctx.fillStyle = p.color;
        ctx.beginPath();
        ctx.arc(p.x, p.y, p.size, 0, Math.PI * 2);
        ctx.fill();

        // Connect nearby particles
        for(let j = idx + 1; j < particles.length; j++) {
          const p2 = particles[j];
          const dist = Math.hypot(p.x - p2.x, p.y - p2.y);
          if(dist < 130) {
            ctx.strokeStyle = `rgba(0, 240, 255, ${0.15 * (1 - dist/130)})`;
            ctx.beginPath(); ctx.moveTo(p.x, p.y); ctx.lineTo(p2.x, p2.y); ctx.stroke();
          }
        }
      });

      requestAnimationFrame(animateParticles);
    }
    animateParticles();

    /* Web Audio API Sound Synthesizer */
    function playCyberSound() {
      try {
        const audioCtx = new (window.AudioContext || window.webkitAudioContext)();
        const osc = audioCtx.createOscillator();
        const gain = audioCtx.createGain();
        osc.type = 'sawtooth';
        osc.frequency.setValueAtTime(440, audioCtx.currentTime);
        osc.frequency.exponentialRampToValueAtTime(880, audioCtx.currentTime + 0.3);
        gain.gain.setValueAtTime(0.2, audioCtx.currentTime);
        gain.gain.exponentialRampToValueAtTime(0.01, audioCtx.currentTime + 0.3);
        osc.connect(gain);
        gain.connect(audioCtx.destination);
        osc.start();
        osc.stop(audioCtx.currentTime + 0.3);
      } catch(e) {}
    }

    /* Terminal System Logic */
    const termInput = document.getElementById('term-input');
    const termBody = document.getElementById('term-body');

    termInput.addEventListener('keydown', (e) => {
      if(e.key === 'Enter') {
        const val = termInput.value.trim().toLowerCase();
        termInput.value = '';
        
        const line = document.createElement('div');
        line.className = 'term-line';
        line.innerHTML = `<span class="prompt">system@amar-gore:~$</span> ${val}`;
        termBody.insertBefore(line, termInput.parentElement);

        let resp = '';
        if(val === 'help') {
          resp = '<span style="color: var(--cyan);">Available commands: <b>projects</b>, <b>skills</b>, <b>vr</b>, <b>contact</b>, <b>clear</b></span>';
        } else if(val === 'projects') {
          resp = '<span style="color: var(--green);">1. XR Slingshot VR (Quest 3S Bare-Hand Tracking)<br/>2. Hand-Tracking AR Cricket<br/>3. Floor Projection Interactive<br/>4. 3D Developer Portfolio</span>';
        } else if(val === 'skills') {
          resp = '<span style="color: var(--gold);">WebXR, Three.js, A-Frame, MediaPipe Hand Tracking, GLSL Shaders, TypeScript, React, Vite</span>';
        } else if(val === 'vr') {
          resp = '<span style="color: var(--magenta);">🥽 Meta Quest 3S WebXR Slingshot Game initialized! Pinch thumb & index finger to pull & launch Angry Birds!</span>';
        } else if(val === 'clear') {
          const lines = termBody.querySelectorAll('.term-line');
          lines.forEach(l => l.remove());
          return;
        } else {
          resp = `<span style="color: #ff5f56;">Command not recognized: '${val}'. Type <b>'help'</b> for commands.</span>`;
        }

        const respLine = document.createElement('div');
        respLine.className = 'term-line';
        respLine.innerHTML = resp;
        termBody.insertBefore(respLine, termInput.parentElement);
        termBody.scrollTop = termBody.scrollHeight;
        playCyberSound();
      }
    });

    /* Interactive Slingshot Simulator Canvas */
    const simCanvas = document.getElementById('sim-canvas');
    const sCtx = simCanvas.getContext('2d');
    simCanvas.width = 800;
    simCanvas.height = 300;

    const anchorX = 150;
    const anchorY = 200;
    let birdX = anchorX;
    let birdY = anchorY;
    let isDragging = false;
    let isFlying = false;
    let vx = 0, vy = 0;

    simCanvas.addEventListener('mousedown', (e) => {
      const rect = simCanvas.getBoundingClientRect();
      const mx = e.clientX - rect.left;
      const my = e.clientY - rect.top;
      if(Math.hypot(mx - birdX, my - birdY) < 40) {
        isDragging = true;
        isFlying = false;
      }
    });

    simCanvas.addEventListener('mousemove', (e) => {
      if(isDragging) {
        const rect = simCanvas.getBoundingClientRect();
        birdX = e.clientX - rect.left;
        birdY = e.clientY - rect.top;
      }
    });

    simCanvas.addEventListener('mouseup', () => {
      if(isDragging) {
        isDragging = false;
        isFlying = true;
        vx = (anchorX - birdX) * 0.25;
        vy = (anchorY - birdY) * 0.25;
        playCyberSound();
      }
    });

    function renderSim() {
      sCtx.clearRect(0, 0, simCanvas.width, simCanvas.height);

      // Slingshot frame
      sCtx.strokeStyle = '#00f0ff';
      sCtx.lineWidth = 4;
      sCtx.beginPath();
      sCtx.moveTo(anchorX, anchorY + 60);
      sCtx.lineTo(anchorX, anchorY);
      sCtx.stroke();

      // Slingshot rubber band
      if(isDragging || isFlying) {
        sCtx.strokeStyle = '#ff007f';
        sCtx.lineWidth = 3;
        sCtx.beginPath();
        sCtx.moveTo(anchorX - 15, anchorY);
        sCtx.lineTo(birdX, birdY);
        sCtx.lineTo(anchorX + 15, anchorY);
        sCtx.stroke();
      }

      // Physics loop
      if(isFlying) {
        birdX += vx;
        birdY += vy;
        vy += 0.4; // gravity

        if(birdY > 260 || birdX > simCanvas.width) {
          isFlying = false;
          birdX = anchorX;
          birdY = anchorY;
        }
      }

      // Target TNT block
      sCtx.fillStyle = '#ff007f';
      sCtx.fillRect(650, 180, 50, 80);
      sCtx.fillStyle = '#fff';
      sCtx.font = 'bold 12px Orbitron';
      sCtx.fillText('TNT', 662, 225);

      // Angry Bird (Red Circle with beak)
      sCtx.fillStyle = '#ff3366';
      sCtx.beginPath();
      sCtx.arc(birdX, birdY, 18, 0, Math.PI * 2);
      sCtx.fill();
      sCtx.strokeStyle = '#fff';
      sCtx.lineWidth = 2;
      sCtx.stroke();

      // Beak
      sCtx.fillStyle = '#facc15';
      sCtx.beginPath();
      sCtx.moveTo(birdX + 10, birdY - 5);
      sCtx.lineTo(birdX + 22, birdY);
      sCtx.lineTo(birdX + 10, birdY + 5);
      sCtx.fill();

      requestAnimationFrame(renderSim);
    }
    renderSim();
  </script>
</body>
</html>


━━━━━━━━━━━━━━━━━━━━

CURRENTLY LEARNING

WebXR
Advanced Unity
AI + XR
3D Development

━━━━━━━━━━━━━━━━━━━━

CONNECT
www.linkedin.com/in/amar-gore-704205320 • https://amar-gore-prortfolio.vercel.app/ • goreamar5077@gmail.com
