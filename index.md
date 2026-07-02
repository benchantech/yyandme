---
layout: default
title: YY and Me Podcast
---

<div class="hero-band">
  <div class="hero-home">
    <div>
      <div class="mono-kicker">WITH BEN CHAN · IN REAL-TIME</div>
      <h1>A Canon of Growing&nbsp;Echoes</h1>
      <p class="hero-tagline">A podcast by Ben Chan exploring and building legacy, myth, violin, and AI — in real-time.</p>
      <div class="hero-cta">
        <a class="btn-cream" href="{{ '/episodes/the-first-echo/' | relative_url }}">▶&nbsp;&nbsp;Start with The First Echo</a>
        <span class="hero-note">the foundation of everything that follows</span>
      </div>
    </div>
    <img class="hero-art" src="{{ '/assets/yyandme-art-1500x1500.jpg' | relative_url }}" alt="YY, a plush squirrel, on the YY and Me cover">
  </div>
</div>

<div class="wrap-800 canon-section">
  <div class="canon-head">
    <span class="mono-label">THE CANON — {{ site.episodes | size }} EPISODES</span>
    <span class="mono-note">newest echo first</span>
  </div>
  <div class="episode-list">
    {%- assign eps = site.episodes | sort: "n" | reverse -%}
    {%- for ep in eps -%}
      {%- include episode-row.html ep=ep show_arc=true -%}
    {%- endfor -%}
  </div>
</div>

<div class="wrap-800 listen-row">
  <span class="mono-label">LISTEN</span>
  <a class="pill-link" href="https://podcasts.apple.com/podcast/yy-and-me/id1826275180" target="_blank" rel="noopener">Apple Podcasts</a>
  <a class="pill-link" href="https://open.spotify.com/show/7snHYZsCpO1oNidk2RZh02" target="_blank" rel="noopener">Spotify</a>
  <a class="pill-link" href="{{ '/feed.xml' | relative_url }}">RSS Feed</a>
  <a class="pill-link" href="{{ '/the-first-echo/' | relative_url }}">Feedback</a>
</div>
