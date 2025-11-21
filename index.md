---
layout: full_width
title: Home
---

<header class="site-header">
  <nav class="site-nav">
    {% for item in site.navigation %}
      <a href="{{ item.url | relative_url }}" {% if page.url == item.url %}class="active"{% endif %}>{{ item.title }}</a>
    {% endfor %}
  </nav>
</header>

<article>
  <h1>{{ site.title }}</h1>
  <p class="subtitle">{{ site.description }}</p>

  <figure class="logo-figure">
    <img src="{{ '/images/logo.jpg' | relative_url }}" alt="Course Logo" class="course-logo"/>
  </figure>

  <section>
    <h2>Welcome</h2>
    <p>This course explores the intersection of machine learning and systematic trading strategies. You will learn to design, implement, and evaluate algorithmic trading systems using modern ML techniques.</p>
  </section>

  <section>
    <h2>Getting Started</h2>
    <p>All programming sessions are written as Jupyter notebooks and run directly in <a href="https://colab.research.google.com/">Google Colab</a>.</p>

    <p>If you prefer to run scripts locally on your machine, follow the <a href="https://colab.research.google.com/drive/1GtAF3kuPGDhxRYacLVUMm5S8f1uBA_oM?usp=sharing">installation instructions</a>.</p>
  </section>

  <section>
    <h2>Course Structure</h2>
    <ul>
      <li><strong>7 Lectures</strong> covering ML foundations to advanced neural networks</li>
      <li><strong>8 Programming Sessions</strong> with hands-on Colab notebooks</li>
      <li><strong>Weekly MCQs</strong> to reinforce concepts</li>
      <li><strong>1 Coursework</strong> project applying learned techniques</li>
      <li><strong>Final Exam</strong> with mock exam provided</li>
    </ul>
  </section>

  <section>
    <h2>Quick Links</h2>
    <div class="quick-links">
      <a href="{{ '/syllabus' | relative_url }}" class="link-card">
        <strong>Syllabus</strong><br/>
        <span>Weekly schedule & materials</span>
      </a>
      <a href="{{ '/programming' | relative_url }}" class="link-card">
        <strong>Programming</strong><br/>
        <span>Colab notebooks & solutions</span>
      </a>
      <a href="{{ '/assessments' | relative_url }}" class="link-card">
        <strong>Assessments</strong><br/>
        <span>Coursework, exams & quizzes</span>
      </a>
      <a href="{{ '/resources' | relative_url }}" class="link-card">
        <strong>Resources</strong><br/>
        <span>Office hours & contact</span>
      </a>
    </div>
  </section>
</article>
