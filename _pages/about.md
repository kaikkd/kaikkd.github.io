---
layout: default
permalink: /
title: Home
description: "Jun Wang's academic homepage"

announcements:
  enabled: false

selected_papers: false
social: false
---

<style>
html { scroll-behavior: smooth; }

body {
  background: var(--global-bg-color, #fff);
}

.container.mt-5 {
  max-width: 1180px !important;
  padding-left: 22px !important;
  padding-right: 22px !important;
}

.navbar .container {
  max-width: 1180px;
}

.hp {
  display: grid;
  grid-template-columns: 250px minmax(0, 1fr) 164px;
  gap: 34px;
  align-items: start;
}

.hp-side {
  position: sticky;
  top: 86px;
  padding-top: 4px;
  text-align: center;
}

.hp-side .avatar {
  width: 168px;
  height: 168px;
  border-radius: 50%;
  object-fit: cover;
  object-position: center 22%;
  display: block;
  margin: 0 auto 14px;
  border: 1px solid var(--global-divider-color, #dedede);
}

.hp-side .name {
  margin: 0;
  font-size: 1.18rem;
  font-weight: 700;
  line-height: 1.25;
}

.hp-side .name-cn {
  margin: 2px 0 10px;
  font-size: 0.86rem;
  color: var(--global-text-color-light, #777);
}

.hp-side .role {
  margin: 0 0 12px;
  font-size: 0.82rem;
  line-height: 1.45;
  color: var(--global-text-color-light, #666);
}

.hp-side .keywords {
  display: flex;
  flex-wrap: wrap;
  gap: 5px;
  justify-content: center;
  margin-bottom: 13px;
}

.hp-side .keywords span {
  padding: 2px 8px;
  border-radius: 12px;
  background: var(--global-code-bg-color, #f2f2f2);
  font-size: 0.68rem;
  color: var(--global-text-color, #333);
}

.hp-side .meta {
  margin: 0 0 14px;
  font-size: 0.78rem;
  color: var(--global-text-color-light, #777);
}

.hp-side .links {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 7px;
}

.hp-side .links a {
  display: inline-flex;
  align-items: center;
  gap: 7px;
  color: var(--global-text-color, #333);
  font-size: 0.79rem;
  opacity: 0.72;
  text-decoration: none;
}

.hp-side .links a:hover {
  color: var(--global-theme-color, #2698ba);
  opacity: 1;
}

.hp-side .links i {
  width: 15px;
  text-align: center;
}

.hp-main {
  min-width: 0;
  line-height: 1.68;
}

.hp-main section {
  margin-bottom: 2.1rem;
}

.hp-main h2 {
  margin: 0 0 0.72rem;
  padding-bottom: 0.35rem;
  border-bottom: 1px solid var(--global-divider-color, #e6e6e6);
  font-size: 1.23rem;
  font-weight: 600;
}

.hp-main h3 {
  margin: 1.1rem 0 0.35rem;
  font-size: 0.98rem;
  font-weight: 600;
}

.hp-main p,
.hp-main li {
  font-size: 0.94rem;
}

.hp-main p {
  margin: 0 0 0.8rem;
}

.hp-main ul {
  margin: 0.35rem 0 0;
  padding-left: 1.15rem;
}

.news-list {
  list-style: none;
  padding: 0;
  margin: 0;
}

.news-list li {
  margin-bottom: 0.32rem;
  line-height: 1.6;
}

.news-list strong {
  font-weight: 600;
  color: var(--global-theme-color, #2698ba);
}

.tl {
  list-style: none;
  padding: 0;
  margin: 0;
}

.tl > li {
  display: grid;
  grid-template-columns: 92px minmax(0, 1fr);
  column-gap: 18px;
  margin-bottom: 1rem;
}

.tl .date {
  font-size: 0.82rem;
  color: var(--global-text-color-light, #777);
  line-height: 1.5;
}

.tl .title {
  font-weight: 600;
  line-height: 1.45;
}

.tl .sub {
  margin-top: 1px;
  font-size: 0.88rem;
  color: var(--global-text-color-light, #666);
}

.tl ul {
  margin-top: 0.26rem;
  padding-left: 1rem;
}

.paper,
.project {
  margin-bottom: 1rem;
}

.paper .p-title,
.project .p-title {
  font-weight: 600;
  line-height: 1.45;
}

.paper .p-authors,
.project .p-desc {
  margin-top: 2px;
  font-size: 0.86rem;
  color: var(--global-text-color-light, #666);
  line-height: 1.5;
}

.paper .p-meta,
.project .p-meta {
  margin-top: 2px;
  display: flex;
  flex-wrap: wrap;
  gap: 7px;
  align-items: center;
  font-size: 0.76rem;
}

.badge-soft {
  display: inline-block;
  padding: 1px 7px;
  border-radius: 4px;
  background: var(--global-code-bg-color, #f2f2f2);
  color: var(--global-text-color, #333);
  font-weight: 600;
}

.link-bracket a {
  margin-right: 2px;
}

.link-bracket a::before { content: "["; }
.link-bracket a::after { content: "]"; }

.award-list {
  padding-left: 1.1rem;
  margin: 0;
}

.award-list li {
  margin-bottom: 0.35rem;
}

.hp-toc {
  position: sticky;
  top: 88px;
}

.hp-toc ul {
  list-style: none;
  margin: 0;
  padding: 0 0 0 12px;
  border-left: 2px solid var(--global-divider-color, #e2e2e2);
}

.hp-toc li {
  margin-bottom: 6px;
}

.hp-toc a {
  display: block;
  color: var(--global-text-color, #333);
  font-size: 0.72rem;
  line-height: 1.35;
  opacity: 0.48;
  text-decoration: none;
}

.hp-toc a:hover,
.hp-toc a.active {
  color: var(--global-theme-color, #2698ba);
  opacity: 1;
}

.hp-footer {
  margin-top: 3rem;
  padding-top: 1.2rem;
  border-top: 1px solid var(--global-divider-color, #e6e6e6);
  text-align: center;
  color: var(--global-text-color-light, #777);
  font-size: 0.78rem;
}

@media (max-width: 1060px) {
  .hp {
    grid-template-columns: 235px minmax(0, 1fr);
    gap: 30px;
  }

  .hp-toc { display: none; }
}

@media (max-width: 768px) {
  .container.mt-5 {
    padding-left: 16px !important;
    padding-right: 16px !important;
  }

  .hp {
    grid-template-columns: 1fr;
    gap: 0;
  }

  .hp-side {
    position: static;
    margin-bottom: 1.5rem;
    padding-bottom: 1.4rem;
    border-bottom: 1px solid var(--global-divider-color, #e6e6e6);
  }

  .hp-side .avatar {
    width: 128px;
    height: 128px;
  }

  .hp-side .links {
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    gap: 12px;
  }

  .tl {
    display: block;
  }

  .tl > li {
    display: block;
  }

  .tl .date {
    margin-bottom: 2px;
  }
}
</style>

<div class="hp">
  <aside class="hp-side">
    <img src="{{ 'assets/img/prof_pic.jpg' | relative_url }}" alt="Jun Wang" class="avatar" />
    <h1 class="name">Jun Wang</h1>
    <p class="name-cn">王骏</p>
    <p class="role">
      UC San Diego CSE CS75 Project<br />
      Computer Science and AI Systems
    </p>
    <div class="keywords">
      <span>Agent Systems</span>
      <span>LLM Evaluation</span>
      <span>VLM Benchmark</span>
      <span>RAG</span>
    </div>
    <p class="meta"><i class="fa-solid fa-location-dot"></i> Beijing, China</p>
    <div class="links">
      <a href="mailto:wangjun170417@163.com"><i class="fa-solid fa-envelope"></i><span>Email</span></a>
      <a href="https://github.com/kaikkd" target="_blank"><i class="fa-brands fa-github"></i><span>GitHub</span></a>
      <a href="{{ '/cv/' | relative_url }}"><i class="fa-solid fa-file-lines"></i><span>CV</span></a>
      <a href="{{ '/publications/' | relative_url }}"><i class="fa-solid fa-book-open"></i><span>Publications</span></a>
    </div>
  </aside>

  <main class="hp-main">
    <section id="about-me">
      <h2>About Me</h2>
      <p>
        I build practical AI systems for coding, evaluation, and multimodal understanding.
        My current work focuses on making agent workflows stable, measurable, and useful in real engineering environments.
      </p>
      <p>
        I am currently participating in the <strong>UC San Diego CSE CS75 project</strong>.
        I received my B.Eng. in Computer Science and Technology from Beijing Forestry University.
      </p>
      <h3>Research Interests</h3>
      <ul>
        <li><strong>Agent systems</strong>: coding agents, tool-use workflows, multi-turn state management, and self-correction.</li>
        <li><strong>Model evaluation</strong>: function-calling benchmarks, sandboxed execution, factuality checks, and LLM/VLM metrics.</li>
        <li><strong>Applied AI</strong>: RAG systems, multimodal recognition, remote sensing, and domain adaptation.</li>
      </ul>
    </section>

    <section id="news">
      <h2>News</h2>
      <ul class="news-list">
        <li><strong>2026.03</strong> Started the UC San Diego CSE CS75 project and focused on practical system implementation for AI agents.</li>
        <li><strong>2025.12</strong> Built a ReAct-style coding agent with planning, tool-use, and critic-based correction.</li>
        <li><strong>2025.08</strong> Started my internship at ByteDance, working on agent development and automated evaluation.</li>
        <li><strong>2025</strong> Published FCDNet in IEEE Transactions on Geoscience and Remote Sensing.</li>
      </ul>
    </section>

    <section id="education">
      <h2>Education</h2>
      <ul class="tl">
        <li>
          <div class="date">2026 - Present</div>
          <div>
            <div class="title">UC San Diego, CSE CS75 Project</div>
            <div class="sub">Project-based advanced computer science implementation practice.</div>
          </div>
        </li>
        <li>
          <div class="date">2022 - 2026</div>
          <div>
            <div class="title">Beijing Forestry University</div>
            <div class="sub">B.Eng. in Computer Science and Technology.</div>
          </div>
        </li>
      </ul>
    </section>

    <section id="experience">
      <h2>Research & Engineering Experience</h2>
      <ul class="tl">
        <li>
          <div class="date">2025.08 - Present</div>
          <div>
            <div class="title">ByteDance, Agent Development / Evaluation</div>
            <div class="sub">LLM agent evaluation, coding agent workflows, and multimodal metrics.</div>
            <ul>
              <li>Integrated BFCLv4 into internal evaluation workflows for large-scale function-calling assessment.</li>
              <li>Built Docker-based sandbox execution to improve isolation and reliability for agent evaluation.</li>
              <li>Designed multi-turn agent interaction and session state management for long-context coding tasks.</li>
              <li>Implemented LLM/VLM metrics including factuality, BON, WON, and benchmark pipeline alignment.</li>
            </ul>
          </div>
        </li>
        <li>
          <div class="date">2024.10 - 2024.12</div>
          <div>
            <div class="title">LargeV Instrument, AI Algorithm Intern</div>
            <div class="sub">Computer vision for oral scan data and model-assisted annotation.</div>
            <ul>
              <li>Compared and tuned YOLO models for oral scan image segmentation and classification.</li>
              <li>Integrated model pre-detection into annotation workflows to reduce manual labeling effort.</li>
            </ul>
          </div>
        </li>
      </ul>
    </section>

    <section id="projects">
      <h2>Selected Projects</h2>
      <div class="project">
        <div class="p-title">Code Agent Bot: Autonomous Coding Agent based on ReAct</div>
        <div class="p-desc">Designed a planner-analyzer-critic workflow that can react to terminal feedback, call tools, rewrite code, and verify results.</div>
        <div class="p-meta"><span class="badge-soft">Agent</span><span class="badge-soft">ReAct</span><span class="badge-soft">MCP</span></div>
      </div>
      <div class="project">
        <div class="p-title">Medical RAG Question Answering System</div>
        <div class="p-desc">Built an end-to-end RAG stack using FAISS retrieval, BGE reranking, multi-model inference, and automatic quality evaluation.</div>
        <div class="p-meta"><span class="badge-soft">RAG</span><span class="badge-soft">LangChain</span><span class="badge-soft">Streamlit</span></div>
      </div>
      <div class="project">
        <div class="p-title">Forestry Knowledge QA with LoRA Fine-tuning</div>
        <div class="p-desc">Fine-tuned a Qwen-based model with LoRA and built a streaming Gradio interface for domain-specific forestry QA.</div>
        <div class="p-meta"><span class="badge-soft">LoRA</span><span class="badge-soft">Qwen</span><span class="badge-soft">Gradio</span></div>
      </div>
      <div class="project">
        <div class="p-title">Multimodal Waterbird Recognition System</div>
        <div class="p-desc">Developed an image-audio recognition pipeline and deployed backend APIs for waterbird identification.</div>
        <div class="p-meta"><span class="badge-soft">CV</span><span class="badge-soft">Audio</span><span class="badge-soft">Flask</span></div>
      </div>
    </section>

    <section id="publications">
      <h2>Selected Publications</h2>
      <div class="paper">
        <div class="p-title">FCDNet: A Multi-Scale Attention Network for Forest Change Detection Using Dual-Temporal Very-High-Resolution Remote Sensing Images</div>
        <div class="p-authors"><strong>Jun Wang</strong>, Zongqi Yao, Long Chen, Ruijing Yang, Xiaoli Zha</div>
        <div class="p-meta"><span class="badge-soft">IEEE TGRS 2025</span><span class="link-bracket"><a href="https://doi.org/10.1109/TGRS.2025.3631750" target="_blank">paper</a></span></div>
      </div>
      <div class="paper">
        <div class="p-title">GCAO: Group-driven Clustering via Gravitational Attraction and Optimization</div>
        <div class="p-authors">Qi Li, <strong>Jun Wang</strong></div>
        <div class="p-meta"><span class="badge-soft">arXiv 2025</span><span class="link-bracket"><a href="https://doi.org/10.48550/arXiv.2510.23259" target="_blank">paper</a></span></div>
      </div>
      <div class="paper">
        <div class="p-title">ForestFoodKG: A Structured Dataset and Knowledge Graph for Forest Food Taxonomy and Nutrition</div>
        <div class="p-authors">Rongen Yan, Zhidan Chen, Shengqi Zhou, Guoxing Niu, Yan Li, Zehui Liu, <strong>Jun Wang</strong>, et al.</div>
        <div class="p-meta"><span class="badge-soft">Foods 2025</span><span class="link-bracket"><a href="https://doi.org/10.3390/foods14244186" target="_blank">paper</a></span></div>
      </div>
    </section>

    <section id="honors">
      <h2>Honors & Awards</h2>
      <ul class="award-list">
        <li>National First Prize, Multimedia Application Competition.</li>
        <li>ACM programming competition silver award, Beijing Forestry University.</li>
        <li>TOEFL 103.</li>
      </ul>
    </section>

    <section id="services">
      <h2>Skills</h2>
      <ul class="award-list">
        <li><strong>Programming</strong>: Python, PyTorch, Docker, Git, MySQL, Java, C.</li>
        <li><strong>AI systems</strong>: LangChain, RAG, function calling, evaluation pipelines, model benchmarking.</li>
        <li><strong>Interfaces</strong>: Streamlit, Gradio, Flask, web-based agent interaction.</li>
      </ul>
    </section>

    <footer class="hp-footer">Last updated: May 2026</footer>
  </main>

  <nav class="hp-toc" aria-label="Table of contents">
    <ul>
      <li><a href="#about-me">About Me</a></li>
      <li><a href="#news">News</a></li>
      <li><a href="#education">Education</a></li>
      <li><a href="#experience">Experience</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#publications">Publications</a></li>
      <li><a href="#honors">Honors</a></li>
      <li><a href="#services">Skills</a></li>
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
    var y = window.scrollY + 120;
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
