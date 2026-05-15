---
layout: full_width
title: Coursework
permalink: /coursework/
---

<header class="site-header">
  <nav class="site-nav">
    <a href="{{ site.baseurl }}/">Home</a>
    <a href="{{ site.baseurl }}/syllabus/">Syllabus</a>
    <a href="{{ site.baseurl }}/programming/">Programming</a>
    <a href="{{ site.baseurl }}/assessments/">Assessments</a>
    <a href="{{ site.baseurl }}/coursework/">Coursework</a>
    <a href="{{ site.baseurl }}/progress/">Progress Tracker</a>
  </nav>
</header>

<article>
  <div class="header-row">
    <img src="{{ site.baseurl }}/images/logo_alken.png" alt="Alken logo" class="course-logo"/>
    <div class="header-text">
      <h1>Coursework: Competition</h1>
      <p class="subtitle">50% of your final grade</p>
    </div>
  </div>

  <section>
    <h2>Overview</h2>
    <p>This year's coursework asks you to build a <strong>metamodel</strong> on top of a primary trading signal that we provide for <strong>11 instruments across three asset classes</strong>. The metamodel's job is to predict, for each primary signal, the probability that following it would be profitable under a triple-barrier exit rule.</p>
    <p>This is a <strong>group project</strong> completed in teams of <strong>5 students</strong> (26 groups in total). The coursework is marked out of <strong>100</strong>.</p>
  </section>

  <section>
    <h2>Key Information</h2>
    <table>
      <tbody>
        <tr>
          <td><strong>Deadline</strong></td>
          <td>June 4, 2026</td>
        </tr>
        <tr>
          <td><strong>Team Size</strong></td>
          <td>5 students (26 groups)</td>
        </tr>
        <tr>
          <td><strong>Weight</strong></td>
          <td>50% of final grade</td>
        </tr>
        <tr>
          <td><strong>Marked out of</strong></td>
          <td>100 (with +10 bonus for the optional competition track)</td>
        </tr>
      </tbody>
    </table>
  </section>

  <section>
    <h2>The Universe</h2>
    <p>You are provided with the primary model's daily signals (-1, 0, +1) for the following 11 instruments.</p>

    <h3>Equity Index Futures</h3>
    <table>
      <thead>
        <tr><th>Ticker</th><th>Index</th></tr>
      </thead>
      <tbody>
        <tr><td><strong>ES1S</strong></td><td>S&amp;P 500</td></tr>
        <tr><td><strong>NQ1S</strong></td><td>Nasdaq 100</td></tr>
        <tr><td><strong>FESX1S</strong></td><td>Euro Stoxx 50</td></tr>
      </tbody>
    </table>

    <h3>Energy</h3>
    <table>
      <thead>
        <tr><th>Ticker</th><th>Commodity</th></tr>
      </thead>
      <tbody>
        <tr><td><strong>CL1S</strong></td><td>WTI Crude Oil</td></tr>
        <tr><td><strong>HO1S</strong></td><td>Heating Oil</td></tr>
        <tr><td><strong>RB1S</strong></td><td>RBOB Gasoline</td></tr>
        <tr><td><strong>NG1S</strong></td><td>Natural Gas</td></tr>
      </tbody>
    </table>

    <h3>Metals</h3>
    <table>
      <thead>
        <tr><th>Ticker</th><th>Metal</th></tr>
      </thead>
      <tbody>
        <tr><td><strong>GC1S</strong></td><td>Gold</td></tr>
        <tr><td><strong>SI1S</strong></td><td>Silver</td></tr>
        <tr><td><strong>HG1S</strong></td><td>Copper</td></tr>
        <tr><td><strong>PL1S</strong></td><td>Platinum</td></tr>
      </tbody>
    </table>

    <p>You are required to cover <strong>at least one full asset class</strong>. Covering more (up to all 11 instruments) is optional.</p>
  </section>

  <section>
    <h2>Task Description</h2>
    <p>Build a metamodel for each instrument you cover. The metamodel takes the primary signal plus your features and outputs a <strong>probability in [0, 1]</strong> that the bet is worth taking.</p>

    <p>The pipeline is:</p>
    <ol>
      <li>Feature engineering from OHLCV (and anything else you can derive)</li>
      <li>Labeling via the <strong>triple-barrier method</strong>, as taught in the course</li>
      <li>Training and comparing several ML models with hyperparameter tuning</li>
      <li>Feature importance analysis at the cluster level</li>
      <li>Evaluation on a clean out-of-sample period</li>
      <li>(Optional) Strategy construction on top of the metamodel probabilities</li>
    </ol>

    <h3>Marking Scheme</h3>
    <table>
      <thead>
        <tr><th>Section</th><th>Marks</th></tr>
      </thead>
      <tbody>
        <tr><td>Feature Engineering</td><td>20</td></tr>
        <tr><td>Labeling (Triple-Barrier Method)</td><td>20</td></tr>
        <tr><td>Model Development and Comparison</td><td>30</td></tr>
        <tr><td>Feature Importance Analysis (Cluster-Level)</td><td>10</td></tr>
        <tr><td>Model Evaluation</td><td>20</td></tr>
        <tr><td><strong>Total</strong></td><td><strong>100</strong></td></tr>
        <tr><td>Optional: Strategy Construction (Competition)</td><td>+10 bonus</td></tr>
      </tbody>
    </table>
    <p>The bonus is capped so the final mark does not exceed 100.</p>

    <h3>1. Feature Engineering (20 marks) 📊</h3>
    <p>Build a rich feature set drawing on the techniques covered in the course:</p>
    <ul>
      <li>Technical indicators</li>
      <li>Latent variable models (GMM, HMM)</li>
      <li>Any of the unsupervised learning methods we discussed</li>
      <li>Anything else you can justify</li>
    </ul>
    <p><strong>Be as creative as possible.</strong> Document what each feature is meant to capture.</p>

    <h3>2. Labeling: Triple-Barrier Method (20 marks) 🏷️</h3>
    <p>Apply the triple-barrier method as taught in the course. You must justify your choice of barrier widths and time-limit.</p>

    <h3>3. Model Development and Comparison (30 marks) 🤖</h3>
    <p>We expect <strong>at least three models with hyperparameter tuning</strong>, drawn from across the three families:</p>
    <ul>
      <li><strong>Linear models</strong> (e.g. Logistic Regression with regularization)</li>
      <li><strong>Tree-based models</strong> (e.g. Random Forest, XGBoost, LightGBM)</li>
      <li><strong>Neural networks</strong> (e.g. Variable Selection Network or Sequential Neural Networks)</li>
    </ul>
    <p>Present a clear comparison: which model wins, on which metric, and why you think so.</p>

    <h3>4. Feature Importance Analysis: Cluster-Level (10 marks) 🔍</h3>
    <p>Beyond per-feature importance, compute importance at the <strong>cluster level</strong>:</p>
    <ul>
      <li>Cluster correlated features together</li>
      <li>Apply MDI, MDA, or SHAP at the cluster level</li>
      <li>Discuss which feature groups drive your metamodel</li>
    </ul>

    <h3>5. Model Evaluation (20 marks) 📈</h3>
    <p>Evaluate on an out-of-sample period that you carve out cleanly from the training period.</p>
    <ul>
      <li>Classification metrics: precision, recall, F1, AUC</li>
      <li>Confusion matrix and decision-threshold analysis</li>
      <li><strong>Per-instrument breakdown</strong> (the metamodel may help on some instruments and not others, say so)</li>
      <li>Comparison against a baseline that follows the primary signal blindly</li>
    </ul>

    <h3>Optional: Strategy Construction, Competition Track (10 bonus marks) 💹</h3>
    <p>For groups that want to compete: use the metamodel probabilities to build a position-sizing strategy on top of the primary signal, either on a single asset class or on the full 11-instrument universe.</p>
    <p><strong>Full constraints (position limits, gross/net exposure, rebalancing rules, target volatility) will be released on Wednesday 20 May.</strong></p>
    <p>Backtest metrics to report:</p>
    <ul>
      <li>CAGR</li>
      <li>Annualised volatility</li>
      <li>Sharpe ratio</li>
      <li>Sortino ratio</li>
      <li>Maximum drawdown</li>
      <li>Average holding period</li>
      <li>Turnover</li>
    </ul>
  </section>

  <section>
    <h2>Dataset</h2>
    <p>Two CSV files are available on <strong>Insendi under Coursework</strong>:</p>

    <h3><code>ohlcv_data.csv</code></h3>
    <p>Daily OHLCV history for all 11 instruments. One row per (instrument, date).</p>
    <table>
      <thead>
        <tr><th>Column</th><th>Description</th></tr>
      </thead>
      <tbody>
        <tr><td><code>date</code></td><td>Trading date (YYYY-MM-DD)</td></tr>
        <tr><td><code>instrument</code></td><td>Lowercase ticker (e.g. <code>cl1s</code>, <code>es1s</code>, <code>gc1s</code>)</td></tr>
        <tr><td><code>open</code>, <code>high</code>, <code>low</code>, <code>close</code></td><td>Continuous-contract prices</td></tr>
        <tr><td><code>volume</code></td><td>Daily volume</td></tr>
        <tr><td><code>open_interest</code></td><td>Daily open interest</td></tr>
      </tbody>
    </table>
    <p>History starts in 1990 for most instruments. Equity Index futures start later: ES1S in 1997, FESX1S in 1998, NQ1S in 1999.</p>

    <h3><code>primary_signals.csv</code></h3>
    <p>Daily primary model signals from January 2020 onwards. One row per date, one column per instrument.</p>
    <table>
      <thead>
        <tr><th>Column</th><th>Description</th></tr>
      </thead>
      <tbody>
        <tr><td><code>date</code></td><td>Trading date (YYYY-MM-DD)</td></tr>
        <tr><td><code>es1s</code>, <code>nq1s</code>, ..., <code>pl1s</code></td><td>Primary signal in {-1, 0, +1}</td></tr>
      </tbody>
    </table>
    <p>The signal convention is:</p>
    <ul>
      <li><code>+1</code>: the primary model wants to go <strong>long</strong> that day</li>
      <li><code>-1</code>: the primary model wants to go <strong>short</strong> that day</li>
      <li><code>0</code>: no position taken by the primary model</li>
    </ul>
    <p><strong>Important.</strong> The data we release covers up to <strong>30 June 2022</strong>. The final <strong>6 months</strong> of data (July to December 2022) are held out and will be used as a hidden test set to evaluate your final submission.</p>
  </section>

  <section>
    <h2>Evaluation</h2>
    <p>You will be judged on:</p>
    <ol>
      <li>Quality and creativity of your feature engineering 💡</li>
      <li>Rigour of your labeling and validation protocol 🛡️</li>
      <li>Appropriateness of your model selection and comparison 🧠</li>
      <li>Critical analysis of your results 🔬</li>
      <li>Code quality, reproducibility, and documentation 📝</li>
    </ol>
    <p><strong>The score is focused entirely on methodology, not on performance.</strong> You can score a high mark even if your metamodel does not beat the primary signal.</p>
    <p>🌟🌟🌟 The best submission, judged on <strong>quality of research</strong> rather than performance, will be <strong>presented to the research team at Alken Asset Management, with an interview for an internship at the end of it.</strong></p>
  </section>

  <section>
    <h2>Getting Started</h2>
    <div class="resource-card">
      <h3>OHLCV Data</h3>
      <p>Download <code>ohlcv_data.csv</code> from the Coursework folder on Insendi.</p>
    </div>
    <div class="resource-card">
      <h3>Primary Signals</h3>
      <p>Download <code>primary_signals.csv</code> from the Coursework folder on Insendi.</p>
    </div>
    <div class="resource-card">
      <h3>Programming Sessions</h3>
      <p>For implementation guidance, refer to <strong>all programming sessions and optional programming sessions</strong> of the course.</p>
    </div>
  </section>

  <section>
    <h2>Submission Rules</h2>
    <ul>
      <li><strong>Group size:</strong> 5 students per group, 26 groups in total</li>
      <li><strong>One submission per group:</strong> a single combined submission</li>
      <li><strong>Documentation:</strong> code must be clean, well-documented and reproducible, your notebook should run end-to-end and produce the deliverable CSV</li>
      <li><strong>Academic integrity:</strong> all work must be original. Plagiarism will result in zero marks and potential disciplinary action.</li>
    </ul>
  </section>

  <section>
    <h2>Deliverables</h2>

    <h3>1. Code</h3>
    <p>A Jupyter notebook or a set of Python files that runs end-to-end and produces the deliverable files below. <strong>Clean, well-documented code is part of the mark.</strong></p>

    <h3>2. Required: Metamodel Predictions</h3>
    <p>A CSV file covering the <strong>first half of 2022</strong> (January to June). We will rerun your code on the hidden second half of 2022 for the final test.</p>
    <p>Format: one row per (date, instrument, prediction).</p>
    <pre><code>date,instrument,prediction
2022-01-03,cl1s,0.74
2022-01-03,es1s,0.51
...</code></pre>
    <ul>
      <li><code>date</code>: trading date (YYYY-MM-DD)</li>
      <li><code>instrument</code>: lowercase ticker</li>
      <li><code>prediction</code>: probability in [0, 1] that the primary signal is worth taking</li>
    </ul>

    <h3>3. Optional: Strategy Weights</h3>
    <p>For groups competing on the strategy track, an additional CSV covering the first half of 2022:</p>
    <pre><code>date,instrument,weight
2022-01-03,cl1s,0.18
2022-01-03,es1s,-0.05
...</code></pre>
    <ul>
      <li><code>weight</code>: signed position weight (positive = long, negative = short)</li>
    </ul>
    <p>Constraints on the weights will be specified on <strong>20 May</strong>.</p>
  </section>

  <section>
    <h2>Contact</h2>
    <p>For any question regarding the coursework: <a href="mailto:h.madmoun@ic.ac.uk">h.madmoun@ic.ac.uk</a></p>
    <p>Good luck and have fun!</p>
  </section>
</article>