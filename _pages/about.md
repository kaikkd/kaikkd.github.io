---
layout: default
permalink: /
title: Home
description: "{YOUR_NAME}'s academic homepage"

announcements:
  enabled: true
  limit: 15

selected_papers: true
social: true
---

<style>
/* ================================================================
   Homepage — Three-column layout: Sidebar | Content | ToC
   Compatible with al-folio dark mode via CSS custom properties.
   ================================================================ */
html { scroll-behavior: smooth; }

/* Widen the default al-folio container */
.container.mt-5 {
  max-width: 1200px !important;
  padding-left: 20px !important;
  padding-right: 20px !important;
}

/* ── Grid ── */
.hp {
  display: grid;
  grid-template-columns: 250px minmax(0, 1fr) 165px;
  gap: 40px;
  align-items: start;
  font-size: 16px;
}

/* ── LEFT SIDEBAR ── */
.hp-side {
  position: sticky;
  top: 85px;
  text-align: center;
  padding-top: 8px;
}
.hp-side .avatar {
  width: 170px;
  height: 170px;
  border-radius: 50%;
  object-fit: cover;
  display: block;
  margin: 0 auto 14px;
}
.hp-side .name {
  font-size: 1.2rem;
  font-weight: 700;
  margin: 0 0 1px;
  line-height: 1.3;
}
.hp-side .name-cn {
  font-size: 0.88rem;
  opacity: 0.50;
  margin: 0 0 10px;
}
.hp-side .aff {
  font-size: 0.8rem;
  margin: 0 0 12px;
  opacity: 0.75;
  line-height: 1.45;
}
.hp-side .kw {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 5px;
  margin-bottom: 12px;
}
.hp-side .kw span {
  font-size: 0.67rem;
  padding: 2px 9px;
  border-radius: 10px;
  background: var(--global-code-bg-color, #f0f0f0);
  color: var(--global-text-color, #333);
}
.hp-side .loc {
  font-size: 0.78rem;
  opacity: 0.55;
  margin-bottom: 16px;
}
.hp-side .icons {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 6px;
}
.hp-side .icons a {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 0.78rem;
  color: var(--global-text-color, #333);
  text-decoration: none;
  opacity: 0.65;
  transition: opacity 0.15s, color 0.15s;
}
.hp-side .icons a:hover {
  opacity: 1;
  color: var(--global-theme-color, #2698BA);
}
.hp-side .icons a i {
  width: 18px;
  text-align: center;
  font-size: 0.95rem;
}

/* ── MAIN CONTENT ── */
.hp-main {
  min-width: 0;
  line-height: 1.7;
}
.hp-main h2 {
  font-size: 1.3rem;
  font-weight: 600;
  margin: 2.6rem 0 0.8rem;
  padding-bottom: 0.3rem;
  border-bottom: 1px solid var(--global-divider-color, #e8e8e8);
}
.hp-main h2:first-child { margin-top: 0; }
.hp-main h3 {
  font-size: 1rem;
  font-weight: 600;
  margin: 1.3rem 0 0.4rem;
}
.hp-main p {
  margin: 0 0 0.85em;
  font-size: 0.95rem;
}
.hp-main ul, .hp-main ol {
  padding-left: 1.3em;
  font-size: 0.95rem;
}
.hp-main a {
  color: var(--global-theme-color, #2698BA);
  text-decoration: none;
}
.hp-main a:hover { text-decoration: underline; }

/* ── RIGHT TABLE OF CONTENTS ── */
.hp-toc {
  position: sticky;
  top: 85px;
}
.hp-toc ul {
  list-style: none;
  padding: 0 0 0 12px;
  margin: 0;
  border-left: 2px solid var(--global-divider-color, #e0e0e0);
}
.hp-toc li { margin-bottom: 5px; }
.hp-toc a {
  font-size: 0.72rem;
  color: var(--global-text-color, #333);
  opacity: 0.45;
  text-decoration: none;
  display: block;
  line-height: 1.35;
  transition: opacity 0.15s, color 0.15s;
}
.hp-toc a:hover, .hp-toc a.active {
  opacity: 1;
  color: var(--global-theme-color, #2698BA);
}

/* ── NEWS ── */
.news-list {
  list-style: none;
  padding: 0;
  margin: 0;
}
.news-list li {
  margin-bottom: 0.35em;
  font-size: 0.91rem;
  line-height: 1.65;
}
.news-more {
  margin-top: 0.4em;
}
.news-more summary {
  cursor: pointer;
  font-size: 0.84rem;
  color: var(--global-theme-color, #2698BA);
  list-style: none;
  user-select: none;
}
.news-more summary::-webkit-details-marker { display: none; }
.news-more summary::before { content: "▸ "; font-size: 0.7rem; }
.news-more[open] summary::before { content: "▾ "; }

/* ── TIMELINE (Education / Experience) ── */
.tl {
  list-style: none;
  padding: 0;
  margin: 0;
}
.tl > li {
  display: flex;
  gap: 14px;
  margin-bottom: 1em;
  align-items: flex-start;
}
.tl .tl-icon {
  width: 40px;
  height: 40px;
  border-radius: 6px;
  flex-shrink: 0;
  margin-top: 2px;
  background: var(--global-code-bg-color, #f5f5f5);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.05rem;
  overflow: hidden;
}
.tl .tl-icon img {
  width: 32px;
  height: 32px;
  object-fit: contain;
}
.tl .tl-body { flex: 1; min-width: 0; }
.tl .tl-head { font-size: 0.88rem; line-height: 1.5; }
.tl .tl-date { font-size: 0.8rem; opacity: 0.5; }
.tl .tl-title { font-weight: 600; }
.tl .tl-sub { font-size: 0.87rem; opacity: 0.78; line-height: 1.5; }
.tl .tl-details {
  margin: 4px 0 0;
  padding-left: 1em;
  font-size: 0.84rem;
  line-height: 1.6;
  opacity: 0.82;
}

/* ── PAPER ENTRY (preprints & custom sections) ── */
.paper { margin-bottom: 1.2em; }
.paper .p-title {
  font-weight: 600;
  font-size: 0.93rem;
  line-height: 1.4;
}
.paper .p-title a { color: var(--global-theme-color, #2698BA); }
.paper .p-authors {
  font-size: 0.84rem;
  opacity: 0.78;
  margin: 2px 0;
  line-height: 1.5;
}
.paper .p-meta {
  display: flex;
  align-items: center;
  gap: 6px;
  margin-top: 3px;
  flex-wrap: wrap;
}
.paper .p-venue {
  display: inline-block;
  font-size: 0.67rem;
  font-weight: 600;
  padding: 1px 8px;
  border-radius: 3px;
  background: var(--global-code-bg-color, #f3f3f3);
  color: var(--global-text-color, #333);
  white-space: nowrap;
}
.paper .p-links a {
  font-size: 0.75rem;
  margin-right: 3px;
}
.paper .p-links a::before { content: "["; }
.paper .p-links a::after  { content: "]"; }

/* ── AWARDS / SERVICES / TALKS ── */
.awards-list, .talks-list, .services-list {
  padding-left: 1.2em;
  margin: 0;
}
.awards-list li, .talks-list li, .services-list li {
  margin-bottom: 0.3em;
  font-size: 0.91rem;
  line-height: 1.6;
}

/* ── AL-FOLIO selected_papers.liquid OVERRIDE ── */
.publications ol {
  list-style: none !important;
  padding: 0 !important;
}
.publications ol > li {
  margin-bottom: 1.4em !important;
  padding: 0 !important;
  border: none !important;
  box-shadow: none !important;
  background: transparent !important;
}
.publications .row {
  margin: 0 !important;
  padding: 0 !important;
  border: none !important;
  box-shadow: none !important;
  flex-wrap: nowrap !important;
  align-items: flex-start !important;
}
.publications .col.col-sm-2.abbr {
  flex: 0 0 auto !important;
  width: auto !important;
  max-width: none !important;
  padding: 4px 10px 0 0 !important;
}
.publications .col-sm-8,
.publications [class*="col-sm-8"],
.publications [class*="col-sm-10"] {
  flex: 1 !important;
  max-width: 100% !important;
  padding-left: 0 !important;
}
.publications .abbr .badge {
  font-size: 0.67rem !important;
  font-weight: 600 !important;
  padding: 2px 8px !important;
  border-radius: 3px !important;
}
.publications .title {
  font-weight: 600 !important;
  font-size: 0.93rem !important;
}
.publications .author {
  font-size: 0.84rem !important;
  opacity: 0.78;
}
.publications .periodical {
  font-size: 0.82rem !important;
  opacity: 0.55;
}
.publications .links {
  margin-top: 2px;
}
.publications .links .btn {
  border: none !important;
  box-shadow: none !important;
  font-size: 0.73rem !important;
  padding: 0 0.4em !important;
  opacity: 0.6;
}
.publications .links .btn:hover { opacity: 1; }
.publications .badges { margin-top: 3px; }
.publications .z-depth-1 { box-shadow: none !important; }
.publications .preview { display: none !important; }

/* ── FOOTER ── */
.hp-footer {
  text-align: center;
  margin-top: 3rem;
  padding: 1.5rem 0;
  border-top: 1px solid var(--global-divider-color, #e8e8e8);
  font-size: 0.78rem;
  opacity: 0.45;
}

/* ── RESPONSIVE ── */
@media (max-width: 1100px) {
  .hp { grid-template-columns: 235px 1fr; gap: 30px; }
  .hp-toc { display: none; }
}
@media (max-width: 768px) {
  .container.mt-5 { padding-left: 16px !important; padding-right: 16px !important; }
  .hp { grid-template-columns: 1fr; gap: 0; }
  .hp-side {
    position: static;
    padding-bottom: 1.5rem;
    margin-bottom: 1.5rem;
    border-bottom: 1px solid var(--global-divider-color, #e8e8e8);
  }
  .hp-side .avatar { width: 110px; height: 110px; }
  .hp-side .icons { flex-direction: row; flex-wrap: wrap; justify-content: center; gap: 14px; }
  .hp-side .icons a span { display: none; }
}
</style>

<div class="hp">

<!-- ============================================================
     LEFT SIDEBAR
     ============================================================ -->
<aside class="hp-side">
  <img
    src="{{ 'assets/img/prof_pic.jpg' | relative_url }}"
    alt="Profile photo"
    class="avatar"
  />
  <h1 class="name">{YOUR_NAME}</h1>
  <p class="name-cn">({YOUR_NAME_CN})</p>
  <p class="aff">{YOUR_TITLE} @ <a href="{YOUR_AFFILIATION_URL}" target="_blank">{YOUR_AFFILIATION}</a></p>
  <div class="kw">
    <span>{YOUR_KEYWORD_1}</span>
    <span>{YOUR_KEYWORD_2}</span>
    <span>{YOUR_KEYWORD_3}</span>
    <span>{YOUR_KEYWORD_4}</span>
  </div>
  <p class="loc"><i class="fa-solid fa-location-dot"></i> {YOUR_LOCATION}</p>
  <div class="icons">
    <a href="mailto:{YOUR_EMAIL}"><i class="fa-solid fa-envelope"></i><span>Email</span></a>
    <a href="{YOUR_TWITTER_URL}" target="_blank"><i class="fa-brands fa-x-twitter"></i><span>Twitter / X</span></a>
    <a href="{YOUR_LINKEDIN_URL}" target="_blank"><i class="fa-brands fa-linkedin"></i><span>LinkedIn</span></a>
    <a href="{YOUR_DBLP_URL}" target="_blank"><i class="ai ai-dblp"></i><span>DBLP</span></a>
    <a href="https://github.com/{YOUR_GITHUB}" target="_blank"><i class="fa-brands fa-github"></i><span>GitHub</span></a>
    <a href="{YOUR_SCHOLAR_URL}" target="_blank"><i class="ai ai-google-scholar"></i><span>Scholar</span></a>
    <a href="{YOUR_ORCID_URL}" target="_blank"><i class="ai ai-orcid"></i><span>ORCID</span></a>
  </div>
</aside>

<!-- ============================================================
     MAIN CONTENT
     ============================================================ -->
<main class="hp-main">

<!-- ── About Me ── -->
<section id="about-me">
<h2>About Me</h2>
<p>
  I am currently a {YOUR_YEAR}-year <a href="{YOUR_PROGRAM_URL}" target="_blank">{YOUR_DEGREE}</a> student
  at the <a href="{YOUR_SCHOOL_URL}" target="_blank">{YOUR_SCHOOL}</a>,
  <a href="{YOUR_UNIVERSITY_URL}" target="_blank">{YOUR_UNIVERSITY}</a>,
  fortunate to be advised by
  <a href="{YOUR_ADVISOR_1_URL}" target="_blank">{YOUR_ADVISOR_1}</a>
  and <a href="{YOUR_ADVISOR_2_URL}" target="_blank">{YOUR_ADVISOR_2}</a>.
  I earned my {YOUR_PREV_DEGREE_1} ({YOUR_PREV_DEGREE_1_YEAR}) and {YOUR_PREV_DEGREE_2} ({YOUR_PREV_DEGREE_2_YEAR})
  from <a href="{YOUR_PREV_UNIVERSITY_URL}" target="_blank">{YOUR_PREV_UNIVERSITY}</a>.
</p>
<p>
  {YOUR_CURRENT_ROLE_DESCRIPTION}. Previously, I held research positions at {YOUR_PREV_POSITIONS}.
  I have published {YOUR_PAPER_COUNT} papers in top-tier conferences and journals
  ({YOUR_FIRST_AUTHOR_COUNT} first-author), including {YOUR_VENUES_LIST}.
</p>

<h3>Research Interests:</h3>
<ul>
  <li><strong>{YOUR_INTEREST_1}</strong> — {YOUR_INTEREST_1_DESC}</li>
  <li><strong>{YOUR_INTEREST_2}</strong> — {YOUR_INTEREST_2_DESC}</li>
  <li><strong>{YOUR_INTEREST_3}</strong> — {YOUR_INTEREST_3_DESC}</li>
</ul>
<p><em>{YOUR_VISION_STATEMENT}</em></p>
</section>

<!-- ── News ── -->
<section id="news">
<h2>🔥 News</h2>
{% assign news = site.news | reverse %}
{% assign news_size = site.news | size %}
<ul class="news-list">
{% for item in news limit: 12 %}
  <li>
    <strong>{{ item.date | date: '%Y.%m' }}</strong> :
    {% if item.inline -%}
      {{ item.content | remove: '<p>' | remove: '</p>' | emojify }}
    {%- else -%}
      <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
    {%- endif %}
  </li>
{% endfor %}
</ul>
{% if news_size > 12 %}
<details class="news-more">
  <summary>Show more</summary>
  <ul class="news-list">
  {% for item in news offset: 12 %}
    <li>
      <strong>{{ item.date | date: '%Y.%m' }}</strong> :
      {% if item.inline -%}
        {{ item.content | remove: '<p>' | remove: '</p>' | emojify }}
      {%- else -%}
        <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
      {%- endif %}
    </li>
  {% endfor %}
  </ul>
</details>
{% endif %}
</section>

<!-- ── Education ── -->
<section id="education">
<h2>📖 Education</h2>
<ul class="tl">
  <li>
    <div class="tl-icon">🎓</div>
    <div class="tl-body">
      <div class="tl-head">
        <span class="tl-date">{YOUR_EDU_1_START} - {YOUR_EDU_1_END}</span> &#124;
        <span class="tl-title">{YOUR_EDU_1_DEGREE}</span>
      </div>
      <div class="tl-sub">{YOUR_EDU_1_SCHOOL}, <a href="{YOUR_EDU_1_URL}" target="_blank">{YOUR_EDU_1_UNIVERSITY}</a></div>
    </div>
  </li>
  <li>
    <div class="tl-icon">🎓</div>
    <div class="tl-body">
      <div class="tl-head">
        <span class="tl-date">{YOUR_EDU_2_START} - {YOUR_EDU_2_END}</span> &#124;
        <span class="tl-title">{YOUR_EDU_2_DEGREE}</span>
      </div>
      <div class="tl-sub"><a href="{YOUR_EDU_2_URL}" target="_blank">{YOUR_EDU_2_UNIVERSITY}</a></div>
    </div>
  </li>
  <!-- Add more entries as needed -->
</ul>
</section>

<!-- ── Research Experience ── -->
<section id="experience">
<h2>💻 Research Experience</h2>
<ul class="tl">
  <li>
    <div class="tl-icon">💼</div>
    <div class="tl-body">
      <div class="tl-head">
        <span class="tl-date">{YOUR_EXP_1_START} - {YOUR_EXP_1_END}</span> &#124;
        <span class="tl-title">{YOUR_EXP_1_ORG}, {YOUR_EXP_1_TEAM}</span>
      </div>
      <ul class="tl-details">
        <li>{YOUR_EXP_1_ROLE}</li>
        <li>Mentors: <a href="{YOUR_EXP_1_MENTOR_1_URL}" target="_blank">{YOUR_EXP_1_MENTOR_1}</a>, <a href="{YOUR_EXP_1_MENTOR_2_URL}" target="_blank">{YOUR_EXP_1_MENTOR_2}</a></li>
      </ul>
    </div>
  </li>
  <li>
    <div class="tl-icon">💼</div>
    <div class="tl-body">
      <div class="tl-head">
        <span class="tl-date">{YOUR_EXP_2_START} - {YOUR_EXP_2_END}</span> &#124;
        <span class="tl-title">{YOUR_EXP_2_ORG}, {YOUR_EXP_2_TEAM}</span>
      </div>
      <ul class="tl-details">
        <li>{YOUR_EXP_2_ROLE}</li>
        <li>Mentor: <a href="{YOUR_EXP_2_MENTOR_URL}" target="_blank">{YOUR_EXP_2_MENTOR}</a></li>
      </ul>
    </div>
  </li>
  <!-- Add more entries as needed -->
</ul>
</section>

<!-- ── Honors & Awards ── -->
<section id="honors">
<h2>🏆 Honors &amp; Awards</h2>

<h3>Grants</h3>
<ul class="awards-list">
  <li>{YOUR_GRANT_1_YEAR}: {YOUR_GRANT_1_DESC}</li>
  <li>{YOUR_GRANT_2_YEAR}: {YOUR_GRANT_2_DESC}</li>
</ul>

<h3>Scholarships</h3>
<ul class="awards-list">
  <li>{YOUR_SCHOLARSHIP_1_YEAR}: {YOUR_SCHOLARSHIP_1_DESC}</li>
  <li>{YOUR_SCHOLARSHIP_2_YEAR}: {YOUR_SCHOLARSHIP_2_DESC}</li>
  <li>{YOUR_SCHOLARSHIP_3_YEAR}: {YOUR_SCHOLARSHIP_3_DESC}, <a href="{YOUR_SCHOLARSHIP_3_URL}" target="_blank">[Link]</a></li>
</ul>

<h3>Competitions</h3>
<ul class="awards-list">
  <li>{YOUR_COMP_1_YEAR}: {YOUR_COMP_1_DESC}</li>
  <li>{YOUR_COMP_2_YEAR}: {YOUR_COMP_2_DESC}, <a href="{YOUR_COMP_2_URL}" target="_blank">[Link]</a></li>
</ul>
</section>

<!-- ── Selected Preprints ── -->
<section id="preprints">
<h2>📝 Selected Preprints</h2>
<p style="font-size:0.82rem;opacity:0.5;margin-bottom:1em;">* corresponding author &ensp; # equal contribution</p>

<div class="paper">
  <div class="p-title"><a href="{YOUR_PREPRINT_1_URL}" target="_blank">{YOUR_PREPRINT_1_TITLE}</a></div>
  <div class="p-authors">{YOUR_PREPRINT_1_AUTHORS}</div>
  <div class="p-meta">
    <span class="p-links">
      <a href="{YOUR_PREPRINT_1_PDF}" target="_blank">paper</a>
      <a href="{YOUR_PREPRINT_1_CODE}" target="_blank">code</a>
    </span>
  </div>
</div>

<div class="paper">
  <div class="p-title"><a href="{YOUR_PREPRINT_2_URL}" target="_blank">{YOUR_PREPRINT_2_TITLE}</a></div>
  <div class="p-authors">{YOUR_PREPRINT_2_AUTHORS}</div>
  <div class="p-meta">
    <span class="p-links">
      <a href="{YOUR_PREPRINT_2_PDF}" target="_blank">paper</a>
    </span>
  </div>
</div>

<!-- Add more preprint entries as needed -->
</section>

<!-- ── Selected Publications ── -->
<section id="publications">
<h2>📝 Selected Publications（<a href="{YOUR_SCHOLAR_URL}" target="_blank">Full List</a>）</h2>

<!-- Rendered from _bibliography/papers.bib entries with selected={true}.
     Add venue info via the `abbr` field in each bib entry. -->
{% include selected_papers.liquid %}

<!-- You may also add custom paper entries below for papers
     not in papers.bib, using the same HTML format as Preprints above:

<div class="paper">
  <div class="p-title"><a href="URL" target="_blank">Paper Title</a></div>
  <div class="p-authors">Author1, <strong>Your Name</strong>, Author2</div>
  <div class="p-meta">
    <span class="p-venue">VENUE YEAR (CCF-X)</span>
    <span class="p-links">
      <a href="URL" target="_blank">paper</a>
      <a href="URL" target="_blank">code</a>
    </span>
  </div>
</div>
-->
</section>

<!-- ── Invited Talks ── -->
<section id="talks">
<h2>🎤 Invited Talks</h2>
<ul class="talks-list">
  <li><strong>{YOUR_TALK_1_DATE}</strong>: "{YOUR_TALK_1_TITLE}", {YOUR_TALK_1_VENUE}, <a href="{YOUR_TALK_1_SLIDES}" target="_blank">[Slides]</a></li>
  <li><strong>{YOUR_TALK_2_DATE}</strong>: "{YOUR_TALK_2_TITLE}", {YOUR_TALK_2_VENUE}</li>
  <!-- Add more entries as needed -->
</ul>
</section>

<!-- ── Academic Services ── -->
<section id="services">
<h2>🔍 Academic Services</h2>

<h3>Journal Reviewer</h3>
<ul class="services-list">
  <li>{YOUR_JOURNAL_1}</li>
</ul>

<h3>Program Committee Member / Reviewer</h3>
<ul class="services-list">
  <li>{YOUR_CONF_AREA_1}: {YOUR_CONF_LIST_1}</li>
  <li>{YOUR_CONF_AREA_2}: {YOUR_CONF_LIST_2}</li>
</ul>
</section>

<footer class="hp-footer">
  © {{ 'now' | date: '%Y' }} {YOUR_NAME}
</footer>

</main>

<!-- ============================================================
     RIGHT TABLE OF CONTENTS
     ============================================================ -->
<nav class="hp-toc" aria-label="Table of contents">
  <ul>
    <li><a href="#about-me">About Me</a></li>
    <li><a href="#news">🔥 News</a></li>
    <li><a href="#education">📖 Education</a></li>
    <li><a href="#experience">💻 Experience</a></li>
    <li><a href="#honors">🏆 Honors &amp; Awards</a></li>
    <li><a href="#preprints">📝 Preprints</a></li>
    <li><a href="#publications">📝 Publications</a></li>
    <li><a href="#talks">🎤 Invited Talks</a></li>
    <li><a href="#services">🔍 Services</a></li>
  </ul>
</nav>

</div>

<!-- ToC active-link highlight (no external libraries) -->
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
