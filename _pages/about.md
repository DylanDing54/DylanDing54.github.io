---
permalink: /
title: "Yifan Ding"
author_profile: true
sidebar_nav: true
redirect_from: 
  - /about/
  - /about.html
---

About Me
======
I am a Master's student in Integrated Circuit Engineering at [Peking University](https://www.pku.edu.cn/), advised by [Prof. Tianyu Jia](https://ic.pku.edu.cn/en/Faculty/Facultys/IntegratedCircuitDesign/Jia_Tianyu/index.htm) and [Prof. Dunshan Yu](https://ic.pku.edu.cn/en/Faculty/Facultys/IntegratedCircuitDesign/YuDunshan/index.htm). Before that, I received my Bachelor's degree in Integrated Circuit Design and Integrated Systems from Hefei University of Technology.

My research sits at the intersection of computer architecture and machine learning systems. I am interested in how emerging integration technologies — 3D stacking, hybrid bonding, chiplets, and optical interconnects — can be co-designed with algorithms to make large model inference and training substantially more efficient.

Recent News
======
<div class="news-list">
  <div class="news-item">
    <span class="news-date">09/2026</span>
    <span class="news-text">One first-author paper accepted to <strong>ASP-DAC 2027</strong>.</span>
  </div>
  <div class="news-item">
    <span class="news-date">05/2026</span>
    <span class="news-text">Attended <strong>ISCAS 2026</strong>, supported by a conference sponsorship.</span>
  </div>
  <div class="news-item">
    <span class="news-date">05/2026</span>
    <span class="news-text">One first-author paper accepted to <strong>ISLPED 2026</strong>.</span>
  </div>
  <div class="news-item">
    <span class="news-date">11/2025</span>
    <span class="news-text">One co-authored paper accepted to <strong>DATE 2026</strong>.</span>
  </div>
  <div class="news-item">
    <span class="news-date">11/2025</span>
    <span class="news-text">One co-authored paper accepted to <strong>ISSCC 2026</strong> (Highlight).</span>
  </div>
  <div class="news-item">
    <span class="news-date">09/2024</span>
    <span class="news-text">Joined the <a href="https://www.tianyuj.com/index.html" target="_blank" rel="noopener">PACIFIC Lab</a> at Peking University.</span>
  </div>
</div>

Research Interests
======
* **3D integration architecture for emerging AI applications** — hybrid-bonding and 3D-stacked accelerators for LLM, VLM, and VLA workloads
* **Scalable AI computing systems** — heterogeneous GPU-PNM systems, chiplet architectures with optical interconnects, and cross-layer optimization for training clusters
* **Efficient RISC-V AI accelerator chips** — compute-in-memory designs, full-stack implementation from RTL through tape-out

Education
======
<div class="education-list">
  <div class="education-item">
    <div class="education-degree"><strong>M.S. in Integrated Circuit Engineering</strong></div>
    <div class="education-school">Peking University, Beijing, China<span class="education-date">Sep. 2024 &ndash; Jun. 2027 (expected)</span></div>
    <div class="education-detail">Advisors: Prof. Tianyu Jia, Prof. Dunshan Yu</div>
  </div>
  <div class="education-item">
    <div class="education-degree"><strong>B.S. in Integrated Circuit Design and Integrated Systems</strong></div>
    <div class="education-school">Hefei University of Technology, Hefei, China<span class="education-date">Sep. 2019 &ndash; Jun. 2023</span></div>
  </div>
</div>

Experience
======
<div class="experience-list">
  <div class="experience-item">
    <div class="experience-role"><strong>Project Collaboration, Huawei 2012 Laboratories</strong></div>
    <div class="experience-org">Joint university-industry project<span class="experience-date">Nov. 2025 &ndash; Feb. 2026</span></div>
    <div class="experience-detail">Helped build a cycle-level hardware simulator for a custom dataflow processor.</div>
  </div>
</div>

Publications
======
<div class="publication-list">
{% for post in site.publications reversed %}
  <div class="publication-item">
    <div class="publication-title">{% if post.paperurl %}<a href="{{ post.paperurl }}" target="_blank" rel="noopener">{{ post.title }}</a>{% else %}{{ post.title }}{% endif %}</div>
    <div class="publication-authors">{{ post.authors }}{% if post.author_note %} <span class="publication-note">{{ post.author_note }}</span>{% endif %}</div>
    <div class="publication-venue">{{ post.venue }}{% if post.venue_short %} (<span class="publication-venue-short">{{ post.venue_short }}</span>){% endif %}, {% if post.year %}{{ post.year }}{% else %}{{ post.date | date: "%Y" }}{% endif %}.{% if post.note %} <span class="publication-badge">{{ post.note }}</span>{% endif %}</div>
  </div>
{% endfor %}
</div>

Honors and Awards
======
* Merit Student of Peking University, 2025
* Hefei University of Technology's Science and Technology Activity Awards, 2022
* Honorable Mention, National Finals, The 6th National College Student Integrated Circuit Innovation and Entrepreneurship Competition, Ministry of Industry and Information Technology, 2022
* Honorable Mention, National Finals, National College Student FPGA Innovation Design Competition, Chinese Institute of Electronics, 2022

Gallery
======
{% for entry in site.data.gallery %}
<div class="gallery-entry">
  <div class="gallery-entry-title">{{ entry.title }}</div>
  <div class="gallery-grid">
  {% for photo in entry.images %}
    <figure class="gallery-item">
      <img src="{{ photo.image | prepend: '/images/gallery/' | relative_url }}" alt="{{ photo.alt }}" loading="lazy">
    </figure>
  {% endfor %}
  </div>
  {% if entry.description %}<p class="gallery-entry-desc">{{ entry.description }}</p>{% endif %}
</div>
{% endfor %}

