<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Physics & Mathematics Reference</title>

  <!-- KaTeX for beautiful math rendering -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.16.9/dist/katex.min.css"
        integrity="sha384-3UiQGuEI4TTMaFmGIZumfRPtfKQ3trwQE2JgosJxCnGmQpL/lJdjpcHkaaFwHlcI" crossorigin="anonymous">
  <script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.9/dist/katex.min.js"
          integrity="sha384-9tPv11A+glH/on/wEu99NVwDPwkMQ5Fjw03dkx/3vG6u3x7tZp3v43Z5Q0Q3b6" crossorigin="anonymous"></script>
  <script defer src="https://cdn.jsdelivr.net/npm/katex@0.16.9/dist/contrib/auto-render.min.js"
          integrity="sha384-+VBxd3r6XgUJFyhVUXiU6P6N3b+oZJU1XZ4Yc4Z0j+8e5V5w5h6nF4XZj3qJ8" crossorigin="anonymous"></script>

  <style>
    :root {
      --primary: #2c3e50;
      --secondary: #3498db;
      --light: #ecf0f1;
      --gray: #7f8c8d;
    }
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
      line-height: 1.6;
      color: var(--primary);
      background-color: #fafafa;
      padding: 1.5rem;
      max-width: 900px;
      margin: 0 auto;
    }
    header {
      text-align: center;
      margin: 2rem 0;
      padding-bottom: 1.2rem;
      border-bottom: 2px solid var(--secondary);
    }
    h1 {
      font-size: 2.3rem;
      margin-bottom: 0.5rem;
    }
    .tagline {
      font-size: 1.1rem;
      color: var(--gray);
    }
    nav {
      text-align: center;
      margin: 1.5rem 0;
    }
    nav a {
      margin: 0 1rem;
      text-decoration: none;
      color: var(--secondary);
      font-weight: 500;
    }
    nav a:hover {
      text-decoration: underline;
    }
    .section {
      margin: 2.5rem 0;
    }
    h2 {
      color: var(--primary);
      margin: 1.5rem 0 1rem;
      padding-bottom: 0.4rem;
      border-bottom: 2px solid var(--secondary);
    }
    .card {
      background: white;
      padding: 1.5rem;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.05);
      margin-bottom: 1.2rem;
    }
    .law-title {
      font-weight: bold;
      font-size: 1.25rem;
      margin-bottom: 0.6rem;
      color: #2c3e50;
    }
    .law-equation {
      background: #f8fbff;
      padding: 1rem;
      border-radius: 6px;
      text-align: center;
      font-size: 1.3em;
      margin: 0.8rem 0;
      overflow-x: auto;
    }
    .btn {
      display: inline-block;
      background: var(--secondary);
      color: white;
      padding: 0.5rem 1.2rem;
      border-radius: 6px;
      text-decoration: none;
      font-weight: 500;
      margin-top: 0.6rem;
    }
    .btn:hover {
      background: #2980b9;
    }
    .copy-btn {
      background: #95a5a6;
      color: white;
      border: none;
      padding: 0.3rem 0.8rem;
      border-radius: 4px;
      cursor: pointer;
      font-size: 0.85em;
      margin-right: 0.4rem;
    }
    footer {
      text-align: center;
      margin-top: 2.5rem;
      padding-top: 1.2rem;
      border-top: 1px solid #eee;
      color: var(--gray);
      font-size: 0.95rem;
    }
    @media (max-width: 600px) {
      body { padding: 1rem; }
      h1 { font-size: 1.8rem; }
      nav a { display: block; margin: 0.4rem 0; }
    }
  </style>
</head>
<body>

<header>
  <h1>Physics & Mathematics Reference</h1>
  <p class="tagline">A living compendium of fundamental laws — precise, interconnected, and open.</p>
</header>

<nav>
  <a href="#home">Home</a>
  <a href="#about">About</a>
  <a href="#physics">Physics</a>
  <a href="#math">Mathematics</a>
</nav>

