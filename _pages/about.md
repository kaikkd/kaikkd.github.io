---
layout: default
permalink: /
title: Home
description: "Jun Wang's homepage"

announcements:
  enabled: false

selected_papers: false
social: true
---

<style>
html { scroll-behavior: smooth; }

.container.mt-5 {
  max-width: 1220px !important;
  padding-left: 22px !important;
  padding-right: 22px !important;
}

.hp {
  display: grid;
  grid-template-columns: 270px minmax(0, 1fr) 175px;
  gap: 34px;
  align-items: start;
}

.hp-side {
  position: sticky;
  top: 86px;
  padding: 18px;
  border-radius: 16px;
  border: 1px solid var(--global-divider-color, #e4e4e4);
  background: color-mix(in oklab, var(--global-bg-color, #fff), var(--global-theme-color, #1f7a8c) 4%);
}

.hp-side .avatar {
  width: 140px;
  height: 140px;
  border-radius: 20px;
  object-fit: cover;
  display: block;
  margin: 0 auto 14px;
}

.hp-side .name {
  margin: 0;
  text-align: center;
  font-size: 1.25rem;
  font-weight: 700;
}

.hp-side .name-cn {
  margin: 2px 0 8px;
  text-align: center;
  opacity: 0.65;
  font-size: 0.9rem;
}

.hp-side .tag {
  text-align: center;
  margin: 0 0 10px;
  font-size: 0.82rem;
  opacity: 0.85;
}

.hp-side .pill-wrap {
  display: flex;
  flex-wrap: wrap;
  gap: 6px;
  justify-content: center;
  margin: 8px 0 12px;
}

.hp-side .pill {
  font-size: 0.72rem;
  padding: 3px 9px;
  border-radius: 999px;
  background: var(--global-code-bg-color, #efefef);
}

.hp-side .links {
  margin-top: 10px;
  display: grid;
  gap: 7px;
}

.hp-side .links a {
  text-decoration: none;
  font-size: 0.84rem;
  opacity: 0.8;
}

.hp-side .links a:hover {
  opacity: 1;
}

.hp-main h2 {
  font-size: 1.28rem;
  margin: 0 0 0.8rem;
  border-bottom: 1px solid var(--global-divider-color, #e4e4e4);
  padding-bottom: 0.35rem;
}

.hp-main section {
  margin-bottom: 2rem;
}

.hp-main p,
.hp-main li {
  font-size: 0.95rem;
  line-height: 1.7;
}

.hp-main ul {
  padding-left: 1.2rem;
  margin: 0.4rem 0 0;
}

.item {
  border: 1px solid var(--global-divider-color, #e7e7e7);
  border-radius: 14px;
  padding: 14px 15px;
  margin-bottom: 10px;
  background: color-mix(in oklab, var(--global-bg-color, #fff), var(--global-theme-color, #1f7a8c) 2%);
}

.item .head {
  display: flex;
  justify-content: space-between;
  gap: 8px;
  flex-wrap: wrap;
  margin-bottom: 4px;
}

.item .title {
  font-weight: 620;
}

.item .time {
  font-size: 0.82rem;
  opacity: 0.62;
}

.cards {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 10px;
}

.card {
  border: 1px solid var(--global-divider-color, #e7e7e7);
  border-radius: 14px;
  padding: 13px;
  background: color-mix(in oklab, var(--global-bg-color, #fff), var(--global-theme-color, #1f7a8c) 1.5%);
}

.card h3 {
  font-size: 0.98rem;
  margin: 0 0 4px;
}

.card p {
  margin: 0;
  font-size: 0.88rem;
  opacity: 0.86;
}

.hp-toc {
  position: sticky;
  top: 90px;
}

.hp-toc ul {
  margin: 0;
  padding: 0 0 0 12px;
  list-style: none;
  border-left: 2px solid var(--global-divider-color, #e4e4e4);
}

.hp-toc li { margin-bottom: 7px; }

.hp-toc a {
  text-decoration: none;
  font-size: 0.76rem;
  opacity: 0.6;
}

.hp-toc a:hover,
.hp-toc a.active {
  opacity: 1;
  color: var(--global-theme-color, #1f7a8c);
}

.hp-footer {
  margin-top: 0.8rem;
  font-size: 0.78rem;
  opacity: 0.55;
  text-align: center;
}

@media (max-width: 1060px) {
  .hp { grid-template-columns: 260px minmax(0, 1fr); }
  .hp-toc { display: none; }
}

@media (max-width: 768px) {
  .container.mt-5 {
    padding-left: 15px !important;
    padding-right: 15px !important;
  }

  .hp {
    grid-template-columns: 1fr;
    gap: 14px;
  }

  .hp-side {
    position: static;
  }

  .cards {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="hp">
  <aside class="hp-side">
    <img src="{{ 'assets/img/prof_pic.jpg' | relative_url }}" alt="Jun Wang" class="avatar" />
    <h1 class="name">Jun Wang</h1>
    <p class="name-cn">王骏</p>
    <p class="tag">UC San Diego · CSE CS75 Project</p>
    <div class="pill-wrap">
      <span class="pill">Agent Systems</span>
      <span class="pill">LLM Evaluation</span>
      <span class="pill">VLM Benchmark</span>
      <span class="pill">RAG</span>
    </div>
    <div class="links">
      <a href="mailto:wangjun170417@163.com">Email: wangjun170417@163.com</a>
      <a href="https://github.com/kaikkd" target="_blank">GitHub: kaikkd</a>
      <a href="/cv/">CV Page</a>
    </div>
  </aside>

  <main class="hp-main">
    <section id="about">
      <h2>About</h2>
      <p>
        I build practical AI systems for coding, evaluation, and multimodal understanding.
        My current focus is on making agent workflows stable, measurable, and production-ready.
      </p>
      <p>
        I am currently participating in the <strong>UC San Diego CSE CS75 project</strong>.
        I received my B.Eng. in Computer Science and Technology from Beijing Forestry University.
      </p>
      <ul>
        <li>Current location: Beijing</li>
        <li>Primary stack: Python, PyTorch, Docker, LangChain, Streamlit</li>
        <li>Interests: coding agents, tool-use evaluation, retrieval systems, multimodal benchmarking</li>
      </ul>
    </section>

    <section id="education">
      <h2>Education</h2>
      <div class="item">
        <div class="head">
          <span class="title">University of California, San Diego - CSE CS75 Project</span>
          <span class="time">2026 - Present</span>
        </div>
        <div>Project-based advanced CS training and implementation practice.</div>
      </div>
      <div class="item">
        <div class="head">
          <span class="title">Beijing Forestry University - B.Eng. in Computer Science and Technology</span>
          <span class="time">2022 - 2026</span>
        </div>
        <div>Undergraduate studies in software, machine learning, and applied AI systems.</div>
      </div>
    </section>

    <section id="experience">
      <h2>Experience</h2>
      <div class="item">
        <div class="head">
          <span class="title">ByteDance - Agent Development / Evaluation</span>
          <span class="time">2025.08 - Present</span>
        </div>
        <ul>
          <li>Integrated BFCLv4 into internal evaluation workflows and supported large-scale automated function-calling evaluation.</li>
          <li>Built distributed sandboxed execution with Docker to improve isolation and reliability of agent assessment.</li>
          <li>Designed coding-agent interaction and multi-turn state management for consistent long-context behavior.</li>
          <li>Reproduced multimodal benchmark pipelines and implemented LLM/VLM metrics including factuality, BON, and WON.</li>
        </ul>
      </div>

      <div class="item">
        <div class="head">
          <span class="title">LargeV Instrument - AI Algorithm Intern</span>
          <span class="time">2024.10 - 2024.12</span>
        </div>
        <ul>
          <li>Applied and compared YOLO models on oral scan data and improved private-dataset detection quality.</li>
          <li>Helped integrate model-assisted annotation flow to reduce manual labeling effort.</li>
        </ul>
      </div>
    </section>

    <section id="projects">
      <h2>Selected Projects</h2>
      <div class="cards">
        <article class="card">
          <h3>Code Agent Bot (ReAct + Tool-Use)</h3>
          <p>Planner-analyzer-critic architecture with iterative self-correction for long coding tasks.</p>
        </article>
        <article class="card">
          <h3>Medical RAG QA System</h3>
          <p>FAISS retrieval + reranker + multi-model inference layer with quality evaluation pipeline.</p>
        </article>
        <article class="card">
          <h3>LoRA Forestry QA</h3>
          <p>Domain adaptation on Qwen with lightweight fine-tuning and streaming Gradio interface.</p>
        </article>
        <article class="card">
          <h3>Multimodal Waterbird Recognition</h3>
          <p>Image-audio pipeline using EfficientNet and backend service deployment.</p>
        </article>
      </div>
    </section>

    <section id="publications">
      <h2>Publications</h2>
      <div class="item">
        <div class="title">FCDNet: A Multi-Scale Attention Network for Forest Change Detection</div>
        <div class="time">IEEE TGRS</div>
      </div>
      <div class="item">
        <div class="title">GCAO: Group-driven Clustering via Gravitational Attraction and Optimization</div>
        <div class="time">arXiv / under review</div>
      </div>
      <div class="item">
        <div class="title">ForestFoodKG: A Structured Dataset and Knowledge Graph for Forest Food</div>
        <div class="time">Foods</div>
      </div>
    </section>

    <section id="awards">
      <h2>Awards</h2>
      <ul>
        <li>National First Prize, Multimedia Application Competition</li>
        <li>ACM programming competition silver award (school level)</li>
        <li>TOEFL 103</li>
      </ul>
    </section>

    <footer class="hp-footer">Last updated: May 2026</footer>
  </main>

  <nav class="hp-toc" aria-label="Table of contents">
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#education">Education</a></li>
      <li><a href="#experience">Experience</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#publications">Publications</a></li>
      <li><a href="#awards">Awards</a></li>
    </ul>
  </nav>
</div>

<script>
(function () {
  var toc = document.querySelectorAll('.hp-toc a');
  if (!toc.length) return;

  var sections = [];
  toc.forEach(function (a) {
    var id = a.getAttribute('href').slice(1);
    var el = document.getElementById(id);
    if (el) sections.push({ id: id, el: el, link: a });
  });

  function update() {
    var y = window.scrollY + 130;
    var current = '';
    sections.forEach(function (s) {
      if (s.el.offsetTop <= y) current = s.id;
    });
    sections.forEach(function (s) {
      s.link.classList.toggle('active', s.id === current);
    });
  }

  window.addEventListener('scroll', update, { passive: true });
  update();
})();
</script>
