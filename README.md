
<style>
* { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: var(--font-mono, monospace); }
.readme { max-width: 860px; margin: 0 auto; padding: 1.5rem 1rem; color: var(--color-text-primary); }
.hero { text-align: center; padding: 2.5rem 1rem 2rem; border-bottom: 0.5px solid var(--color-border-tertiary); }
.hero-tag { font-size: 11px; letter-spacing: 0.12em; color: var(--color-text-tertiary); text-transform: uppercase; margin-bottom: 1rem; font-family: var(--font-mono); }
.hero h1 { font-size: 22px; font-weight: 500; line-height: 1.4; margin-bottom: 0.75rem; font-family: var(--font-sans); color: var(--color-text-primary); }
.hero-sub { font-size: 13px; color: var(--color-text-secondary); margin-bottom: 1.5rem; font-family: var(--font-sans); }
.badges { display: flex; gap: 8px; justify-content: center; flex-wrap: wrap; }
.badge { display: inline-flex; align-items: center; gap: 5px; font-size: 11px; padding: 4px 10px; border-radius: 99px; border: 0.5px solid var(--color-border-secondary); color: var(--color-text-secondary); font-family: var(--font-sans); text-decoration: none; background: var(--color-background-secondary); }
.badge i { font-size: 13px; }
.section { padding: 1.75rem 0; border-bottom: 0.5px solid var(--color-border-tertiary); }
.section-label { font-size: 11px; letter-spacing: 0.1em; text-transform: uppercase; color: var(--color-text-tertiary); margin-bottom: 1.25rem; font-family: var(--font-mono); }
.whoami { font-size: 14px; line-height: 1.9; color: var(--color-text-secondary); font-family: var(--font-sans); max-width: 640px; }
.whoami span { color: var(--color-text-primary); font-weight: 500; }
.dash-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 10px; }
.dash-card { background: var(--color-background-secondary); border-radius: var(--border-radius-md); padding: 0.875rem 1rem; border: 0.5px solid var(--color-border-tertiary); }
.dash-key { font-size: 11px; color: var(--color-text-tertiary); margin-bottom: 4px; font-family: var(--font-mono); display: flex; align-items: center; gap: 6px; }
.dash-val { font-size: 13px; color: var(--color-text-primary); font-family: var(--font-sans); font-weight: 500; line-height: 1.4; }
.proj-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 12px; }
.proj-card { background: var(--color-background-primary); border: 0.5px solid var(--color-border-tertiary); border-radius: var(--border-radius-lg); padding: 1.25rem; transition: border-color 0.15s; }
.proj-card:hover { border-color: var(--color-border-secondary); }
.proj-label { font-size: 10px; letter-spacing: 0.1em; text-transform: uppercase; color: var(--color-text-tertiary); margin-bottom: 6px; font-family: var(--font-mono); }
.proj-title { font-size: 14px; font-weight: 500; margin-bottom: 8px; font-family: var(--font-sans); color: var(--color-text-primary); }
.proj-desc { font-size: 12px; color: var(--color-text-secondary); line-height: 1.6; margin-bottom: 12px; font-family: var(--font-sans); }
.proj-tags { display: flex; flex-wrap: wrap; gap: 5px; }
.tag { font-size: 10px; padding: 2px 7px; border-radius: 4px; font-family: var(--font-mono); }
.tag-blue { background: #E6F1FB; color: #0C447C; }
.tag-teal { background: #E1F5EE; color: #085041; }
.tag-purple { background: #EEEDFE; color: #3C3489; }
.tag-amber { background: #FAEEDA; color: #633806; }
.tag-coral { background: #FAECE7; color: #712B13; }
.stack-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 10px; }
.stack-group { font-family: var(--font-sans); }
.stack-key { font-size: 11px; font-weight: 500; color: var(--color-text-secondary); margin-bottom: 6px; display: flex; align-items: center; gap: 6px; font-family: var(--font-mono); }
.stack-items { display: flex; flex-wrap: wrap; gap: 4px; }
.stack-item { font-size: 11px; padding: 2px 8px; background: var(--color-background-secondary); border: 0.5px solid var(--color-border-tertiary); border-radius: 4px; color: var(--color-text-secondary); font-family: var(--font-mono); }
.philosophy { display: grid; gap: 10px; }
.principle { display: flex; gap: 12px; align-items: flex-start; font-family: var(--font-sans); font-size: 13px; }
.prin-num { font-size: 11px; font-family: var(--font-mono); color: var(--color-text-tertiary); min-width: 28px; padding-top: 2px; }
.prin-text { color: var(--color-text-secondary); line-height: 1.6; }
.prin-text strong { color: var(--color-text-primary); font-weight: 500; }
.lab-grid { display: grid; gap: 8px; }
.lab-row { display: flex; align-items: center; gap: 12px; padding: 0.75rem 1rem; background: var(--color-background-secondary); border-radius: var(--border-radius-md); border: 0.5px solid var(--color-border-tertiary); }
.lab-status { width: 7px; height: 7px; border-radius: 50%; flex-shrink: 0; }
.status-active { background: #1D9E75; box-shadow: 0 0 0 3px #E1F5EE; }
.status-research { background: #7F77DD; box-shadow: 0 0 0 3px #EEEDFE; }
.status-idea { background: #EF9F27; box-shadow: 0 0 0 3px #FAEEDA; }
.lab-title { font-size: 13px; font-weight: 500; color: var(--color-text-primary); font-family: var(--font-sans); flex: 1; }
.lab-note { font-size: 11px; color: var(--color-text-tertiary); font-family: var(--font-mono); }
.roadmap { position: relative; padding-left: 1.5rem; }
.roadmap-line { position: absolute; left: 6px; top: 12px; bottom: 12px; width: 0.5px; background: var(--color-border-secondary); }
.roadmap-year { position: relative; margin-bottom: 1.5rem; }
.roadmap-dot { width: 13px; height: 13px; border-radius: 50%; border: 2px solid var(--color-border-secondary); background: var(--color-background-primary); position: absolute; left: -1.5rem; top: 3px; }
.roadmap-dot.active { background: #1D9E75; border-color: #1D9E75; }
.roadmap-year-label { font-size: 12px; font-weight: 500; color: var(--color-text-secondary); font-family: var(--font-mono); margin-bottom: 6px; }
.roadmap-items { display: flex; flex-wrap: wrap; gap: 5px; }
.roadmap-item { font-size: 11px; padding: 3px 8px; border-radius: 4px; font-family: var(--font-sans); }
.ri-done { background: #E1F5EE; color: #085041; }
.ri-now { background: #E6F1FB; color: #0C447C; }
.ri-future { background: var(--color-background-secondary); color: var(--color-text-secondary); border: 0.5px solid var(--color-border-tertiary); }
.contact-grid { display: flex; flex-wrap: wrap; gap: 10px; }
.contact-link { display: inline-flex; align-items: center; gap: 8px; padding: 8px 14px; border: 0.5px solid var(--color-border-secondary); border-radius: var(--border-radius-md); font-size: 13px; font-family: var(--font-sans); color: var(--color-text-secondary); text-decoration: none; background: var(--color-background-primary); transition: background 0.12s; }
.contact-link:hover { background: var(--color-background-secondary); }
.contact-link i { font-size: 16px; }
.exp-row { display: flex; align-items: flex-start; gap: 12px; padding: 0.875rem 0; border-bottom: 0.5px solid var(--color-border-tertiary); }
.exp-row:last-child { border-bottom: none; }
.exp-dot { width: 8px; height: 8px; border-radius: 50%; background: var(--color-border-secondary); flex-shrink: 0; margin-top: 5px; }
.exp-dot.current { background: #1D9E75; }
.exp-body { flex: 1; }
.exp-role { font-size: 13px; font-weight: 500; color: var(--color-text-primary); font-family: var(--font-sans); }
.exp-co { font-size: 12px; color: var(--color-text-secondary); font-family: var(--font-sans); }
.exp-date { font-size: 11px; color: var(--color-text-tertiary); font-family: var(--font-mono); white-space: nowrap; }
.copy-btn { font-size: 11px; padding: 3px 8px; border: 0.5px solid var(--color-border-secondary); border-radius: 4px; background: var(--color-background-secondary); color: var(--color-text-secondary); cursor: pointer; font-family: var(--font-mono); float: right; margin-top: -2px; }
.copy-btn:hover { background: var(--color-background-primary); }
</style>

<div class="readme">

<div class="hero">
  <div class="hero-tag">Chennai, India · AI & Data Science · Open to opportunities</div>
  <h1>Building AI systems that transform<br>data into decisions.</h1>
  <div class="hero-sub">ML Engineer · Applied AI · Generative AI · LLM Systems</div>
  <div class="badges">
    <a class="badge" href="https://github.com/AADHITHYA-K"><i class="ti ti-brand-github" aria-hidden="true"></i>AADHITHYA-K</a>
    <a class="badge" href="https://www.linkedin.com/in/aadhithya-k-797690288/"><i class="ti ti-brand-linkedin" aria-hidden="true"></i>LinkedIn</a>
    <a class="badge" href="mailto:aadhithyak123@gmail.com"><i class="ti ti-mail" aria-hidden="true"></i>aadhithyak123@gmail.com</a>
    <a class="badge" href="#"><i class="ti ti-world" aria-hidden="true"></i>Portfolio</a>
  </div>
</div>

<div class="section">
  <div class="section-label">$ whoami</div>
  <div class="whoami">
    AI & Data Science undergraduate building <span>production-grade ML systems</span> and LLM-powered applications.
    Currently interning at <span>Itech India Pvt. Ltd.</span> — owning the full ML loop from data to deployment.
    Obsessed with the gap between AI research and real-world products.
    <span>Not studying AI. Shipping it.</span>
  </div>
</div>

<div class="section">
  <div class="section-label">⌗ dashboard</div>
  <div class="dash-grid">
    <div class="dash-card">
      <div class="dash-key"><i class="ti ti-briefcase" aria-hidden="true" style="font-size:13px"></i>current role</div>
      <div class="dash-val">AI/ML Intern @ Itech India</div>
    </div>
    <div class="dash-card">
      <div class="dash-key"><i class="ti ti-target" aria-hidden="true" style="font-size:13px"></i>targeting</div>
      <div class="dash-val">ML Engineer · Applied AI · GenAI</div>
    </div>
    <div class="dash-card">
      <div class="dash-key"><i class="ti ti-school" aria-hidden="true" style="font-size:13px"></i>education</div>
      <div class="dash-val">B.Tech AI & DS · CGPA 8.99</div>
    </div>
    <div class="dash-card">
      <div class="dash-key"><i class="ti ti-trophy" aria-hidden="true" style="font-size:13px"></i>recognition</div>
      <div class="dash-val">Startup Pitch Fest Finalist · NPTEL Top 1%</div>
    </div>
    <div class="dash-card">
      <div class="dash-key"><i class="ti ti-flask" aria-hidden="true" style="font-size:13px"></i>research</div>
      <div class="dash-val">RAG · Agentic AI · LLM Fine-Tuning</div>
    </div>
    <div class="dash-card">
      <div class="dash-key"><i class="ti ti-code" aria-hidden="true" style="font-size:13px"></i>projects built</div>
      <div class="dash-val">5+ AI · 2 Full-Stack · 1 LLM System</div>
    </div>
  </div>
</div>

<div class="section">
  <div class="section-label">◈ featured ai products</div>
  <div class="proj-grid">
    <div class="proj-card">
      <div class="proj-label">🔍 Private AI Search</div>
      <div class="proj-title">Local LLM Semantic Retrieval</div>
      <div class="proj-desc">Fully local RAG pipeline — drop any document, get context-aware answers. Zero cloud dependency. No data leaves your machine.</div>
      <div class="proj-tags">
        <span class="tag tag-blue">RAG</span>
        <span class="tag tag-blue">Local LLM</span>
        <span class="tag tag-teal">Vector DB</span>
        <span class="tag tag-teal">Docker</span>
        <span class="tag tag-purple">Semantic Search</span>
      </div>
    </div>
    <div class="proj-card">
      <div class="proj-label">🩺 AI Healthcare</div>
      <div class="proj-title">Medical Diagnosis System</div>
      <div class="proj-desc">Symptom-to-diagnosis prediction pairing ML inference with a curated medical knowledge base. Explainable outputs, not black-box.</div>
      <div class="proj-tags">
        <span class="tag tag-coral">NLP</span>
        <span class="tag tag-coral">ML Inference</span>
        <span class="tag tag-amber">Knowledge Base</span>
        <span class="tag tag-amber">XAI</span>
      </div>
    </div>
    <div class="proj-card">
      <div class="proj-label">🌿 AI Agriculture</div>
      <div class="proj-title">Plant Disease Detection</div>
      <div class="proj-desc">Image classification model detecting crop diseases from leaf photos. Actionable diagnosis without expert consultation.</div>
      <div class="proj-tags">
        <span class="tag tag-teal">Computer Vision</span>
        <span class="tag tag-teal">Deep Learning</span>
        <span class="tag tag-blue">Image Classification</span>
      </div>
    </div>
    <div class="proj-card">
      <div class="proj-label">⚡ Dev Productivity</div>
      <div class="proj-title">Resume Builder</div>
      <div class="proj-desc">Web app with guided form UI, live preview, and exportable templates. Built from personal frustration with clunky tools.</div>
      <div class="proj-tags">
        <span class="tag tag-purple">React</span>
        <span class="tag tag-purple">REST API</span>
        <span class="tag tag-blue">Live Preview</span>
      </div>
    </div>
  </div>
</div>

<div class="section">
  <div class="section-label">⚙ technical arsenal</div>
  <div class="stack-grid">
    <div class="stack-group">
      <div class="stack-key"><i class="ti ti-code" aria-hidden="true"></i>languages</div>
      <div class="stack-items">
        <span class="stack-item">Python</span><span class="stack-item">Java</span><span class="stack-item">C</span><span class="stack-item">HTML</span><span class="stack-item">CSS</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-key"><i class="ti ti-brain" aria-hidden="true"></i>ml & ai</div>
      <div class="stack-items">
        <span class="stack-item">RAG</span><span class="stack-item">NLP</span><span class="stack-item">CV</span><span class="stack-item">Scikit-learn</span><span class="stack-item">Embeddings</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-key"><i class="ti ti-sparkles" aria-hidden="true"></i>generative ai</div>
      <div class="stack-items">
        <span class="stack-item">Local LLMs</span><span class="stack-item">LangChain</span><span class="stack-item">Prompt Eng.</span><span class="stack-item">Vector DBs</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-key"><i class="ti ti-server" aria-hidden="true"></i>backend & tools</div>
      <div class="stack-items">
        <span class="stack-item">Docker</span><span class="stack-item">FastAPI</span><span class="stack-item">Git</span><span class="stack-item">MongoDB</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-key"><i class="ti ti-chart-bar" aria-hidden="true"></i>data</div>
      <div class="stack-items">
        <span class="stack-item">Pandas</span><span class="stack-item">NumPy</span><span class="stack-item">Jupyter</span><span class="stack-item">Colab</span>
      </div>
    </div>
    <div class="stack-group">
      <div class="stack-key"><i class="ti ti-layout" aria-hidden="true"></i>frontend</div>
      <div class="stack-items">
        <span class="stack-item">React</span><span class="stack-item">UI/UX</span><span class="stack-item">Figma</span>
      </div>
    </div>
  </div>
</div>

<div class="section">
  <div class="section-label">◎ what i believe</div>
  <div class="philosophy">
    <div class="principle"><span class="prin-num">01 ·</span><span class="prin-text"><strong>Ship fast, iterate faster.</strong> Perfect is the enemy of deployed.</span></div>
    <div class="principle"><span class="prin-num">02 ·</span><span class="prin-text"><strong>AI without a use case is just math.</strong> Build for real problems.</span></div>
    <div class="principle"><span class="prin-num">03 ·</span><span class="prin-text"><strong>Local-first systems beat cloud dependency</strong> for sensitive applications.</span></div>
    <div class="principle"><span class="prin-num">04 ·</span><span class="prin-text"><strong>The best ML model</strong> is the one that actually makes it to production.</span></div>
    <div class="principle"><span class="prin-num">05 ·</span><span class="prin-text"><strong>Research should inform products,</strong> not replace them.</span></div>
  </div>
</div>

<div class="section">
  <div class="section-label">🧪 building in public — lab notebook</div>
  <div class="lab-grid">
    <div class="lab-row">
      <div class="lab-status status-active"></div>
      <div class="lab-title">Advanced RAG with hybrid retrieval + re-ranking</div>
      <div class="lab-note">🔄 active</div>
    </div>
    <div class="lab-row">
      <div class="lab-status status-active"></div>
      <div class="lab-title">Agentic AI with multi-step tool-use pipelines</div>
      <div class="lab-note">🔄 active</div>
    </div>
    <div class="lab-row">
      <div class="lab-status status-research"></div>
      <div class="lab-title">LLM Fine-Tuning via LoRA / QLoRA on domain data</div>
      <div class="lab-note">🔬 researching</div>
    </div>
    <div class="lab-row">
      <div class="lab-status status-research"></div>
      <div class="lab-title">MLOps — model versioning + deployment automation</div>
      <div class="lab-note">🧱 building</div>
    </div>
    <div class="lab-row">
      <div class="lab-status status-idea"></div>
      <div class="lab-title">Generative AI product targeting a real workflow</div>
      <div class="lab-note">💡 ideating</div>
    </div>
  </div>
</div>

<div class="section">
  <div class="section-label">◈ roadmap</div>
  <div class="roadmap">
    <div class="roadmap-line"></div>
    <div class="roadmap-year">
      <div class="roadmap-dot active"></div>
      <div class="roadmap-year-label">2025 — now</div>
      <div class="roadmap-items">
        <span class="roadmap-item ri-done">✓ AI/ML Intern @ Itech India</span>
        <span class="roadmap-item ri-done">✓ Startup Pitch Fest Finalist</span>
        <span class="roadmap-item ri-done">✓ NPTEL Top 1%</span>
        <span class="roadmap-item ri-now">→ 2 open-source AI tools</span>
        <span class="roadmap-item ri-now">→ Master RAG + Agentic AI</span>
      </div>
    </div>
    <div class="roadmap-year">
      <div class="roadmap-dot"></div>
      <div class="roadmap-year-label">2026 — engineer</div>
      <div class="roadmap-items">
        <span class="roadmap-item ri-future">Graduate B.Tech AI & DS</span>
        <span class="roadmap-item ri-future">ML/AI Engineer role</span>
        <span class="roadmap-item ri-future">Contribute to a production LLM system</span>
        <span class="roadmap-item ri-future">Technical writing on AI systems</span>
      </div>
    </div>
    <div class="roadmap-year">
      <div class="roadmap-dot"></div>
      <div class="roadmap-year-label">2027 — researcher</div>
      <div class="roadmap-items">
        <span class="roadmap-item ri-future">AI Research Engineer</span>
        <span class="roadmap-item ri-future">500+ star open-source project</span>
        <span class="roadmap-item ri-future">Agentic AI specialization</span>
      </div>
    </div>
  </div>
</div>

<div class="section">
  <div class="section-label">◉ experience</div>
  <div class="exp-row">
    <div class="exp-dot current"></div>
    <div class="exp-body">
      <div class="exp-role">AI/ML Intern</div>
      <div class="exp-co">Itech India Pvt. Ltd. · Full loop — data cleaning → training → deployment</div>
    </div>
    <div class="exp-date">Feb 2025 – Present</div>
  </div>
  <div class="exp-row">
    <div class="exp-dot"></div>
    <div class="exp-body">
      <div class="exp-role">Machine Learning Intern</div>
      <div class="exp-co">Edunet Foundation · Supervised + unsupervised models from scratch</div>
    </div>
    <div class="exp-date">Feb – Mar 2025</div>
  </div>
  <div class="exp-row">
    <div class="exp-dot"></div>
    <div class="exp-body">
      <div class="exp-role">Full Stack Development Intern</div>
      <div class="exp-co">Big-si-Bucks Innovation · UI design to backend APIs, end-to-end ownership</div>
    </div>
    <div class="exp-date">Nov – Dec 2025</div>
  </div>
</div>

<div class="section" style="border-bottom:none">
  <div class="section-label">◈ contact</div>
  <div class="contact-grid">
    <a class="contact-link" href="https://github.com/AADHITHYA-K"><i class="ti ti-brand-github" aria-hidden="true"></i>GitHub</a>
    <a class="contact-link" href="https://www.linkedin.com/in/aadhithya-k-797690288/"><i class="ti ti-brand-linkedin" aria-hidden="true"></i>LinkedIn</a>
    <a class="contact-link" href="mailto:aadhithyak123@gmail.com"><i class="ti ti-mail" aria-hidden="true"></i>Email</a>
    <a class="contact-link" href="#"><i class="ti ti-world" aria-hidden="true"></i>Portfolio</a>
  </div>
  <div style="margin-top:1.5rem; font-size:12px; color:var(--color-text-tertiary); font-family:var(--font-mono);">Chennai, India · Open to remote and relocation · Not studying AI. Shipping it.</div>
</div>

</div>
