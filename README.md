
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="theme-color" content="#101a18">
  <title>Adapa Mukhesh Raju | Embedded Systems</title>

  <style>
    :root {
      --bg: #101a18;
      --surface: #192923;
      --surface-hover: #203d32;
      --border: #315044;
      --green: #70d6a0;
      --green-light: #a9e7c4;
      --text: #f1f5f3;
      --muted: #b9c9c1;
      --radius: 14px;
    }

    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      background: var(--bg);
      color: var(--text);
      font-family: Inter, -apple-system, BlinkMacSystemFont,
        "Segoe UI", sans-serif;
      line-height: 1.7;
    }

    .container {
      width: min(920px, 92%);
      margin: 40px auto;
    }

    .hero {
      padding: 34px;
      border: 1px solid var(--border);
      border-radius: 20px;
      background: linear-gradient(135deg, #192923, #101a18);
    }

    .eyebrow {
      color: var(--green);
      font-size: 12px;
      font-weight: 700;
      letter-spacing: 2px;
      text-transform: uppercase;
    }

    h1 {
      margin: 10px 0 2px;
      font-size: clamp(28px, 5vw, 42px);
      line-height: 1.2;
      letter-spacing: -1px;
    }

    .role {
      margin: 12px 0;
      color: var(--green);
      font-size: 18px;
      font-weight: 600;
    }

    .intro {
      max-width: 680px;
      color: var(--muted);
    }

    .tags {
      display: flex;
      flex-wrap: wrap;
      gap: 9px;
      margin-top: 22px;
    }

    .tag {
      padding: 5px 12px;
      border: 1px solid #38664f;
      border-radius: 7px;
      background: var(--surface-hover);
      color: var(--green-light);
      font-size: 13px;
      font-weight: 600;
    }

    section {
      margin-top: 36px;
    }

    .section-heading {
      display: flex;
      align-items: center;
      gap: 12px;
      margin-bottom: 17px;
    }

    .section-heading .icon {
      display: grid;
      width: 42px;
      height: 42px;
      flex-shrink: 0;
      place-items: center;
      border-radius: 10px;
      background: var(--surface-hover);
      color: var(--green);
      font-size: 21px;
    }

    h2 {
      margin: 0;
      font-size: 23px;
    }

    h3 {
      margin: 0;
      font-size: 17px;
    }

    .section-description {
      margin: 3px 0 0;
      color: var(--muted);
      font-size: 14px;
    }

    .project-card {
      display: flex;
      gap: 16px;
      padding: 20px;
      border: 1px solid var(--border);
      border-radius: var(--radius);
      background: var(--surface);
      transition: border-color 180ms ease,
                  transform 180ms ease;
    }

    .project-card:hover {
      transform: translateY(-2px);
      border-color: var(--green);
    }

    .project-icon {
      display: grid;
      width: 46px;
      height: 46px;
      flex-shrink: 0;
      place-items: center;
      border-radius: 10px;
      background: var(--surface-hover);
      color: var(--green);
      font-size: 23px;
    }

    .project-content {
      flex: 1;
      min-width: 0;
    }

    .project-content p {
      margin: 5px 0 12px;
      color: var(--muted);
      font-size: 14px;
    }

    .project-meta {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 8px;
    }

    .mini-tag {
      color: var(--green-light);
      font-size: 12px;
    }

    .status {
      margin-left: auto;
      padding: 3px 9px;
      border-radius: 20px;
      background: #244a37;
      color: var(--green-light);
      font-size: 11px;
    }

    .levels {
      display: grid;
      grid-template-columns: repeat(2, minmax(0, 1fr));
      gap: 14px;
    }

    .level-card {
      padding: 20px;
      border: 1px solid var(--border);
      border-radius: var(--radius);
      background: var(--surface);
    }

    .level-number {
      color: var(--green);
      font-size: 12px;
      font-weight: 700;
      letter-spacing: 1px;
    }

    .level-card h3 {
      margin: 8px 0;
    }

    .level-card p {
      margin: 0;
      color: var(--muted);
      font-size: 13px;
    }

    .level-card ul {
      margin: 14px 0 0;
      padding-left: 19px;
      color: var(--muted);
      font-size: 13px;
    }

    .level-card li {
      margin: 5px 0;
    }

    .tool-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .tool {
      padding: 9px 14px;
      border: 1px solid var(--border);
      border-radius: 9px;
      background: var(--surface);
      color: var(--green-light);
      font-size: 13px;
      font-weight: 600;
    }

    .index-card {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 16px;
      padding: 22px;
      border: 1px solid #38664f;
      border-radius: var(--radius);
      background: linear-gradient(120deg, #203d32, #192923);
    }

    .index-card p {
      margin: 5px 0 0;
      color: var(--muted);
      font-size: 14px;
    }

    .index-label {
      color: var(--green-light);
      font-size: 13px;
      white-space: nowrap;
    }

    a {
      color: var(--green);
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    footer {
      margin-top: 40px;
      padding: 24px 0;
      border-top: 1px solid var(--border);
      color: var(--muted);
      font-size: 13px;
    }

    .footer-links {
      display: flex;
      flex-wrap: wrap;
      gap: 18px;
      margin-top: 8px;
    }

    @media (max-width: 600px) {
      .container {
        margin: 18px auto;
      }

      .hero {
        padding: 24px 20px;
      }

      .levels {
        grid-template-columns: 1fr;
      }

      .index-card {
        align-items: flex-start;
        flex-direction: column;
      }

      .status {
        margin-left: 0;
      }
    }

    @media (prefers-reduced-motion: reduce) {
      *,
      *::before,
      *::after {
        transition: none !important;
        scroll-behavior: auto !important;
      }
    }
  </style>
</head>

<body>
  <main class="container">

    <header class="hero">
      <div class="eyebrow">Embedded Systems / Firmware</div>

      <h1>Adapa Mukhesh Raju</h1>

      <div class="role">
        Embedded Systems | Firmware Development
      </div>

      <p class="intro">
        Learning embedded systems by building and testing projects.
        I'm an Electronics and Communication Engineering undergraduate
        working toward a career in embedded firmware development.
        I enjoy understanding how software interacts with hardware
        and turning what I learn into working projects.
      </p>

      <div class="tags">
        <span class="tag">Firmware</span>
        <span class="tag">STM32</span>
        <span class="tag">IoT</span>
      </div>
    </header>

    <section>
      <div class="section-heading">
        <div class="icon" aria-hidden="true">⌘</div>
        <div>
          <h2>Currently Building</h2>
          <p class="section-description">
            My current hands-on work
          </p>
        </div>
      </div>

      <article class="project-card">
        <div class="project-icon" aria-hidden="true">💡</div>
        <div class="project-content">
          <h3>STM32 LED Controller</h3>
          <p>
            Exploring GPIO control, LED states and timing using
            STM32 HAL in PICSimLab.
          </p>
          <div class="project-meta">
            <span class="mini-tag">STM32</span>
            <span class="mini-tag">GPIO</span>
            <span class="mini-tag">C</span>
            <span class="status">In progress</span>
          </div>
        </div>
      </article>
    </section>

    <section>
      <div class="section-heading">
        <div class="icon" aria-hidden="true">▦</div>
        <div>
          <h2>My Projects</h2>
          <p class="section-description">
            From fundamentals to complete embedded systems
          </p>
        </div>
      </div>

      <div class="levels">

        <article class="level-card">
          <div class="level-number">LEVEL 01</div>
          <h3>Basic Projects</h3>
          <p>Building strong microcontroller fundamentals.</p>
          <ul>
            <li>LED Blink</li>
            <li>RGB LED Controller</li>
            <li>Button-Controlled LED</li>
          </ul>
        </article>

        <article class="level-card">
          <div class="level-number">LEVEL 02</div>
          <h3>Intermediate Projects</h3>
          <p>Working with peripherals and structured firmware.</p>
          <ul>
            <li>PWM Signal Generator</li>
            <li>UART Command Interface</li>
            <li>Sensor Monitor</li>
          </ul>
        </article>

        <article class="level-card">
          <div class="level-number">LEVEL 03</div>
          <h3>Original Projects</h3>
          <p>Developing solutions through my own ideas.</p>
          <ul>
            <li>Smart Temperature Monitor</li>
            <li>Smart Water Tank Controller</li>
            <li>ColdGuard</li>
          </ul>
        </article>

        <article class="level-card">
          <div class="level-number">LEVEL 04</div>
          <h3>Advanced Systems</h3>
          <p>Exploring system-level firmware concepts.</p>
          <ul>
            <li>Real-time systems and RTOS</li>
            <li>Fault handling and watchdogs</li>
            <li>Robotics and drone firmware</li>
          </ul>
        </article>

      </div>
    </section>

    <section>
      <div class="section-heading">
        <div class="icon" aria-hidden="true">⚙</div>
        <div>
          <h2>Tools & Technologies</h2>
          <p class="section-description">
            Tools I use in my development workflow
          </p>
        </div>
      </div>

      <div class="tool-grid">
        <span class="tool">C</span>
        <span class="tool">STM32CubeIDE</span>
        <span class="tool">PICSimLab</span>
        <span class="tool">Git</span>
        <span class="tool">GitHub</span>
      </div>
    </section>

    <section>
      <div class="index-card">
        <div>
          <h3>Embedded Projects Index</h3>
          <p>
            A categorized directory of my firmware projects,
            documentation and testing notes.
          </p>
        </div>
        <span class="index-label">Coming soon</span>
      </div>
    </section>

    <footer>
      <strong>Connect</strong>
      <div class="footer-links">
        <a href="YOUR_LINKEDIN_URL">LinkedIn</a>
        <a href="https://github.com/mukhesh-qtech">GitHub</a>
      </div>
    </footer>

  </main>
</body>
</html>
