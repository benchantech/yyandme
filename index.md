---
layout: default
title: YY and Me Podcast
---

<div class="hero">
  <h1>A Canon of Growing Echoes</h1>
  <p>A podcast by Ben Chan exploring and building legacy, myth, violin, and AI - in real-time.</p>
  <p>Start with <strong><a href="/episodes/the-first-echo/">The First Echo</a></strong> to understand the foundation of everything that follows.</p>
</div>

<div class="episodes-grid">
  {%- assign eps = site.episodes | sort: "n" | reverse -%}
  {%- for ep in eps -%}
    {%- include episode-card.html ep=ep -%}
  {%- endfor -%}
</div>