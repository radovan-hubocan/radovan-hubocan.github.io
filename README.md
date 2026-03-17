<!DOCTYPE html>
<html lang="sk">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Radovan Hubočan | Vizitka</title>
  <meta
    name="description"
    content="Minimalistická responzívna online vizitka študenta a OSINT analytika."
  />
  <style>
    :root {
      --bg: #0d1117;
      --card: #161b22;
      --line: rgba(255, 255, 255, 0.08);
      --text: #f3f4f6;
      --muted: #a7b0bd;
      --accent: #58a6ff;
      --accent-soft: #7ee787;
      --shadow: 0 18px 40px rgba(0, 0, 0, 0.35);
      --radius: 20px;
      --max-width: 760px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Inter, "Segoe UI", Roboto, Arial, sans-serif;
      background:
        radial-gradient(circle at top left, rgba(88, 166, 255, 0.12), transparent 28%),
        linear-gradient(180deg, #0d1117 0%, #11161d 100%);
      color: var(--text);
      min-height: 100vh;
      padding: 32px 16px;
      line-height: 1.55;
    }

    .card {
      width: 100%;
      max-width: var(--max-width);
      margin: 0 auto;
      background: var(--card);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      overflow: hidden;
    }

    .top-line {
      height: 6px;
      background: linear-gradient(90deg, var(--accent), var(--accent-soft));
    }

    .content {
      padding: 34px;
    }

    .name {
      font-size: clamp(2rem, 4vw, 2.9rem);
      line-height: 1.1;
      margin-bottom: 8px;
      letter-spacing: -0.04em;
    }

    .role {
      color: var(--muted);
      font-size: 1.15rem;
      margin-bottom: 14px;
      font-style: italic;
    }

    .institutions {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin: 0 0 18px;
    }

    .institution {
      display: inline-flex;
      align-items: center;
      padding: 8px 12px;
      border-radius: 999px;
      font-size: 0.92rem;
      font-weight: 600;
      letter-spacing: 0.01em;
      border: 1px solid transparent;
    }

    .institution.uni {
      color: #9ee6b3;
      background: rgba(126, 231, 135, 0.10);
      border-color: rgba(126, 231, 135, 0.22);
    }

    .institution.nbu {
      color: #8cc8ff;
      background: rgba(88, 166, 255, 0.10);
      border-color: rgba(88, 166, 255, 0.22);
    }

    .org {
      margin-bottom: 20px;
    }

    .org strong {
      display: block;
      font-size: 1.06rem;
      margin-bottom: 4px;
    }

    .org span {
      color: var(--accent-soft);
      font-weight: 600;
    }

    .divider {
      height: 1px;
      background: var(--line);
      margin: 22px 0;
    }

    .section-title {
      font-size: 1.05rem;
      margin-bottom: 10px;
      color: var(--accent);
    }

    .text {
      color: var(--text);
      font-size: 1rem;
    }

    .muted {
      color: var(--muted);
    }

    .list {
      display: grid;
      gap: 10px;
    }

    .item strong {
      color: var(--text);
    }

    .item a {
      color: var(--accent-soft);
      text-decoration: none;
    }

    .item a:hover {
      text-decoration: underline;
    }

    .chips {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      margin-top: 6px;
    }

    .chip {
      padding: 8px 12px;
      border-radius: 999px;
      background: rgba(255, 255, 255, 0.04);
      border: 1px solid var(--line);
      color: var(--muted);
      font-size: 0.95rem;
    }

    .footer {
      margin-top: 8px;
      color: var(--muted);
      font-size: 0.92rem;
    }

    @media (max-width: 768px) {
      body {
        padding: 20px 12px;
      }

      .content {
        padding: 24px;
      }

      .role {
        font-size: 1rem;
      }

      .text,
      .item,
      .chip {
        font-size: 0.96rem;
      }
    }

    @media (max-width: 480px) {
      .content {
        padding: 20px;
      }

      .name {
        font-size: 1.8rem;
      }

      .divider {
        margin: 18px 0;
      }

      .institutions {
        gap: 8px;
        margin: 0 0 16px;
      }

      .institution {
        width: 100%;
        justify-content: flex-start;
        font-size: 0.9rem;
      }
    }
  </style>
</head>
<body>
  <main class="card">
    <div class="top-line"></div>

    <section class="content">
      <h1 class="name">Radovan Hubočan</h1>
      <p class="role">Študent / OSINT analytik</p>

      <div class="institutions">
        <span class="institution uni">Žilinská univerzita v Žiline</span>
        <span class="institution nbu">Národný bezpečnostný úrad</span>
      </div>

      <div class="org">
        <strong>Žilina, Slovensko</strong>
        <span>Web development • Python aplikácie • Kybernetická bezpečnosť</span>
      </div>

      <div class="divider"></div>

      <section>
        <h2 class="section-title">O mne</h2>
        <p class="text">
          Venujem sa vývoju webových a desktopových aplikácií. Zaujímam sa o Python,
          JavaScript, HTML/CSS, návrh systémov, prácu s dátami a tvorbu praktických riešení
          s dôrazom na prehľadnosť, čistý dizajn a použiteľnosť.
        </p>
      </section>

      <div class="divider"></div>

      <section>
        <h2 class="section-title">Oblasti zamerania</h2>
        <div class="chips">
          <span class="chip">Python</span>
          <span class="chip">Threat Intelligence</span>
          <span class="chip">HTML</span>
          <span class="chip">SOCMINT</span>
          <span class="chip">JSON</span>
          <span class="chip">VS Code</span>
          <span class="chip">Kybernetická bezpečnosť</span>
        </div>
      </section>

      <div class="divider"></div>

      <section>
        <h2 class="section-title">Kontakt</h2>
        <div class="list">
          <div class="item"><strong>E-mail:</strong> <a href="mailto:hubocan4@stud.uniza.sk">hubocan4@stud.uniza.sk</a></div>
          <div class="item"><strong>GitHub:</strong> <a href="https://github.com/radovan-hubocan" target="_blank" rel="noopener noreferrer">github.com/radovan-hubocan</a></div>
          <div class="item"><strong>LinkedIn:</strong> <a href="https://linkedin.com/in/tvojprofil" target="_blank" rel="noopener noreferrer">linkedin.com/in/tvojprofil</a></div>
        </div>
      </section>

      <p class="footer">© 2026 Radovan Hubočan</p>
    </section>
  </main>
</body>
</html>
