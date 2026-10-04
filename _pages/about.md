---
permalink: /
title: ""
excerpt: ""
author_profile: true
publications:
  - title: '“Do I Trust the AI?” Towards Trustworthy AI-Assisted Diagnosis: Understanding User Perception in LLM-Supported Clinical Reasoning'
    venue_short: "CHI 2026"
    type: "Research Article"
    venue: "Proceedings of the 2026 CHI Conference on Human Factors in Computing Systems"
    authors:
      - Yuansong Xu
      - Yichao Zhu
      - Haokai Wang
      - Yuchen Wu
      - Yang Ouyang
      - Hanlu Li
      - Wenzhe Zhou
      - Xinyu Liu
      - Chang Jiang
      - Quan Li
    url: "https://dl.acm.org/doi/full/10.1145/3772318.3790835"
    doi: "https://doi.org/10.1145/3772318.3790835"
    teaser: "/images/CHI 26.png"
redirect_from:
  - /about/
  - /about.html
---

<section class="hero" id="about-me">
  <h1>Hi, I'm Yichao Zhu.</h1>
  <p class="hero__intro">I'm a first-year master's student at the <a href="https://sist.shanghaitech.edu.cn/">School of Information Science and Technology</a>, ShanghaiTech University, supervised by Prof. <a href="https://faculty.sist.shanghaitech.edu.cn/liquan/">Quan Li</a>. My research interests include human-computer interaction and data visualization, with a recent focus on their applications in healthcare.</p>
</section>

<section class="profile-section" id="publications">
  <div class="section-heading">
    <span class="section-heading__number">01</span>
    <div><h2>Publications</h2></div>
  </div>
  {% for publication in page.publications %}
  <article class="publication-card{% if publication.teaser and publication.teaser != '' %} publication-card--with-teaser{% endif %}">
    {% if publication.teaser and publication.teaser != '' %}
    <a class="publication-card__teaser" href="{{ publication.url }}"><img src="{{ publication.teaser | relative_url }}" alt="Teaser for {{ publication.title | escape }}" loading="lazy"></a>
    {% endif %}
    <div class="publication-card__body">
      <div class="publication-card__meta"><span>{{ publication.venue_short }}</span><span>{{ publication.type }}</span></div>
      <h3><a href="{{ publication.url }}">{{ publication.title }}</a></h3>
      <p>{% for author in publication.authors %}{% if forloop.last and forloop.length > 1 %}and {% endif %}{% if author == "Yichao Zhu" %}<strong>{{ author }}</strong>{% else %}{{ author }}{% endif %}{% unless forloop.last %}, {% endunless %}{% endfor %}</p>
      <div class="publication-card__footer"><span>{{ publication.venue }}</span><a href="{{ publication.doi }}">DOI ↗</a></div>
    </div>
  </article>
  {% endfor %}
</section>

<section class="profile-section" id="honors-and-awards">
  <div class="section-heading">
    <span class="section-heading__number">02</span>
    <div><h2>Honors &amp; Awards</h2></div>
  </div>
  <div class="timeline">
    <article class="timeline__item">
      <time>2026</time>
      <div><h3>ChinaVis 2026 Data Visualization Challenge</h3><p>Second Prize</p></div>
    </article>
    <article class="timeline__item">
      <span class="timeline__label">ShanghaiTech</span>
      <div><h3>ShanghaiTech University AI Innovation Application Competition</h3><p>Track Excellence Award</p></div>
    </article>
    <article class="timeline__item">
      <time>Sep 2024</time>
      <div><h3>National Undergraduate Mathematical Contest in Modeling</h3><p>Second Prize · Shanghai Zone</p></div>
    </article>
    <article class="timeline__item">
      <time>Jul 2023</time>
      <div><h3>Outstanding Social Practice Member</h3><p>Recognized for community engagement and contribution.</p></div>
    </article>
  </div>
</section>

<section class="profile-section" id="education">
  <div class="section-heading">
    <span class="section-heading__number">03</span>
    <div><h2>Education</h2></div>
  </div>
  <div class="education-list">
    <article class="feature-card">
      <div class="feature-card__mark"><img src="{{ '/images/education-master.png' | relative_url }}" alt="" aria-hidden="true"></div>
      <div><time>2026 — Present</time><h3>ShanghaiTech University</h3><p>Master's Student · School of Information Science and Technology · Shanghai</p></div>
    </article>
    <article class="feature-card">
      <div class="feature-card__mark"><img src="{{ '/images/education-bachelor.png' | relative_url }}" alt="" aria-hidden="true"></div>
      <div><time>2022 — 2026</time><h3>ShanghaiTech University</h3><p>Bachelor's Degree · School of Information Science and Technology · Shanghai</p></div>
    </article>
  </div>
</section>

<section class="profile-section" id="service">
  <div class="section-heading">
    <span class="section-heading__number">04</span>
    <div><h2>Service</h2></div>
  </div>
  <div class="service-grid">
    <article class="service-card"><time>Fall 2027</time><h3>Teaching Assistant</h3><p>ART 1422 · Data Visualization</p></article>
    <article class="service-card"><time>Spring 2026</time><h3>Teaching Assistant</h3><p>SI100B · Introduction to Information Science and Technology</p></article>
    <article class="service-card"><time>2024.09 — 2025.09</time><h3>President</h3><p>ShanghaiTech Music Club</p></article>
    <article class="service-card"><time>2023.09 — 2025.09</time><h3>Student Assistant</h3><p>Mind and Health Center</p></article>
  </div>
</section>
