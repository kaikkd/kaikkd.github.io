---
layout: default
permalink: /
title: ""
excerpt: ""
description: "Jun Wang's academic homepage"
announcements:
  enabled: false
selected_papers: false
social: false
---

<style>
html { scroll-behavior: smooth; }
body {
  margin: 0;
  color: #494e52;
  background: #fff;
  font-family: "Trebuchet MS", Helvetica, sans-serif;
  font-size: 14px;
  line-height: 1.5;
}
body.fixed-top-nav { padding-top: 0 !important; }
body > header,
body > footer { display: none !important; }
.container.mt-5[role="main"] {
  width: 100% !important;
  max-width: none !important;
  margin: 0 !important;
  padding: 0 !important;
}
a { color: #224b8d; }
a:hover { color: #1a3869; }
.dg-masthead {
  position: sticky;
  top: 0;
  z-index: 20;
  background: #fff;
  border-bottom: 1px solid #f2f3f3;
  animation: dgIntro .3s both;
  animation-delay: .15s;
}
.dg-masthead__inner-wrap {
  max-width: 1280px;
  margin-left: auto;
  margin-right: auto;
  padding: .5em;
  font-family: "Trebuchet MS", Helvetica, sans-serif;
}
.dg-masthead__menu ul {
  clear: both;
  margin: 0;
  padding: 0;
  list-style: none;
}
.dg-greedy-nav {
  position: relative;
  min-width: 250px;
  background: #fff;
}
.dg-greedy-nav .visible-links {
  display: flex;
  align-items: center;
  flex-wrap: nowrap;
  overflow: hidden;
}
.dg-greedy-nav a {
  display: block;
  margin: 0 1rem 0 0;
  padding: .5rem 0;
  color: #7a8288;
  text-decoration: none;
  white-space: nowrap;
}
.dg-greedy-nav a:hover { color: #51585d; }
.dg-masthead__menu-item {
  display: block;
  white-space: nowrap;
}
.dg-masthead__menu-item--lg {
  padding-right: 2em;
  font-weight: 700;
}
#dg-main {
  max-width: 1280px;
  margin: 1em auto 0;
  padding-left: 1em;
  padding-right: 1em;
  animation: dgIntro .3s both;
  animation-delay: .35s;
}
#dg-main::after {
  display: block;
  clear: both;
  content: "";
}
.dg-sidebar {
  transform: translate3d(0, 0, 0);
  margin-bottom: 1em;
}
.dg-sidebar::after {
  display: block;
  clear: both;
  content: "";
}
.dg-sidebar h2,
.dg-sidebar h3,
.dg-sidebar h4,
.dg-sidebar h5,
.dg-sidebar h6 {
  margin-bottom: 0;
  font-family: "Trebuchet MS", Helvetica, sans-serif;
}
.dg-sidebar h3,
.dg-sidebar h4 { font-size: 1em; }
.dg-sidebar p,
.dg-sidebar li {
  font-family: "Trebuchet MS", Helvetica, sans-serif;
  font-size: 1em;
  line-height: 1.5;
}
.dg-profile_box {
  display: flex;
  justify-content: flex-start;
  align-content: flex-start;
  align-items: center;
}
.dg-author__avatar-wrap {
  display: table-cell;
  width: 75px;
  vertical-align: top;
}
.dg-author__avatar {
  display: block;
  width: 100%;
  max-width: 175px;
  min-width: 75px;
  border-radius: 50%;
  object-fit: cover;
  object-position: center 22%;
}
.dg-author__content {
  display: table-cell;
  min-width: 120px;
  padding-left: 10px;
  line-height: 1;
  vertical-align: top;
}
.dg-author__name {
  margin: 0;
  font-family: "Trebuchet MS", Helvetica, sans-serif;
  font-size: 1.2em;
}
.dg-author__bio { margin: 0; }
.dg-author__urls-wrapper {
  position: relative;
  z-index: 10;
  display: table-cell;
  margin-left: auto;
  font-family: "Trebuchet MS", Helvetica, sans-serif;
  vertical-align: middle;
}
.dg-author__urls {
  display: none;
  position: absolute;
  right: 0;
  z-index: -1;
  margin-top: 15px;
  padding: 10px;
  list-style: none;
  border: 1px solid #f2f3f3;
  border-radius: 4px;
  background: #fff;
  box-shadow: 0 0 10px rgba(0,0,0,.25);
}
.dg-author__urls::before {
  display: block;
  content: "";
  position: absolute;
  top: -11px;
  left: calc(50% - 10px);
  width: 0;
  border-style: solid;
  border-width: 0 10px 10px;
  border-color: #f2f3f3 transparent;
  z-index: 0;
}
.dg-author__urls::after {
  display: block;
  content: "";
  position: absolute;
  top: -10px;
  left: calc(50% - 10px);
  width: 0;
  border-style: solid;
  border-width: 0 10px 10px;
  border-color: #fff transparent;
  z-index: 1;
}
.dg-author__urls li { white-space: nowrap; }
.dg-author__urls a {
  display: block;
  margin-bottom: 5px;
  padding: 2px 5px 2px 0;
  color: inherit;
  font-size: 1em;
  text-decoration: none;
}
.dg-author__urls a:hover { text-decoration: underline; }
.dg-author__urls .dg-desc {
  white-space: normal;
  margin-bottom: 1em;
}
.dg-author__urls_sm {
  display: block;
  padding: .25em;
  font-size: 1.75em;
}
.dg-author__urls_sm a {
  color: inherit;
  text-decoration: none;
}
.dg-author__urls_sm a:hover { text-decoration: underline; }
.dg-page {
  min-width: 0;
}
.dg-page__inner-wrap,
.dg-page__content {
  width: 100%;
  min-width: 0;
}
.dg-page__content #about-me {
  margin-top: -10em;
}
.dg-page__content #about-me::before {
  content: "";
  display: block;
  position: relative;
  width: 0;
  height: 10em;
  margin-top: -10em;
}
.dg-page__content h1 {
  margin-top: 1em;
  margin-bottom: .5em;
  padding-bottom: .5em;
  border-bottom: 1px solid #f2f3f3;
  color: #494e52;
  font-family: "Trebuchet MS", Helvetica, sans-serif;
  font-size: 1.563em;
  font-weight: 700;
  line-height: 1.2;
}
.dg-page__content h3 {
  margin-top: 1em;
  margin-bottom: .5em;
  color: #494e52;
  font-family: "Trebuchet MS", Helvetica, sans-serif;
  font-size: 1.2em;
  font-weight: 700;
  line-height: 1.2;
}
.dg-page__content p,
.dg-page__content li,
.dg-page__content dl {
  font-size: 1.1em;
}
.dg-page__content p { margin: 0 0 .5em; }
.dg-page__content ul { margin-top: 0; }
.dg-page__content a { text-decoration: underline; }
.dg-page__content a:hover { text-decoration: underline; }
.dg-page__content .small { font-size: 1em; }
.dg-page__content .dg-inline-logo {
  display: inline-block;
  width: 1em;
  height: 1em;
  margin-right: .25em;
  border-radius: 2px;
  background: #f2f3f3;
  color: #224b8d;
  font-size: .9em;
  font-style: normal;
  font-weight: 700;
  line-height: 1em;
  text-align: center;
  vertical-align: -0.08em;
}
.dg-page__content .dg-badge {
  display: inline-block;
  margin-left: .25em;
  padding: .08em .42em;
  border: 1px solid #d9dfe5;
  border-radius: 4px;
  color: #494e52;
  background: #fff;
  font-size: .78em;
  font-weight: 700;
  line-height: 1.35;
  text-decoration: none;
}
.dg-page__content .dg-red { color: #c00000; }
.dg-page__content .dg-muted { color: #7a8288; }
.dg-page__content .dg-paper { margin-bottom: .82em; }
.dg-page__content .dg-service-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: .5em 1.2em;
  padding-left: 1.2em;
}
.dg-footer-note {
  margin: 3em 0 1em;
  padding-top: 1em;
  border-top: 1px solid #f2f3f3;
  color: #7a8288;
  font-size: .9em;
  text-align: center;
}
@media (min-width: 925px) {
  .dg-sidebar {
    position: sticky;
    top: 3.7em;
    float: left;
    width: 15.2542372881%;
    opacity: 1;
    transition: opacity .2s ease-in-out;
  }
  .dg-profile_box { display: block; }
  .dg-author__avatar-wrap {
    display: block;
    width: auto;
    height: auto;
  }
  .dg-author__avatar {
    box-sizing: border-box;
    width: 100%;
    padding: 5px;
    border: 1px solid #f2f3f3;
  }
  .dg-author__content {
    display: block;
    width: 100%;
    padding-right: 0;
    padding-left: 0;
  }
  .dg-author__name {
    margin-top: 10px;
    margin-bottom: 10px;
    font-size: 1.4em;
  }
  .dg-author__bio {
    margin-top: 10px;
    margin-bottom: 20px;
  }
  .dg-author__urls-wrapper { display: block; }
  .dg-author__urls {
    display: block;
    position: relative;
    z-index: auto;
    margin: 0;
    padding: 0;
    border: 0;
    background: transparent;
    box-shadow: none;
  }
  .dg-author__urls::before,
  .dg-author__urls::after { display: none; }
  .dg-author__urls_sm { display: none; }
  .dg-page {
    float: right;
    width: 83.0508474576%;
    padding-left: 4.2372881356%;
  }
}
@media (max-width: 924px) {
  .dg-masthead__inner-wrap { padding: .35em .85em; }
  .dg-greedy-nav .visible-links { overflow-x: auto; }
  .dg-greedy-nav a { margin-right: .85rem; }
  #dg-main { margin-top: .75em; }
  .dg-sidebar { position: relative; }
  .dg-author__urls-wrapper:hover .dg-author__urls,
  .dg-author__urls-wrapper:focus-within .dg-author__urls { display: block; }
}
@media (max-width: 720px) {
  body { font-size: 13px; }
  .dg-profile_box { align-items: flex-start; }
  .dg-author__avatar-wrap { width: 88px; }
  .dg-author__content { padding-top: .2em; }
  .dg-page__content .dg-service-grid { grid-template-columns: 1fr; }
}
@media (max-width: 520px) {
  .dg-masthead__menu-item--lg { padding-right: .75em; }
  .dg-greedy-nav a { margin-right: .75rem; font-size: .92em; }
  #dg-main { padding-left: .75em; padding-right: .75em; }
}
@keyframes dgIntro {
  0% { opacity: 0; transform: translateY(5px); }
  100% { opacity: 1; transform: translateY(0); }
}
</style>

<div class="dg-masthead">
  <div class="dg-masthead__inner-wrap">
    <div class="dg-masthead__menu">
      <nav id="site-nav" class="dg-greedy-nav" aria-label="Primary navigation">
        <ul class="visible-links">
          <li class="dg-masthead__menu-item dg-masthead__menu-item--lg"><a href="#about-me">Homepage</a></li>
          <li class="dg-masthead__menu-item"><a href="#about-me">About me</a></li>
          <li class="dg-masthead__menu-item"><a href="#news">News</a></li>
          <li class="dg-masthead__menu-item"><a href="#education">Education</a></li>
          <li class="dg-masthead__menu-item"><a href="#experiences">Experiences</a></li>
          <li class="dg-masthead__menu-item"><a href="#honors-awards">Honors & Awards</a></li>
          <li class="dg-masthead__menu-item"><a href="#publications">Selected Publications</a></li>
          <li class="dg-masthead__menu-item"><a href="#selected-preprints">Selected Preprints</a></li>
          <li class="dg-masthead__menu-item"><a href="#invited-talks">Invited Talks</a></li>
          <li class="dg-masthead__menu-item"><a href="#academic-services">Academic Services</a></li>
        </ul>
      </nav>
    </div>
  </div>
</div>

<div id="dg-main" role="main">
  <aside class="dg-sidebar sticky">
    <div itemscope itemtype="http://schema.org/Person" class="dg-profile_box">
      <div class="dg-author__avatar-wrap">
        <img src="{{ '/assets/img/prof_pic.jpg' | relative_url }}" class="dg-author__avatar" alt="Jun Wang">
      </div>
      <div class="dg-author__content">
        <h3 class="dg-author__name">Jun Wang</h3>
        <p class="dg-author__bio">UC San Diego CSE CS75 Project</p>
      </div>
      <div class="dg-author__urls-wrapper">
        <ul class="dg-author__urls social-icons">
          <li><div class="dg-desc">AI Agents; Evaluation; Applied Machine Learning</div></li>
          <li><i class="fa-solid fa-fw fa-location-dot" aria-hidden="true"></i> San Diego, CA</li>
          <li><i class="fa-solid fa-fw fa-building-columns" aria-hidden="true"></i> UC San Diego</li>
          <li><a href="mailto:wangjun170417@163.com"><i class="fa-solid fa-fw fa-envelope" aria-hidden="true"></i> Email</a></li>
          <li><a href="https://github.com/kaikkd"><i class="fa-brands fa-fw fa-github" aria-hidden="true"></i> Github</a></li>
          <li><a href="https://scholar.google.com/"><i class="fa-solid fa-fw fa-graduation-cap" aria-hidden="true"></i> Google Scholar</a></li>
        </ul>
        <div class="dg-author__urls_sm">
          <a href="mailto:wangjun170417@163.com" aria-label="Email"><i class="fa-solid fa-envelope" aria-hidden="true"></i></a>
          <a href="https://github.com/kaikkd" aria-label="Github"><i class="fa-brands fa-github" aria-hidden="true"></i></a>
          <a href="https://scholar.google.com/" aria-label="Google Scholar"><i class="fa-solid fa-graduation-cap" aria-hidden="true"></i></a>
        </div>
      </div>
    </div>
  </aside>

  <article class="dg-page" itemscope itemtype="http://schema.org/CreativeWork">
    <div class="dg-page__inner-wrap">
      <section class="dg-page__content" itemprop="text">
        <span class="anchor" id="about-me"></span>
        <h1>About Me</h1>

        <p>I am currently participating in the <a href="https://ucsd.edu/">UC San Diego</a> <strong>CSE CS75 Project</strong>. My work focuses on practical AI systems for coding agents, tool-use workflows, model evaluation, and multimodal understanding.</p>

        <p>I received my B.Eng. in Computer Science and Technology from <a href="https://www.bjfu.edu.cn/">Beijing Forestry University</a>. I have built applied systems across LLM agents, RAG, evaluation pipelines, and multimodal recognition, with engineering experience in Python, PyTorch, Docker, Git, MySQL, Java, and C.</p>

        <h3>Research Interests:</h3>
        <ul>
          <li><strong>General Agent Systems</strong> — Coding agents, tool-use workflows, multi-turn state management, and self-correction.</li>
          <li><strong>Model Evaluation</strong> — Function-calling benchmarks, sandboxed execution, factuality checks, and LLM/VLM metrics.</li>
          <li><strong>Applied AI</strong> — Retrieval-augmented generation, multimodal recognition, remote sensing, and domain adaptation.</li>
        </ul>

        <p>My long-term goal is to build reliable AI systems that can solve real engineering tasks with clear evaluation, controllable tool use, and robust feedback loops.</p>

        <span class="anchor" id="news"></span>
        <h1>🔥 News</h1>
        <ul>
          <li><em>2026.03</em>: Started the <strong>UC San Diego CSE CS75 Project</strong>.</li>
          <li><em>2025.12</em>: Built a ReAct-style coding agent with tool execution, sandbox feedback, and iterative repair.</li>
          <li><em>2025.08</em>: Started internship work at <strong>ByteDance</strong>, focusing on agent development and evaluation.</li>
          <li><em>2025</em>: <strong>FCDNet</strong> was published in <em>IEEE Transactions on Geoscience and Remote Sensing</em>.</li>
        </ul>

        <span class="anchor" id="education"></span>
        <h1>📖 Education</h1>
        <ul>
          <li><span style="font-size: 0.92em;"><strong>2026.03 - Present</strong> | <span class="dg-inline-logo">U</span> <strong>UC San Diego CSE CS75 Project</strong></span><br>University of California San Diego</li>
          <li><span style="font-size: 0.92em;"><strong>2022.09 - 2026.06</strong> | <span class="dg-inline-logo">B</span> <strong>B.Eng. in Computer Science and Technology</strong></span><br>Beijing Forestry University</li>
        </ul>

        <span class="anchor" id="experiences"></span>
        <h1>💻 Research Experience</h1>
        <ul>
          <li><span style="font-size: 0.92em;"><strong>2025.08 - Present</strong> | <strong>ByteDance, Agent Development / Evaluation</strong></span><br><span style="font-size: 0.869em;">- Built and evaluated LLM agent workflows with tool calling, benchmark instrumentation, and execution feedback.<br>- Worked on practical coding-agent behavior, failure analysis, and iterative improvement loops.</span></li>
          <li><span style="font-size: 0.92em;"><strong>2024.10 - 2024.12</strong> | <strong>LargeV Instrument, AI Algorithm Intern</strong></span><br><span style="font-size: 0.869em;">- Developed applied AI components for recognition and analysis workflows.<br>- Improved model inference, data processing, and system integration for production-oriented prototypes.</span></li>
        </ul>

        <span class="anchor" id="honors-awards"></span>
        <h1>🏆 Honors & Awards</h1>
        <h3>Competitions and Recognition</h3>
        <ul>
          <li>National First Prize, Multimedia Application Competition.</li>
          <li>Silver Award, ACM Programming Competition, Beijing Forestry University.</li>
          <li>TOEFL 103.</li>
        </ul>

        <span class="anchor" id="publications"></span>
        <h1>📝 Selected Publications</h1>
        <p><em>Selected peer-reviewed publications and research manuscripts.</em></p>

        <h3>2025</h3>
        <div class="dg-paper">
          <span style="font-size: 0.92em;"><a href="https://doi.org/10.1109/TGRS.2025.3631750"><strong>FCDNet: Frequency Curriculum Domain Adaptation Network for Remote Sensing Semantic Segmentation</strong></a></span><br>
          <span style="font-size: 0.869em;"><strong>Jun Wang</strong> et al.</span><br>
          <span style="font-size: 0.87em; color: #c00000;"><strong>IEEE Transactions on Geoscience and Remote Sensing, 2025</strong></span>
          <a class="dg-badge" href="https://doi.org/10.1109/TGRS.2025.3631750">DOI</a>
        </div>

        <div class="dg-paper">
          <span style="font-size: 0.92em;"><a href="https://doi.org/10.48550/arXiv.2510.23259"><strong>GCAO: A General Coding Agent Optimization Framework</strong></a></span><br>
          <span style="font-size: 0.869em;"><strong>Jun Wang</strong> et al.</span><br>
          <span style="font-size: 0.87em; color: #c00000;"><strong>arXiv, 2025</strong></span>
          <a class="dg-badge" href="https://doi.org/10.48550/arXiv.2510.23259">DOI</a>
        </div>

        <div class="dg-paper">
          <span style="font-size: 0.92em;"><a href="https://doi.org/10.3390/foods14244186"><strong>ForestFoodKG: Knowledge Graph Construction for Forestry Food Domain QA</strong></a></span><br>
          <span style="font-size: 0.869em;"><strong>Jun Wang</strong> et al.</span><br>
          <span style="font-size: 0.87em; color: #c00000;"><strong>Foods, 2025</strong></span>
          <a class="dg-badge" href="https://doi.org/10.3390/foods14244186">DOI</a>
        </div>

        <span class="anchor" id="selected-preprints"></span>
        <h1>📝 Selected Preprints</h1>
        <p><em>Representative projects, preprints, and technical reports.</em></p>
        <ul>
          <li><span style="font-size: 0.92em;"><strong>Code Agent Bot</strong></span><br><span style="font-size: 0.869em;">A ReAct-style coding agent with terminal tools, sandbox execution, multi-turn memory, and automatic repair.</span></li>
          <li><span style="font-size: 0.92em;"><strong>Medical RAG QA System</strong></span><br><span style="font-size: 0.869em;">A retrieval-augmented question-answering system with document indexing, answer grounding, and interface deployment.</span></li>
          <li><span style="font-size: 0.92em;"><strong>Forestry Knowledge QA with LoRA Fine-tuning</strong></span><br><span style="font-size: 0.869em;">A domain QA system combining instruction tuning, knowledge retrieval, and forestry-specific data processing.</span></li>
          <li><span style="font-size: 0.92em;"><strong>Multimodal Waterbird Recognition System</strong></span><br><span style="font-size: 0.869em;">An applied recognition system for multimodal classification and practical deployment.</span></li>
        </ul>

        <span class="anchor" id="invited-talks"></span>
        <h1>🎤 Invited Talks</h1>
        <ul>
          <li><em>Available upon request.</em></li>
        </ul>

        <span class="anchor" id="academic-services"></span>
        <h1>🔍 Academic Services</h1>
        <ul class="dg-service-grid">
          <li><strong>Programming:</strong> Python, PyTorch, Docker, Git, MySQL, Java, C.</li>
          <li><strong>AI Systems:</strong> LangChain, RAG, function calling, evaluation pipelines, benchmarking.</li>
          <li><strong>Interfaces:</strong> Streamlit, Gradio, Flask, web-based agent interaction.</li>
          <li><strong>Research Workflow:</strong> literature review, experiment tracking, error analysis, report writing.</li>
        </ul>

        <div class="dg-footer-note">Last updated: May 2026. Hosted on GitHub Pages.</div>
      </section>
    </div>

  </article>
</div>
