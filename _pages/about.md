---
layout: about
title: about
permalink: /
subtitle: ""

profile:
  align: right
  image: prof_pic.jpg
  image_circular: true

selected_papers: true
social: true

announcements:
  enabled: true
  scrollable: false
  limit: 5

latest_posts:
  enabled: false
---

<style>
/* ── Page width ── */
.post {
  max-width: 700px !important;
  margin-left: auto !important;
  margin-right: auto !important;
  padding-top: 0 !important;
}

/* ── Hide default title block ── */
.post-header .post-title {
  display: none !important;
}
.post-header .desc {
  display: none !important;
}
.post-header {
  margin-bottom: 0 !important;
  padding-bottom: 0 !important;
}

/* ── Profile: centered, unfloated ── */
.profile {
  float: none !important;
  width: auto !important;
  max-width: none !important;
  text-align: center !important;
  margin: 0 auto 0.3rem !important;
  padding: 0 !important;
}
.profile figure,
.profile .figure {
  display: inline-block !important;
  width: 130px !important;
  margin: 0 auto !important;
}
.profile img {
  width: 130px !important;
  height: 130px !important;
  object-fit: cover !important;
}
.profile .more-info {
  display: none !important;
}
.post .z-depth-1 {
  box-shadow: none !important;
}

/* ── Typography ── */
.post article {
  line-height: 1.85;
}
.post article .clearfix p {
  margin-bottom: 1.5em;
}
.clearfix .page-heading {
  text-align: center;
  font-size: 1.45rem;
  font-weight: 300;
  letter-spacing: 0.01em;
  margin-top: 0.4rem;
  margin-bottom: 2.8rem;
  line-height: 1.4;
  opacity: 0.88;
}

/* ── Section headings: replace text via CSS ── */
.post article > h2 {
  margin-top: 4rem !important;
  margin-bottom: 1.2rem !important;
  padding-bottom: 0 !important;
  border: none !important;
}
.post article > h2 a {
  pointer-events: none !important;
  cursor: default !important;
  text-decoration: none !important;
  color: inherit !important;
  font-size: 0 !important;
  line-height: 0 !important;
}
.post article > h2 a[href*="news"]::after {
  content: "some ongoing notes";
  font-size: 1rem;
  font-weight: 400;
  font-style: italic;
  opacity: 0.45;
  line-height: 1.85;
}
.post article > h2 a[href*="publications"]::after {
  content: "work I care about";
  font-size: 1rem;
  font-weight: 400;
  font-style: italic;
  opacity: 0.45;
  line-height: 1.85;
}

/* ── News: personal log / journal style ── */
.news .table-responsive {
  max-height: none !important;
  overflow: visible !important;
}
.news table.table {
  border: none !important;
}
.news table.table tbody {
  display: block !important;
}
.news table.table tr {
  display: block !important;
  margin-bottom: 0.85em !important;
  border: none !important;
}
.news table.table th {
  display: block !important;
  border: none !important;
  padding: 0 !important;
  font-weight: 400 !important;
  font-size: 0.75rem !important;
  opacity: 0.35;
  width: auto !important;
  letter-spacing: 0.06em;
  text-transform: uppercase;
}
.news table.table td {
  display: block !important;
  border: none !important;
  padding: 0.1em 0 0 0 !important;
  line-height: 1.7;
}
.news table.table td a.news-title {
  text-decoration: none;
  font-weight: 400;
}

/* ── Publications: clean reading style ── */
.publications ol {
  list-style: none !important;
  padding-left: 0 !important;
}
.publications ol li {
  margin-bottom: 1.8em !important;
  padding: 0 !important;
  border: none !important;
  box-shadow: none !important;
  background: transparent !important;
}
.publications .col-sm-2.abbr,
.publications .col.col-sm-2.abbr {
  display: none !important;
}
.publications .col-sm-8 {
  flex: 0 0 100% !important;
  max-width: 100% !important;
  padding-left: 0 !important;
}
.publications .row {
  margin: 0 !important;
  border: none !important;
  box-shadow: none !important;
  padding: 0 !important;
}
.publications .title {
  font-weight: 500;
  font-size: 1rem;
  margin-bottom: 0.15em;
}
.publications .author {
  font-size: 0.9rem;
  opacity: 0.75;
}
.publications .periodical {
  font-size: 0.88rem;
  opacity: 0.6;
}
.publications .links .btn {
  border: none !important;
  box-shadow: none !important;
  font-size: 0.78rem !important;
  padding: 0.1em 0.45em !important;
  opacity: 0.55;
}
.publications .links .btn:hover {
  opacity: 1;
}
.publications .badges {
  display: none !important;
}

/* ── Social ── */
.social {
  margin-top: 4rem !important;
  text-align: center !important;
}
.social .contact-icons {
  justify-content: center !important;
}
.social .contact-note {
  font-size: 0.85rem;
  opacity: 0.45;
  margin-top: 0.5rem;
}

/* ── Global cleanup ── */
.post article .news,
.post article .publications,
.post article .social {
  border: none !important;
  box-shadow: none !important;
}
</style>

<h1 class="page-heading">A Walk by the Sea & Sunshine</h1>

I'm Jun Wang — friends know me as Kaik. This fall I'll be starting my M.S. in Computer Science at UC San Diego, which feels like the right place to be: close to the ocean, close to ideas I care about, and just far enough from the familiar to make things interesting.

My background is a bit unusual for someone heading into CS grad school. I studied Urban Forestry at Beijing Forestry University — yes, trees — with a minor in Computer Science. Somewhere between ecological modeling and late-night algorithm practice sessions, I realized that what excites me most is finding hidden structure in complex data. The trees were beautiful, but the patterns underneath were what kept me up at night.

Recently, I've been working on a clustering framework called GCAO — _Group-driven Clustering via Gravitational Attraction and Optimization_. The core idea is borrowed from physics: what if data points attracted each other the way masses do, forming natural groups through gravitational pull? It's still under review, but the early results have been encouraging — meaningful improvements over standard baselines across eleven high-dimensional datasets. This line of thinking, using physical metaphors to organize messy real-world data, is where I want to spend my research energy going forward.

On the practical side, I'm currently at ByteDance, building and evaluating coding agents. My day-to-day involves everything from WebSocket streaming interfaces to designing benchmarks that actually measure whether an AI system can reason. It's a sharp contrast to the quiet patience of research, but I've come to appreciate both rhythms — one teaches you to think carefully, the other teaches you to ship.

When I'm not at a keyboard, I'm usually chasing sea and sunshine — learning to surf along the coast, occasionally paragliding, or wandering through places like Bali and Solo in Indonesia. I believe the best ideas come when you give your mind room to breathe.
