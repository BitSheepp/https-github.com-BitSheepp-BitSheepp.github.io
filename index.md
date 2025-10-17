---
title: BitSheepp
layout: default
---

<link rel="stylesheet" href="{{ '/assets/css/custom.css' | relative_url }}">

{% assign p = site.data.profile %}
<div class="wrapper">
  <section class="hero">
    <h1>{{ p.name }}</h1>
    <div class="subtitle">{{ p.subtitle }}</div>
    <div class="meta">
      {{ p.location }} · <a href="mailto:{{ p.email }}">{{ p.email }}</a> · {{ p.phone }}
    </div>
  </section>

  <section class="section">
    <h2>About</h2>
    <p>{{ p.about }}</p>
    <div class="badges">
      {% for b in p.badges %}<span class="badge">{{ b }}</span>{% endfor %}
    </div>
  </section>

  <section class="section">
    <h2>Quick links</h2>
    <div class="grid">
      <a class="card" href="{{ '/pages/cv/' | relative_url }}"><h3>CV</h3><div class="muted">网页版，数据驱动</div></a>
      <a class="card" href="{{ '/projects/' | relative_url }}"><h3>Projects</h3><div class="muted">平台/算法/论文工程</div></a>
      <a class="card" href="{{ '/publications/' | relative_url }}"><h3>Publications</h3><div class="muted">Journal / Submission</div></a>
      <a class="card" href="{{ '/news/' | relative_url }}"><h3>News</h3><div class="muted">最近动态</div></a>
    </div>
  </section>
</div>
