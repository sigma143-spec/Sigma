
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>BIO DEFENSE | Molecular Survival Project</title>

  <link rel="stylesheet" href="style.css">

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700;800;900&display=swap" rel="stylesheet">

  <script type="module" src="https://unpkg.com/@splinetool/viewer@1.10.38/build/spline-viewer.js"></script>
</head>

<body>

  <!-- BACKGROUND DECORATIONS -->
  <div class="ambient ambient-one"></div>
  <div class="ambient ambient-two"></div>

  <!-- NAVIGATION -->
  <header class="navbar">

    <div class="brand" onclick="navigate('home')">
      <span class="brand-icon">🌻</span>
      <span>BIO<span class="green">DEFENSE</span></span>
    </div>

    <nav>
      <button class="nav-link active" data-page="home" onclick="navigate('home')">Home</button>
      <button class="nav-link" data-page="missions" onclick="navigate('missions')">Missions</button>
      <button class="nav-link" data-page="database" onclick="navigate('database')">Database</button>
      <button class="nav-link" data-page="quiz" onclick="navigate('quiz')">Challenge</button>
    </nav>

    <div class="status">
      <span class="status-dot"></span>
      SYSTEM ONLINE
    </div>

  </header>


  <!-- ================= HOME ================= -->

  <main>

    <section id="home" class="page active">

      <div class="hero-content">

        <div class="eyebrow">
          <span>✦</span> CONSUMER CHEMISTRY FIELD OPERATIONS
        </div>

        <h1>
          THE MOLECULAR<br>
          <span class="green">SURVIVAL PROJECT</span>
        </h1>

        <p class="hero-description">
          The garden is under attack. Understand the molecules
          that sustain life, investigate their structures, and
          defend the biochemical foundations of living organisms.
        </p>

        <div class="hero-buttons">
          <button class="button-primary" onclick="navigate('missions')">
            START EXPLORATION <span>→</span>
          </button>

          <button class="button-secondary" onclick="navigate('database')">
            OPEN DATABASE
          </button>
        </div>

        <div class="hero-stats">
          <div>
            <strong>03</strong>
            <span>MOLECULAR CLASSES</span>
          </div>

          <div>
            <strong>06</strong>
            <span>FIELD MISSIONS</span>
          </div>

          <div>
            <strong>01</strong>
            <span>FINAL CHALLENGE</span>
          </div>
        </div>

      </div>

      <div class="hero-art">

        <div class="battlefield-label">
          <span class="status-dot"></span>
          BIOLOGICAL DEFENSE ZONE
        </div>

        <div class="hero-emblem">
          <div class="emblem-circle">
            <span>🌻</span>
          </div>

          <div class="orbit orbit-one"></div>
          <div class="orbit orbit-two"></div>

          <div class="floating molecule-float">🧬</div>
          <div class="floating lipid-float">🫒</div>
          <div class="floating shield-float">🛡️</div>
        </div>

        <div class="battlefield-bottom">
          <span>PLANT DEFENSE NETWORK</span>
          <span>SECTOR 01 — ACTIVE</span>
        </div>

        <p class="art-note">
          A biochemical battlefield awaits your investigation.
        </p>

      </div>

    </section>


    <!-- ================= MISSIONS ================= -->

    <section id="missions" class="page">

      <div class="section-heading">
        <div class="eyebrow">FIELD OPERATIONS / 001</div>
        <h1>SELECT YOUR <span class="green">MISSION</span></h1>
        <p>Investigate the fundamental biomolecules of life.</p>
      </div>

      <div class="mission-grid">

        <article class="mission-card protein-card"
          onclick="openTopic('protein')">

          <div class="mission-number">MISSION 01</div>
          <div class="mission-art">🧬</div>

          <h2>PROTEIN PROTOCOL</h2>

          <p>
            Investigate amino acids, peptide bonds,
            structural organization, and biological functions.
          </p>

          <div class="mission-footer">
            <span>STRUCTURE & FUNCTION</span>
            <span>→</span>
          </div>

        </article>


        <article class="mission-card lipid-card"
          onclick="openTopic('lipid')">

          <div class="mission-number">MISSION 02</div>
          <div class="mission-art">🫒</div>

          <h2>LIPID LABORATORY</h2>

          <p>
            Explore energy storage, triglycerides,
            phospholipids, and membrane architecture.
          </p>

          <div class="mission-footer">
            <span>ENERGY & MEMBRANES</span>
            <span>→</span>
          </div>

        </article>


        <article class="mission-card fatty-card"
          onclick="openTopic('fatty')">

          <div class="mission-number">MISSION 03</div>
          <div class="mission-art">🔬</div>

          <h2>FATTY ACID FRONTIER</h2>

          <p>
            Compare saturated and unsaturated fatty acids
            and examine their molecular configurations.
          </p>

          <div class="mission-footer">
            <span>MOLECULAR COMPOSITION</span>
            <span>→</span>
          </div>

        </article>

      </div>

      <div class="mission-note">
        <span>⚠</span>
        Complete the molecular investigations before entering
        the final defense challenge.
      </div>

    </section>


    <!-- ================= DATABASE ================= -->

    <section id="database" class="page">

      <div class="section-heading">
        <div class="eyebrow">RESEARCH ARCHIVE / 002</div>
        <h1>MOLECULAR <span class="green">DATABASE</span></h1>
        <p>Access the biochemical profiles of the three major subjects.</p>
      </div>

      <div class="database-layout">

        <div class="database-menu">

          <button class="database-tab selected"
            onclick="openTopic('protein')">
            🧬 PROTEINS
          </button>

          <button class="database-tab"
            onclick="openTopic('lipid')">
            🫒 LIPIDS
          </button>

          <button class="database-tab"
            onclick="openTopic('fatty')">
            🔬 FATTY ACIDS
          </button>

        </div>

        <div id="topic-display" class="topic-display">

          <div class="topic-placeholder">
            <div>🧪</div>
            <h2>SELECT A BIOCHEMICAL SUBJECT</h2>
            <p>Choose an entry from the molecular database.</p>
          </div>

        </div>

      </div>

    </section>


    <!-- ================= 3D LAB ================= -->

    <section id="lab" class="page">

      <div class="section-heading">
        <div class="eyebrow">INTERACTIVE RESEARCH / 003</div>
        <h1>3D MOLECULAR <span class="green">LABORATORY</span></h1>
        <p>Explore the molecular world through interactive 3D visualization.</p>
      </div>

      <div class="spline-panel">

        <div class="spline-header">
          <span>MOLECULAR VIEWPORT</span>
          <span class="status-dot"></span>
        </div>

        <div class="spline-viewport" id="spline-viewport">

          <div class="spline-placeholder">
            <div>🧬</div>
            <h2>3D LABORATORY INITIALIZING</h2>
            <p>
              Your published Spline scene will appear here.
              Add its embed code to this viewport.
            </p>
          </div>

          <!--
          Replace the placeholder with:

          <spline-viewer
            url="YOUR_SPLINE_SCENE_URL">
          </spline-viewer>

          -->

        </div>

        <div class="spline-footer">
          <span>INTERACTIVE MOLECULAR VISUALIZATION</span>
          <button onclick="navigate('missions')">BACK TO MISSIONS</button>
        </div>

      </div>

    </section>


    <!-- ================= QUIZ ================= -->

    <section id="quiz" class="page">

      <div class="section-heading">
        <div class="eyebrow">FINAL OPERATION / 004</div>
        <h1>THE FINAL <span class="green">DEFENSE</span></h1>
        <p>Test your biochemical knowledge and defend the garden.</p>
      </div>

      <div class="quiz-container">

        <div class="quiz-top">
          <span id="question-count">QUESTION 01 / 05</span>
          <span id="score-display">SCORE: 0</span>
        </div>

        <div class="progress-track">
          <div id="progress-fill"></div>
        </div>

        <div class="quiz-content">

          <div class="quiz-icon">🌻</div>

          <h2 id="question">
            Which type of bond connects amino acids
            in a polypeptide chain?
          </h2>

          <div id="answers" class="answer-grid"></div>

          <div id="feedback" class="feedback"></div>

          <button id="next-button"
            class="button-primary hidden"
            onclick="nextQuestion()">
            NEXT QUESTION →
          </button>

        </div>

      </div>

    </section>

  </main>


  <!-- ================= FOOTER ================= -->

  <footer>
    <div>BIO<span class="green">DEFENSE</span></div>
    <p>CONSUMER CHEMISTRY • BIOCHEMICAL EDUCATION PROJECT</p>
    <span>THE SCIENCE BEHIND THE SURVIVAL OF LIFE.</span>
  </footer>


  <!-- TOPIC MODAL -->

  <div id="topic-modal" class="modal">

    <div class="modal-content">

      <button class="modal-close" onclick="closeModal()">×</button>

      <div id="modal-content"></div>

    </div>

  </div>


  <script src="script.js"></script>

</body>
</html>
# Sigma