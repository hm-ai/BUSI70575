# **Instructions

## **Global Instructions (apply to all pages)**

* Fix the layout issue: widen paragraph containers. The theme’s CSS makes text too narrow; override it with a wider `max-width` or container style.

---

## **Instructions for `@index.md`**

* Insert the logo **immediately before** the title “Systematic Trading…”.
* Remove the entire **Getting Started** section from this page.
* Add a clear explanation of the **Course Structure** using this exact breakdown:

  * 8 Lectures
  * 8 Programming Sessions
  * Weekly MCQs
  * 4 Optional Sessions (Refresher + advanced ML topics)
  * 1 Coursework (Competition)
  * 1 Final Exam (written, one page allowed)

* Explicitly state that the **Competition is done in groups of 3–4 students**.
* State that **Weekly quizzes do not count toward the final mark**.
* Add a **table of assessments weights**:

  * 50 percent Competition
  * 50 percent Final Exam

---

## **Instructions for the Syllabus Page**

### **Restructure the syllabus**

* Replace the word **Lectures** with **Sessions** everywhere.
* Format them as:

  * Session 1: Introduction to Systematic Strategies with Machine Learning
  * Session 2: Introduction to Unsupervised Learning Techniques
  * Session 3: Latent Variable Models in Financial Asset Regime Detection
  * Session 4: Supervised Learning Algorithms
  * Session 5: Project – Enhancing Strategy Performance in Crypto Markets
  * Session 6: Introducing Variable Selection Networks
  * Session 7: Neural Networks for Interpretable Time Series Forecasting
  * Session 8: Volatility Forecasting with Temporal Fusion Transformers
  * Session 9: Review Session – Mock Exam

* Set `date:` to **“coming soon”** for all sessions.
* Remove the **Q and A session** entirely.

### **Add Optional Sessions (in the same page, separated clearly)**

* Optional Session 1: Probability and Calculus Refresher
* Optional Session 2: Introduction to Deep Generative Models
* Optional Session 3: Introduction to Graph Neural Networks
* Optional Session 4: Introduction to LLMs

---

## **New Page: Student Progress Tracker**

Create one dedicated page where students can self-assess their understanding for **every session**.

### **Purpose**

* Students enter:

  * Name
  * Confidence: `I feel confident` / `I am struggling`
  * Optional question
* Data goes to **one single Google Form**, stored in a private Google Sheet.
* No results are displayed on the site.

### **Header text**

Include:

* Explanation of how the page works
* Clarify that responses are **not anonymous**, but visible only to the instructor
* Clarify that this is for **learning support**, not grading

### **Layout**

* Display a structured list of all Sessions (1–9).
* For each session:

  * Show the session title
  * Add a line: “Submit your confidence and any question for this session:”
  * Add **one button** linking to the **prefilled Google Form URL** for that session
* Keep everything on **one page**.

### **Prefilled Google Form integration**

* Use one base Google Form prefilled URL (from “Get pre-filled link”).
* Replace the `Session` field value in the query string for each session.
* URL-encode titles correctly.
* Use these URLs as the `href` for each session’s “Submit feedback” button.

### **Privacy Requirements**

* Do not show response data.
* Do not embed Google Sheets or summaries.
* No counts, no leaderboards, no visualizations.

### **UX Requirements**

* Links open in a new tab.
* Buttons visually consistent.
* Optional grouping by weeks permitted, but all sessions must remain on this one page.

---

## **Instructions for Assessments Page**

* Create a **Weekly Quizzes** section following the same structure as the Sessions 1–9 list.

  * If quiz content exists, insert it.
  * Otherwise leave placeholders (empty, ready to fill).

* Add three sections:
  **Mock Exams**, **Final Exams**, **Coursework**
  Structured by academic year:

  * **2024/2025**
  * **2025/2026: coming soon**

---

## **Instructions for Resources**

* Move the **Contact** section to the **end of `@index.md`**.

* Move the **Getting Started** section into **`@programming.md` as the first section**.

* In `@index.md`, build an **Office Hours table** and add an office hour immediately after each Session 1–9.

  * Leave all time/date/location cells as “coming soon”.

* In the **Resources** page:

  * Structure downloadable PDFs under two headings only:

    * **Optional Sessions**
    * **Lectures**
  * No additional categories.

---

## **New Page: Coursework**

### **Page structure**

1. **Overview**

   * 2–3 sentences explaining that the coursework is a competition where students submit a prediction file and code.

2. **Key Information**

   * Competition link (coming soon)
   * Deadline (coming soon)

3. **Task Description**

   * Placeholder: coming soon

4. **Dataset**

   * Placeholder: coming soon

5. **Evaluation**

   * Placeholder: coming soon

6. **Getting Started**

   * Links to:

     * Join competition
     * Starter notebook
     * Baseline model

7. **Submission Rules**

   * Daily submission limits
   * One team account
   * Documentation expectations
   * Academic integrity rules

8. **Deliverables**

   * Code repository / notebook
   * Submission file

---

If you want, I can package this into a single `.md` ready to paste into Claude.