<main id="home">
  <section class="section" id="physics">
    <h2>🔬 Core Physics Laws</h2>

    <div class="card">
      <div class="law-title">Newton’s Second Law of Motion</div>
      <div class="law-equation" id="eq1">
        \( \vec{F}_{\text{net}} = m \vec{a} \)
      </div>
      <p>Relates net force on a body to its acceleration in inertial frames. Valid for \( v \ll c \) and constant mass.</p>
      <button class="copy-btn" onclick="copyLaTeX('\\vec{F}_{\\text{net}} = m \\vec{a}')">LaTeX</button>
      <button class="copy-btn" onclick="copyText('F = m a')">Plain</button>
      <a href="#newton" class="btn">Details</a>
    </div>

    <div class="card">
      <div class="law-title">Maxwell’s Equations (Differential Form)</div>
      <div class="law-equation" id="eq2">
        \[
        \begin{aligned}
        \nabla \cdot \mathbf{E} &= \frac{\rho}{\varepsilon_0} \\
        \nabla \cdot \mathbf{B} &= 0 \\
        \nabla \times \mathbf{E} &= -\frac{\partial \mathbf{B}}{\partial t} \\
        \nabla \times \mathbf{B} &= \mu_0 \mathbf{J} + \mu_0 \varepsilon_0 \frac{\partial \mathbf{E}}{\partial t}
        \end{aligned}
        \]
      </div>
      <p>The foundation of classical electromagnetism, light, and all electric/magnetic phenomena.</p>
      <button class="copy-btn" onclick="copyLaTeX('\\nabla \\cdot \\mathbf{E} = \\\\frac{\\rho}{\\varepsilon_0} \\\\quad \\ldots')">LaTeX</button>
      <a href="#maxwell" class="btn">Details</a>
    </div>
  </section>

  <section class="section" id="math">
    <h2>🧮 Foundational Mathematics</h2>

    <div class="card">
      <div class="law-title">Fundamental Theorem of Calculus</div>
      <div class="law-equation">
        \( \int_a^b f'(x)\,dx = f(b) - f(a) \)
      </div>
      <p>Connects differentiation and integration — instantaneous change ↔ accumulated quantity.</p>
      <button class="copy-btn" onclick="copyLaTeX('\\int_a^b f\\'(x)\\,dx = f(b) - f(a)')">LaTeX</button>
      <a href="#ftc" class="btn">Details</a>
    </div>
  </section>

  <section class="section" id="about">
    <h2>👨‍🏫 About This Project</h2>
    <div class="card">
      <p>
        This is a personal academic project to build a clear, rigorous, and interlinked reference for physics and mathematics.
        Every law is presented with:
      </p>
      <ul style="margin: 1rem 0 0 1.5rem;">
        <li>✅ Precise statement and domain of validity</li>
        <li>✅ Physical/mathematical context</li>
        <li>✅ Key derivations or connections (e.g., Noether’s theorem → conservation laws)</li>
        <li>✅ Clean LaTeX for easy reuse</li>
      </ul>
      <p>
        The site is static, fast, and hosted for free via GitHub Pages.
        All content is written in plain HTML — no database, no backend.
      </p>
      <p><em>— Built with clarity and passion for the unity of knowledge.</em></p>
    </div>
  </section>
</main>

<footer>
  <p>© 2025 Physics & Mathematics Reference | Open Source</p>
  <p>Contact: <a href="mailto:youremail@example.com">youremail@example.com</a></p>
</footer>

<script>
  // Render LaTeX on page load
  document.addEventListener("DOMContentLoaded", () => {
    renderMathInElement(document.body, {
      delimiters: [
        {left: "$$", right: "$$", display: true},
        {left: "\\[", right: "\\]", display: true},
        {left: "$", right: "$", display: false},
        {left: "\\(", right: "\\)", display: false}
      ],
      throwOnError: false
    });
  });

  // Copy utilities
  function copyText(text) {
    navigator.clipboard.writeText(text).then(() => {
      alert('✓ Copied: ' + text);
    }).catch(() => alert('Copy failed.'));
  }

  function copyLaTeX(latex) {
    navigator.clipboard.writeText(latex).then(() => {
      alert('✓ LaTeX copied:\n' + latex);
    }).catch(() => alert('Copy failed.'));
  }
</script>

</body>
</html>
