
<style>
  @import url('https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=DM+Sans:ital,wght@0,300;0,400;0,500;0,600;1,300&display=swap');

  * { box-sizing: border-box; margin: 0; padding: 0; }

  .readme {
    font-family: 'DM Sans', sans-serif;
    background: #0d1117;
    color: #e6edf3;
    max-width: 860px;
    margin: 0 auto;
    padding: 0;
    border-radius: 12px;
    overflow: hidden;
    border: 1px solid #21262d;
  }

  .hero {
    position: relative;
    padding: 52px 48px 40px;
    background: #0d1117;
    border-bottom: 1px solid #21262d;
    overflow: hidden;
  }

  .hero-grid {
    position: absolute;
    inset: 0;
    background-image:
      linear-gradient(rgba(55,138,221,0.04) 1px, transparent 1px),
      linear-gradient(90deg, rgba(55,138,221,0.04) 1px, transparent 1px);
    background-size: 32px 32px;
  }

  .hero-accent {
    position: absolute;
    top: -80px; right: -80px;
    width: 320px; height: 320px;
    border-radius: 50%;
    background: radial-gradient(circle, rgba(55,138,221,0.08) 0%, transparent 70%);
  }

  .hero-content { position: relative; z-index: 1; }

  .badge-row {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
    margin-bottom: 24px;
  }

  .badge {
    display: inline-flex;
    align-items: center;
    gap: 6px;
    padding: 5px 12px;
    border-radius: 20px;
    font-size: 12px;
    font-weight: 500;
    letter-spacing: 0.02em;
    text-decoration: none;
    transition: opacity 0.2s;
    border: 1px solid;
  }

  .badge:hover { opacity: 0.8; }
  .badge-linkedin { background: rgba(0,119,181,0.12); border-color: rgba(0,119,181,0.3); color: #58a6ff; }
  .badge-ig { background: rgba(228,64,95,0.12); border-color: rgba(228,64,95,0.3); color: #ff7b9e; }
  .badge-hr { background: rgba(46,200,102,0.12); border-color: rgba(46,200,102,0.3); color: #56d364; }

  .badge-dot {
    width: 7px; height: 7px;
    border-radius: 50%;
  }
  .badge-linkedin .badge-dot { background: #58a6ff; }
  .badge-ig .badge-dot { background: #ff7b9e; }
  .badge-hr .badge-dot { background: #56d364; }

  .greeting {
    font-family: 'Space Mono', monospace;
    font-size: 13px;
    color: #378add;
    margin-bottom: 10px;
    letter-spacing: 0.05em;
  }

  .hero-name {
    font-family: 'DM Sans', sans-serif;
    font-size: 40px;
    font-weight: 600;
    color: #e6edf3;
    line-height: 1.1;
    margin-bottom: 10px;
    letter-spacing: -0.02em;
  }

  .hero-name span {
    color: #378add;
  }

  .hero-sub {
    font-size: 16px;
    color: #8b949e;
    font-weight: 300;
    margin-bottom: 24px;
    line-height: 1.5;
  }

  .status-row {
    display: flex;
    gap: 20px;
    flex-wrap: wrap;
  }

  .status-item {
    display: flex;
    align-items: center;
    gap: 8px;
    font-size: 13px;
    color: #8b949e;
  }

  .status-icon {
    font-size: 14px;
  }

  .status-item strong {
    color: #e6edf3;
    font-weight: 500;
  }

  .section {
    padding: 32px 48px;
    border-bottom: 1px solid #21262d;
  }

  .section:last-child { border-bottom: none; }

  .section-label {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 24px;
  }

  .section-label-line {
    flex: 1;
    height: 1px;
    background: #21262d;
  }

  .section-label span {
    font-family: 'Space Mono', monospace;
    font-size: 11px;
    color: #378add;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    white-space: nowrap;
  }

  .skills-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 12px;
  }

  .skill-card {
    padding: 16px 18px;
    background: #161b22;
    border: 1px solid #21262d;
    border-radius: 10px;
    transition: border-color 0.2s, background 0.2s;
    cursor: default;
  }

  .skill-card:hover {
    border-color: rgba(55,138,221,0.3);
    background: #1a2030;
  }

  .skill-card-header {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 8px;
  }

  .skill-icon {
    width: 32px; height: 32px;
    border-radius: 7px;
    display: flex; align-items: center; justify-content: center;
    font-size: 17px;
  }

  .skill-name {
    font-size: 14px;
    font-weight: 500;
    color: #e6edf3;
  }

  .skill-desc {
    font-size: 12px;
    color: #8b949e;
    line-height: 1.4;
  }

  .skill-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 5px;
    margin-top: 10px;
  }

  .skill-tag {
    font-size: 10px;
    padding: 2px 8px;
    border-radius: 20px;
    background: #21262d;
    color: #8b949e;
    font-family: 'Space Mono', monospace;
  }

  .projects-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 12px;
  }

  .project-card {
    padding: 20px;
    background: #161b22;
    border: 1px solid #21262d;
    border-radius: 10px;
    transition: border-color 0.2s;
    cursor: default;
  }

  .project-card:hover { border-color: rgba(55,138,221,0.3); }

  .project-header {
    display: flex;
    align-items: flex-start;
    justify-content: space-between;
    margin-bottom: 10px;
  }

  .project-name {
    font-size: 14px;
    font-weight: 500;
    color: #58a6ff;
    margin-bottom: 4px;
  }

  .project-desc {
    font-size: 12px;
    color: #8b949e;
    line-height: 1.5;
  }

  .project-badge {
    font-size: 10px;
    padding: 3px 8px;
    border-radius: 20px;
    font-weight: 500;
    white-space: nowrap;
  }

  .badge-ml { background: rgba(55,138,221,0.15); color: #58a6ff; }
  .badge-api { background: rgba(46,200,102,0.15); color: #56d364; }
  .badge-wip { background: rgba(246,185,59,0.15); color: #e3b341; }

  .stats-row {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 12px;
    margin-bottom: 20px;
  }

  .stat-card {
    background: #161b22;
    border: 1px solid #21262d;
    border-radius: 10px;
    padding: 16px 18px;
    text-align: center;
  }

  .stat-value {
    font-family: 'Space Mono', monospace;
    font-size: 22px;
    color: #378add;
    font-weight: 700;
    margin-bottom: 4px;
  }

  .stat-label {
    font-size: 11px;
    color: #8b949e;
    text-transform: uppercase;
    letter-spacing: 0.06em;
  }

  .streak-wrap {
    background: #161b22;
    border: 1px solid #21262d;
    border-radius: 10px;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 16px;
  }

  .streak-wrap img {
    max-width: 100%;
    border-radius: 4px;
  }

  .footer-note {
    padding: 20px 48px;
    background: #0d1117;
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .footer-mono {
    font-family: 'Space Mono', monospace;
    font-size: 11px;
    color: #484f58;
  }

  .visitor-badge img {
    height: 18px;
    opacity: 0.6;
    filter: invert(0.4);
  }

  @media (max-width: 600px) {
    .skills-grid { grid-template-columns: 1fr; }
    .projects-grid { grid-template-columns: 1fr; }
    .stats-row { grid-template-columns: repeat(2, 1fr); }
    .hero, .section { padding-left: 24px; padding-right: 24px; }
    .footer-note { padding: 16px 24px; }
    .hero-name { font-size: 30px; }
  }
</style>

<div class="readme">

  <div class="hero">
    <div class="hero-grid"></div>
    <div class="hero-accent"></div>
    <div class="hero-content">

      <div class="badge-row">
        <a class="badge badge-linkedin" href="https://www.linkedin.com/in/muhammad-fikri-b3766a2b1/" target="_blank">
          <span class="badge-dot"></span> LinkedIn
        </a>
        <a class="badge badge-ig" href="https://www.instagram.com/sunshinewoon/" target="_blank">
          <span class="badge-dot"></span> Instagram
        </a>
        <a class="badge badge-hr" href="https://www.hackerrank.com/profile/muhammadfikri101" target="_blank">
          <span class="badge-dot"></span> HackerRank
        </a>
      </div>

      <div class="greeting">// hello, world</div>
      <h1 class="hero-name">Muhammad <span>Fikri</span></h1>
      <p class="hero-sub">ML Engineer Intern · Building intelligent systems, one model at a time.</p>

      <div class="status-row">
        <div class="status-item">
          <span class="status-icon">🔭</span>
          Working on <strong>&nbsp;ML Engineering</strong>
        </div>
        <div class="status-item">
          <span class="status-icon">📚</span>
          Learning <strong>&nbsp;AI/ML · MLOps · FastAPI</strong>
        </div>
        <div class="status-item">
          <span class="status-icon">📍</span>
          Based in <strong>&nbsp;Jakarta, Indonesia</strong>
        </div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">
      <span>Tech Stack</span>
      <div class="section-label-line"></div>
    </div>
    <div class="skills-grid">

      <div class="skill-card">
        <div class="skill-card-header">
          <div class="skill-icon" style="background:rgba(55,138,221,0.12);">🐍</div>
          <span class="skill-name">Python</span>
        </div>
        <p class="skill-desc">Primary language for ML pipelines and backend APIs</p>
        <div class="skill-tags">
          <span class="skill-tag">scikit-learn</span>
          <span class="skill-tag">pandas</span>
          <span class="skill-tag">numpy</span>
        </div>
      </div>

      <div class="skill-card">
        <div class="skill-card-header">
          <div class="skill-icon" style="background:rgba(238,76,44,0.12);">🔥</div>
          <span class="skill-name">Deep Learning</span>
        </div>
        <p class="skill-desc">Model training, evaluation, and experimentation</p>
        <div class="skill-tags">
          <span class="skill-tag">PyTorch</span>
          <span class="skill-tag">HuggingFace</span>
          <span class="skill-tag">Jupyter</span>
        </div>
      </div>

      <div class="skill-card">
        <div class="skill-card-header">
          <div class="skill-icon" style="background:rgba(9,175,123,0.12);">⚡</div>
          <span class="skill-name">Backend / API</span>
        </div>
        <p class="skill-desc">REST API development and model serving</p>
        <div class="skill-tags">
          <span class="skill-tag">FastAPI</span>
          <span class="skill-tag">Pydantic</span>
          <span class="skill-tag">REST</span>
        </div>
      </div>

      <div class="skill-card">
        <div class="skill-card-header">
          <div class="skill-icon" style="background:rgba(46,200,102,0.12);">🚀</div>
          <span class="skill-name">MLOps</span>
        </div>
        <p class="skill-desc">Experiment tracking, pipeline packaging & deployment</p>
        <div class="skill-tags">
          <span class="skill-tag">MLflow</span>
          <span class="skill-tag">Docker</span>
          <span class="skill-tag">joblib</span>
        </div>
      </div>

      <div class="skill-card">
        <div class="skill-card-header">
          <div class="skill-icon" style="background:rgba(246,185,59,0.12);">☁️</div>
          <span class="skill-name">Cloud & DevTools</span>
        </div>
        <p class="skill-desc">Cloud deployment and developer tooling</p>
        <div class="skill-tags">
          <span class="skill-tag">GCP</span>
          <span class="skill-tag">Bash</span>
          <span class="skill-tag">VSCode</span>
        </div>
      </div>

      <div class="skill-card">
        <div class="skill-card-header">
          <div class="skill-icon" style="background:rgba(228,64,95,0.12);">🗄️</div>
          <span class="skill-name">Data & Platforms</span>
        </div>
        <p class="skill-desc">Datasets, querying, and ML competition workflows</p>
        <div class="skill-tags">
          <span class="skill-tag">MySQL</span>
          <span class="skill-tag">Kaggle</span>
          <span class="skill-tag">CSV/JSON</span>
        </div>
      </div>

    </div>
  </div>

  <div class="section">
    <div class="section-label">
      <span>Featured Projects</span>
      <div class="section-label-line"></div>
    </div>
    <div class="projects-grid">

      <div class="project-card">
        <div class="project-header">
          <div>
            <div class="project-name">Heart Disease Classifier</div>
          </div>
          <span class="project-badge badge-ml">ML</span>
        </div>
        <p class="project-desc">Classification model on Heart Statlog Cleveland Hungary dataset. Benchmarked Random Forest, XGBoost, LightGBM with overfitting diagnosis and sklearn Pipeline.</p>
        <div class="skill-tags" style="margin-top:12px">
          <span class="skill-tag">scikit-learn</span>
          <span class="skill-tag">XGBoost</span>
          <span class="skill-tag">LightGBM</span>
        </div>
      </div>

      <div class="project-card">
        <div class="project-header">
          <div>
            <div class="project-name">Cancer Detection Model</div>
          </div>
          <span class="project-badge badge-ml">ML</span>
        </div>
        <p class="project-desc">Binary classification for cancer detection. Focused on model generalization, accuracy degradation diagnosis, and synthetic data validation.</p>
        <div class="skill-tags" style="margin-top:12px">
          <span class="skill-tag">Python</span>
          <span class="skill-tag">pandas</span>
          <span class="skill-tag">matplotlib</span>
        </div>
      </div>

      <div class="project-card">
        <div class="project-header">
          <div>
            <div class="project-name">TaskFlow API</div>
          </div>
          <span class="project-badge badge-wip">WIP</span>
        </div>
        <p class="project-desc">RESTful task management API built with FastAPI. Covers Pydantic validation, CRUD patterns, path/query params — production-ready portfolio project.</p>
        <div class="skill-tags" style="margin-top:12px">
          <span class="skill-tag">FastAPI</span>
          <span class="skill-tag">Pydantic</span>
          <span class="skill-tag">Python</span>
        </div>
      </div>

      <div class="project-card">
        <div class="project-header">
          <div>
            <div class="project-name">ML Model Serving</div>
          </div>
          <span class="project-badge badge-api">API</span>
        </div>
        <p class="project-desc">Integrating trained sklearn pipelines with FastAPI for real-time prediction endpoints. Full deployment pipeline with joblib serialization.</p>
        <div class="skill-tags" style="margin-top:12px">
          <span class="skill-tag">FastAPI</span>
          <span class="skill-tag">joblib</span>
          <span class="skill-tag">Docker</span>
        </div>
      </div>

    </div>
  </div>

  <div class="section">
    <div class="section-label">
      <span>GitHub Stats</span>
      <div class="section-label-line"></div>
    </div>

    <div class="stats-row">
      <div class="stat-card">
        <div class="stat-value">ML</div>
        <div class="stat-label">Primary Focus</div>
      </div>
      <div class="stat-card">
        <div class="stat-value">Python</div>
        <div class="stat-label">Top Language</div>
      </div>
      <div class="stat-card">
        <div class="stat-value">4+</div>
        <div class="stat-label">Projects</div>
      </div>
    </div>

    <div class="streak-wrap">
      <img
        src="https://streak-stats.demolab.com?user=fiksdevploper&locale=en&mode=daily&theme=dark&hide_border=true&border_radius=5"
        alt="GitHub Streak Stats"
      />
    </div>
  </div>

  <div class="footer-note">
    <span class="footer-mono">// muhammad-fikri · ml engineer · indonesia</span>
    <span class="footer-mono">
      <img src="https://visitor-badge.laobi.icu/badge?page_id=fiksdevploper.fiksdevploper" alt="visitors" style="height:16px;opacity:0.5;" />
    </span>
  </div>

</div>
