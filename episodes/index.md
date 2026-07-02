---
layout: default
title: All Episodes
permalink: /episodes/
---

<div class="hero-band">
  <div class="hero-center">
    <div class="mono-kicker">THE CANON · {{ site.episodes | size }} EPISODES</div>
    <h1>Episodes</h1>
    <p class="hero-blurb">Start with The First Echo to understand the foundation of everything that follows.</p>
  </div>
</div>

<div class="wrap-800 canon-section">
  {%- assign sorted = site.episodes | sort: "n" | reverse -%}
  {%- assign arc1 = sorted | where: "arc", "Arc 1" -%}
  {%- assign foundation = sorted | where: "arc", "Foundation" -%}

  <div class="arc-group">
    <div class="section-rule">
      <span class="mono-label">ARC 1</span>
      <span class="line"></span>
      <span class="mono-note">{{ arc1 | size }} echoes</span>
    </div>
    <div class="episode-list">
      {%- for ep in arc1 -%}
        {%- include episode-row.html ep=ep -%}
      {%- endfor -%}
    </div>
  </div>

  <div class="arc-group">
    <div class="section-rule">
      <span class="mono-label">FOUNDATION</span>
      <span class="line"></span>
      <span class="mono-note">where it begins</span>
    </div>
    <div class="episode-list">
      {%- for ep in foundation -%}
        {%- include episode-row.html ep=ep -%}
      {%- endfor -%}
    </div>
  </div>
</div>
