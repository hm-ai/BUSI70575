---
layout: full_width
title: Assessments
permalink: /assessments/
---

<header class="site-header">
  <nav class="site-nav">
    {% for item in site.navigation %}
      <a href="{{ item.url | relative_url }}" {% if page.url == item.url %}class="active"{% endif %}>{{ item.title }}</a>
    {% endfor %}
  </nav>
</header>

<article>
  <h1>Assessments</h1>
  <p class="subtitle">Coursework, exams, and weekly quizzes</p>

  <section>
    <h2>Coursework</h2>
    <div class="assessment-card coursework">
      <div class="assessment-header">
        <h3>Main Coursework Project</h3>
        <span class="badge">Individual</span>
      </div>
      <div class="assessment-dates">
        <span><strong>Released:</strong> 16 May 2025</span>
        <span><strong>Deadline:</strong> 06 June 2025</span>
      </div>
      <div class="assessment-links">
        <a href="https://colab.research.google.com/drive/1---SysIELmc-zlDn5t3Ebm0H7vFQ41HB?usp=sharing" class="btn btn-colab">Open Coursework</a>
      </div>
    </div>
  </section>

  <section>
    <h2>Exams</h2>

    <div class="exam-grid">
      <div class="assessment-card">
        <h3>Mock Exam 2025</h3>
        <p>Practice exam to prepare for the final.</p>
        <div class="assessment-links">
          <a href="{{ '/Exams/Mock_Exam_2025.pdf' | relative_url }}" class="btn">Exam</a>
          <a href="{{ '/Exams/Solution_Mock_Exam_2025.pdf' | relative_url }}" class="btn btn-solution">Solution</a>
        </div>
      </div>

      <div class="assessment-card">
        <h3>Final Exam 2025</h3>
        <p>End of term examination.</p>
        <div class="assessment-links">
          <a href="{{ '/Exams/Exam_2025.pdf' | relative_url }}" class="btn">Exam</a>
          <a href="{{ '/Exams/Solution_Exam_2025.pdf' | relative_url }}" class="btn btn-solution">Solution</a>
        </div>
      </div>
    </div>
  </section>

  <section>
    <h2>Weekly Quizzes (MCQs)</h2>
    <p>Short multiple-choice quizzes to test your understanding of each lecture.</p>

    <table class="quiz-table">
      <thead>
        <tr>
          <th>Lecture</th>
          <th>Topic</th>
          <th>Quiz</th>
          <th>Solution</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1</td>
          <td>Introduction to Systematic Strategies</td>
          <td>
            <a href="https://forms.gle/RDyctQvfY5unEbKH8">Online</a> |
            <a href="{{ '/Quiz/Quiz_1.pdf' | relative_url }}">PDF</a>
          </td>
          <td><a href="{{ '/Solution_Quiz/Solution_Quiz_1.pdf' | relative_url }}">Solution</a></td>
        </tr>
        <tr>
          <td>2</td>
          <td>Unsupervised Learning Techniques</td>
          <td>
            <a href="https://forms.gle/QHC3meaZr6bPYqej9">Online</a> |
            <a href="{{ '/Quiz/Quiz_2.pdf' | relative_url }}">PDF</a>
          </td>
          <td><a href="{{ '/Solution_Quiz/Solution_Quiz_2.pdf' | relative_url }}">Solution</a></td>
        </tr>
        <tr>
          <td>3</td>
          <td>Latent Variable Models & Regime Detection</td>
          <td>
            <a href="https://forms.gle/eWUYm7mr1JH3ULSG8">Online</a> |
            <a href="{{ '/Quiz/Quiz_3.pdf' | relative_url }}">PDF</a>
          </td>
          <td><a href="{{ '/Solution_Quiz/Solution_Quiz_3.pdf' | relative_url }}">Solution</a></td>
        </tr>
        <tr>
          <td>4</td>
          <td>Supervised Learning Algorithms</td>
          <td>
            <a href="https://forms.gle/K7SBmjxmxXHiiw1a9">Online</a> |
            <a href="{{ '/Quiz/Quiz_4.pdf' | relative_url }}">PDF</a>
          </td>
          <td><a href="{{ '/Solution_Quiz/Solution_Quiz_4.pdf' | relative_url }}">Solution</a></td>
        </tr>
        <tr>
          <td>5</td>
          <td>Enhancing Strategy Performance</td>
          <td colspan="2" class="na">Programming Session - No Quiz</td>
        </tr>
        <tr>
          <td>6</td>
          <td>Variable Selection Networks</td>
          <td colspan="2" class="na">Programming Session - No Quiz</td>
        </tr>
        <tr>
          <td>7</td>
          <td>Temporal Fusion Transformers</td>
          <td>
            <a href="https://forms.gle/Uoh4Vj4Zq8oG4nde8">Online</a> |
            <a href="{{ '/Quiz/Quiz_7.pdf' | relative_url }}">PDF</a>
          </td>
          <td><a href="{{ '/Solution_Quiz/Solution_Quiz_7.pdf' | relative_url }}">Solution</a></td>
        </tr>
      </tbody>
    </table>
  </section>
</article>
