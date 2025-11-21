---
layout: full_width
title: Resources
permalink: /resources/
---

<header class="site-header">
  <nav class="site-nav">
    {% for item in site.navigation %}
      <a href="{{ item.url | relative_url }}" {% if page.url == item.url %}class="active"{% endif %}>{{ item.title }}</a>
    {% endfor %}
  </nav>
</header>

<article>
  <h1>Resources</h1>
  <p class="subtitle">Office hours, setup instructions, and contact information</p>

  <section>
    <h2>Office Hours</h2>
    <p>In-person office hours are held weekly during term time. Please check the schedule below.</p>

    <table class="office-hours-table">
      <thead>
        <tr>
          <th>Date</th>
          <th>Time</th>
          <th>Location</th>
          <th>Notes</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>Thu 22 May</td>
          <td>13:00-14:00</td>
          <td>Business School Boardroom</td>
          <td>Level 1, opposite LT1</td>
        </tr>
        <tr>
          <td>Thu 22 May</td>
          <td>17:00-18:00</td>
          <td>LT2</td>
          <td>Same lecture theatre as class</td>
        </tr>
        <tr>
          <td>Thu 29 May</td>
          <td>13:00-14:00</td>
          <td>CAGB 475</td>
          <td>Through the door by elevators into City & Guilds hallway</td>
        </tr>
        <tr>
          <td>Thu 29 May</td>
          <td>17:00-18:00</td>
          <td>LT2</td>
          <td>Same lecture theatre as class</td>
        </tr>
        <tr>
          <td>Thu 05 Jun</td>
          <td>13:00-14:00</td>
          <td>Business School Boardroom</td>
          <td>Same location as 22 May</td>
        </tr>
        <tr>
          <td>Thu 05 Jun</td>
          <td>17:00-18:00</td>
          <td>LT2</td>
          <td>Same lecture theatre as class</td>
        </tr>
        <tr>
          <td>Thu 12 Jun</td>
          <td>13:00-14:00</td>
          <td>Room 0.09, 53 Prince's Gate</td>
          <td>Basement level, opposite main Imperial entrance</td>
        </tr>
        <tr>
          <td>Thu 12 Jun</td>
          <td>17:00-18:00</td>
          <td>Room 0.09, 53 Prince's Gate</td>
          <td>Same as above</td>
        </tr>
      </tbody>
    </table>
  </section>

  <section>
    <h2>Getting Started</h2>

    <div class="resource-card">
      <h3>Google Colab (Recommended)</h3>
      <p>All programming sessions run directly in Google Colab - no local installation required. Simply click the Colab links in the syllabus or programming pages.</p>
      <a href="https://colab.research.google.com/" class="btn">Open Google Colab</a>
    </div>

    <div class="resource-card">
      <h3>Local Setup</h3>
      <p>If you prefer to run notebooks locally, follow the installation instructions to set up your Python environment.</p>
      <a href="https://colab.research.google.com/drive/1GtAF3kuPGDhxRYacLVUMm5S8f1uBA_oM?usp=sharing" class="btn">Installation Guide</a>
    </div>
  </section>

  <section>
    <h2>Optional Reading</h2>

    <ul class="reading-list">
      <li>
        <a href="{{ '/Lectures/Session_2/Optional_Lecture_Notes.pdf' | relative_url }}">Lecture 2: Unsupervised Learning Notes</a>
      </li>
      <li>
        <a href="{{ '/Lectures/Session_3/Optional_Lecture_Notes.pdf' | relative_url }}">Lecture 3: Latent Variable Models Notes</a>
      </li>
      <li>
        <a href="{{ '/Lectures/Session_6/Optional_Lecture_Notes.pdf' | relative_url }}">Lecture 6: The Adam Optimizer</a>
      </li>
      <li>
        <a href="{{ '/Lectures/Session_7/Optional_Lecture_Notes.pdf' | relative_url }}">Lecture 7: Time Series Forecasting Notes</a>
      </li>
      <li>
        <a href="{{ '/Lectures/Optional_Session/Optional_Lecture.pdf' | relative_url }}">Probability & Calculus Refresher</a>
      </li>
      <li>
        <a href="{{ '/Lectures/Optional_Session/Graph_Representation_Learning.pdf' | relative_url }}">Graph Representation Learning</a>
      </li>
      <li>
        <a href="https://arxiv.org/pdf/2506.02515">LLMs for Decision Making (ArXiv)</a>
      </li>
    </ul>
  </section>

  <section>
    <h2>Contact</h2>
    <div class="contact-card">
      <h3>Hachem Madmoun</h3>
      <p>For questions about practical implementations and course materials:</p>
      <a href="mailto:h.madmoun@ic.ac.uk" class="btn">h.madmoun@ic.ac.uk</a>
    </div>
  </section>
</article>
