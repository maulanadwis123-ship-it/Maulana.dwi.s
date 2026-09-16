<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <meta name="description"
        content="Professional Portfolio Maulana Dwi Saputro — Internal Audit, Dealer Finance & CF Audit, Risk & Compliance.">

  <title>Maulana Dwi Saputro | Internal Audit Portfolio</title>

  <style>
    :root {
      --bg: #090b0e;
      --card: #12161b;
      --card2: #171c22;
      --line: #282f37;
      --text: #f4f1e9;
      --muted: #9ba3ad;
      --gold: #c9a96b;
      --gold-light: #e1c58b;
      --green: #7fa889;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      background: var(--bg);
      color: var(--text);
      font-family: Inter, Arial, Helvetica, sans-serif;
      line-height: 1.7;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    .container {
      width: min(1160px, 92%);
      margin: auto;
    }

    /* ================= NAVBAR ================= */

    nav {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(9, 11, 14, 0.88);
      backdrop-filter: blur(18px);
      border-bottom: 1px solid rgba(255,255,255,.06);
    }

    .nav-inner {
      height: 70px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-size: 14px;
      font-weight: 800;
      letter-spacing: .15em;
    }

    .logo span {
      color: var(--gold);
    }

    .nav-links {
      display: flex;
      gap: 25px;
      color: var(--muted);
      font-size: 12px;
    }

    .nav-links a {
      transition: .25s;
    }

    .nav-links a:hover {
      color: var(--gold-light);
    }

    /* ================= HERO ================= */

    .hero {
      padding: 90px 0 65px;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.35fr .85fr;
      gap: 30px;
      align-items: stretch;
    }

    .eyebrow {
      color: var(--gold);
      text-transform: uppercase;
      letter-spacing: .2em;
      font-size: 11px;
      font-weight: 700;
    }

    .hero h1 {
      font-size: clamp(48px, 7vw, 86px);
      line-height: .96;
      letter-spacing: -.06em;
      margin: 18px 0 25px;
    }

    .hero h1 span {
      color: var(--gold);
    }

    .hero-description {
      color: var(--muted);
      max-width: 720px;
      font-size: 16px;
    }

    .buttons {
      display: flex;
      flex-wrap: wrap;
      gap: 11px;
      margin-top: 30px;
    }

    .button {
      padding: 12px 18px;
      border: 1px solid var(--line);
      border-radius: 10px;
      font-size: 12px;
      transition: .25s;
    }

    .button:hover {
      border-color: var(--gold);
      transform: translateY(-2px);
    }

    .button-primary {
      background: var(--gold);
      color: #111;
      border-color: var(--gold);
      font-weight: 800;
    }

    /* ================= STATS ================= */

    .stats {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 12px;
    }

    .stat {
      min-height: 145px;
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
      padding: 23px;
      border: 1px solid var(--line);
      border-radius: 18px;
      background:
        linear-gradient(145deg, var(--card), var(--card2));
    }

    .stat-number {
      font-size: 31px;
      font-weight: 800;
      letter-spacing: -.04em;
    }

    .stat-label {
      color: var(--muted);
      font-size: 11px;
      margin-top: 4px;
    }

    /* ================= SECTION ================= */

    section {
      padding: 65px 0;
    }

    .section-header {
      display: flex;
      justify-content: space-between;
      align-items: end;
      gap: 30px;
      margin-bottom: 27px;
    }

    .section-number {
      color: var(--gold);
      text-transform: uppercase;
      letter-spacing: .18em;
      font-size: 11px;
      font-weight: 700;
    }

    h2 {
      font-size: 34px;
      line-height: 1.1;
      letter-spacing: -.04em;
      margin-top: 5px;
    }

    .section-description {
      max-width: 520px;
      color: var(--muted);
      font-size: 13px;
    }

    /* ================= CARD ================= */

    .card {
      background:
        linear-gradient(145deg, var(--card), var(--card2));
      border: 1px solid var(--line);
      border-radius: 18px;
      padding: 26px;
    }

    .card h3 {
      font-size: 18px;
      margin-bottom: 10px;
    }

    .card p {
      color: var(--muted);
      font-size: 13px;
    }

    .two-column {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 16px;
    }

    /* ================= TAGS ================= */

    .tags {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin-top: 18px;
    }

    .tag {
      border: 1px solid var(--line);
      border-radius: 50px;
      padding: 7px 11px;
      color: #cdd2d8;
      font-size: 10px;
    }

    /* ================= AUDIT SCOPE ================= */

    .audit-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 14px;
    }

    .audit-card {
      min-height: 240px;
      position: relative;
      overflow: hidden;
    }

    .audit-number {
      color: var(--gold);
      font-size: 11px;
      font-weight: 800;
      letter-spacing: .1em;
    }

    .audit-card h3 {
      margin-top: 14px;
    }

    .audit-card ul {
      margin-top: 12px;
      padding-left: 17px;
    }

    .audit-card li {
      color: var(--muted);
      font-size: 12px;
      margin-bottom: 5px;
    }

    /* ================= APPROACH ================= */

    .approach {
      margin-top: 17px;
    }

    .flow {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 8px;
      margin-top: 20px;
    }

    .flow-item {
      padding: 10px 13px;
      border: 1px solid var(--line);
      border-radius: 9px;
      color: #ddd;
      font-size: 11px;
      background: rgba(255,255,255,.02);
    }

    .arrow {
      color: var(--gold);
    }

    .quote {
      border-left: 2px solid var(--gold);
      padding-left: 17px;
      margin-top: 22px;
      color: #ddd;
      font-size: 15px;
    }

    /* ================= RISK ================= */

    .risk-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 10px;
      margin-top: 18px;
    }

    .risk {
      padding: 15px;
      border: 1px solid var(--line);
      border-radius: 12px;
      color: #d7dbe0;
      font-size: 12px;
      text-align: center;
      background: rgba(255,255,255,.015);
    }

    /* ================= JOURNEY ================= */

    .timeline {
      position: relative;
    }

    .trip {
      display: grid;
      grid-template-columns: 60px 18px 1fr;
      gap: 14px;
      padding: 17px 0;
    }

    .trip-year {
      color: var(--gold);
      font-size: 12px;
      font-weight: 800;
    }

    .trip-dot {
      width: 9px;
      height: 9px;
      margin-top: 7px;
      border-radius: 50%;
      background: var(--gold);
    }

    .trip h3 {
      font-size: 16px;
      margin-bottom: 2px;
    }

    .trip p {
      margin: 0;
    }

    /* ================= CASE STUDY ================= */

    .case-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 16px;
    }

    .case-label {
      color: var(--gold);
      text-transform: uppercase;
      letter-spacing: .15em;
      font-size: 10px;
      font-weight: 700;
    }

    .case-card ul {
      padding-left: 18px;
      margin-top: 13px;
    }

    .case-card li {
      color: var(--muted);
      font-size: 13px;
      margin-bottom: 7px;
    }

    /* ================= CAREER ================= */

    .career-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 14px;
    }

    .career-card {
      min-height: 170px;
    }

    .career-label {
      color: var(--gold);
      text-transform: uppercase;
      letter-spacing: .15em;
      font-size: 10px;
    }

    /* ================= FOOTER ================= */

    footer {
      border-top: 1px solid var(--line);
      padding: 35px 0 50px;
      color: var(--muted);
      font-size: 11px;
    }

    .footer-inner {
      display: flex;
      justify-content: space-between;
      gap: 15px;
      flex-wrap: wrap;
    }

    /* ================= MOBILE ================= */

    @media (max-width: 850px) {

      .hero-grid,
      .two-column,
      .case-grid {
        grid-template-columns: 1fr;
      }

      .audit-grid {
        grid-template-columns: 1fr 1fr;
      }

      .career-grid {
        grid-template-columns: 1fr 1fr;
      }

      .nav-links {
        display: none;
      }

      .section-header {
        display: block;
      }

      .section-description {
        margin-top: 12px;
      }
    }

    @media (max-width: 560px) {

      .container {
        width: 92%;
      }

      .hero {
        padding-top: 55px;
      }

      .hero h1 {
        font-size: 49px;
      }

      .stats,
      .audit-grid,
      .career-grid,
      .risk-grid {
        grid-template-columns: 1fr;
      }

      .flow {
        display: block;
      }

      .flow-item {
        margin-bottom: 6px;
        display: inline-block;
      }

      .arrow {
        display: none;
      }
    }
  </style>
</head>

<body>

<!-- ================= NAVBAR ================= -->

<nav>
  <div class="container nav-inner">

    <div class="logo">
      MAULANA<span>.</span>
    </div>

    <div class="nav-links">
      <a href="#profile">Profile</a>
      <a href="#audit">Audit</a>
      <a href="#journey">Journey</a>
      <a href="#case-study">Case Study</a>
      <a href="#career">Career</a>
    </div>

  </div>
</nav>


<!-- ================= HERO ================= -->

<header class="hero">

  <div class="container hero-grid">

    <div>

      <div class="eyebrow">
        Internal Audit · Risk · Compliance
      </div>

      <h1>
        Audit from<br>
        <span>data to field.</span>
      </h1>

      <p class="hero-description">
        Professional portfolio Maulana Dwi Saputro —
        pengalaman Internal Audit pada perusahaan multifinance
        dengan fokus pada Dealer Finance & Consumer Financing,
        operational risk, asset verification, compliance,
        dan identifikasi indikasi fraud.
      </p>

      <div class="buttons">

        <a href="#audit" class="button button-primary">
          Explore Audit Experience
        </a>

        <a href="#journey" class="button">
          View Field Journey
        </a>

      </div>

    </div>


    <div class="stats">

      <div class="stat">
        <div class="stat-number">83+</div>
        <div class="stat-label">
          Branch Exposure
        </div>
      </div>

      <div class="stat">
        <div class="stat-number">29</div>
        <div class="stat-label">
          Completed Assignments
        </div>
      </div>

      <div class="stat">
        <div class="stat-number">2024–26</div>
        <div class="stat-label">
          Field Journey
        </div>
      </div>

      <div class="stat">
        <div class="stat-number">QIA</div>
        <div class="stat-label">
          Professional Certification
        </div>
      </div>

    </div>

  </div>

</header>


<!-- ================= PROFILE ================= -->

<section id="profile">

  <div class="container">

    <div class="section-header">

      <div>
        <div class="section-number">
          01 / Profile
        </div>

        <h2>
          Built in the field.
        </h2>
      </div>

      <p class="section-description">
        Audit bukan sekadar menemukan kesalahan,
        tetapi memahami akar masalah, dampak,
        risiko, dan bagaimana kontrol dapat diperkuat.
      </p>

    </div>


    <div class="two-column">

      <div class="card">

        <h3>
          Professional Overview
        </h3>

        <p>
          Memiliki pengalaman dalam Internal Audit pada perusahaan
          multifinance dengan exposure terhadap branch operations,
          Dealer Finance & Consumer Financing, credit financing,
          asset & inventory, SOP compliance, physical verification,
          risk identification, dan audit follow-up.
        </p>

        <p style="margin-top:14px;">
          Terbiasa menghubungkan data sistem, dokumen,
          transaksi, kondisi fisik, dan hasil konfirmasi
          untuk menghasilkan risk assessment yang lebih menyeluruh.
        </p>

      </div>


      <div class="card">

        <h3>
          Core Skills
        </h3>

        <div class="tags">

          <span class="tag">Internal Audit</span>
          <span class="tag">Dealer Finance & CF</span>
          <span class="tag">Operational Risk</span>
          <span class="tag">Fraud Investigation</span>
          <span class="tag">Asset Verification</span>
          <span class="tag">Inventory</span>
          <span class="tag">Data Analysis</span>
          <span class="tag">SOP Review</span>
          <span class="tag">Root Cause Analysis</span>
          <span class="tag">Audit Follow-up</span>
          <span class="tag">QIA</span>
          <span class="tag">Multifinance Auditor</span>

        </div>

      </div>

    </div>

  </div>

</section>


<!-- ================= AUDIT ================= -->

<section id="audit">

  <div class="container">

    <div class="section-header">

      <div>
        <div class="section-number">
          02 / Audit Experience
        </div>

        <h2>
          Dealer Finance & CF Audit
        </h2>
      </div>

      <p class="section-description">
        Risk-based examination dari proses pembiayaan,
        aktivitas dealer, kualitas portfolio,
        hingga verifikasi unit secara fisik.
      </p>

    </div>


    <div class="audit-grid">


      <!-- 01 -->

      <div class="card audit-card">

        <div class="audit-number">
          01 / DEALER
        </div>

        <h3>
          Dealer & Showroom Review
        </h3>

        <ul>

          <li>
            Evaluasi aktivitas dan kualitas kerja sama dealer.
          </li>

          <li>
            Review histori pencairan dan pola pembiayaan.
          </li>

          <li>
            Evaluasi kepatuhan terhadap SOP.
          </li>

          <li>
            Identifikasi aktivitas pembiayaan tidak wajar.
          </li>

          <li>
            Review kondisi showroom dan unit.
          </li>

          <li>
            Follow-up temuan audit sebelumnya.
          </li>

        </ul>

      </div>


      <!-- 02 -->

      <div class="card audit-card">

        <div class="audit-number">
          02 / FINANCING
        </div>

        <h3>
          Credit & Financing Process
        </h3>

        <ul>

          <li>
            Review proses pengajuan hingga pencairan.
          </li>

          <li>
            Pemeriksaan kesesuaian data dan dokumen.
          </li>

          <li>
            Review plafond, tenor, DP dan pembayaran.
          </li>

          <li>
            Identifikasi penggunaan plafond tidak sesuai.
          </li>

          <li>
            Review repeat disbursement.
          </li>

          <li>
            Identifikasi credit risk.
          </li>

        </ul>

      </div>


      <!-- 03 -->

      <div class="card audit-card">

        <div class="audit-number">
          03 / PHYSICAL
        </div>

        <h3>
          Physical Unit Verification
        </h3>

        <ul>

          <li>
            Verifikasi keberadaan unit.
          </li>

          <li>
            Pencocokan data dengan kondisi aktual.
          </li>

          <li>
            Pemeriksaan RO, foto dan odometer.
          </li>

          <li>
            Pemeriksaan nomor rangka.
          </li>

          <li>
            Identifikasi unit tidak standby.
          </li>

          <li>
            Evaluasi risiko recovery.
          </li>

        </ul>

      </div>


      <!-- 04 -->

      <div class="card audit-card">

        <div class="audit-number">
          04 / COMPLIANCE
        </div>

        <h3>
          Document & Legal Compliance
        </h3>

        <ul>

          <li>
            Review kelengkapan dokumen pembiayaan.
          </li>

          <li>
            Pemeriksaan fidusia.
          </li>

          <li>
            Review BPKB dan asuransi.
          </li>

          <li>
            Review ketentuan internal.
          </li>

          <li>
            Pemeriksaan kesesuaian SOP.
          </li>

          <li>
            Identifikasi dokumen tidak konsisten.
          </li>

        </ul>

      </div>


      <!-- 05 -->

      <div class="card audit-card">

        <div class="audit-number">
          05 / PORTFOLIO
        </div>

        <h3>
          Portfolio & Collection Risk
        </h3>

        <ul>

          <li>
            Review kualitas pembiayaan.
          </li>

          <li>
            Analisis SLIK dan histori pembayaran.
          </li>

          <li>
            Identifikasi risiko delinquency/NPL.
          </li>

          <li>
            Review tunggakan.
          </li>

          <li>
            Evaluasi potensi recovery.
          </li>

          <li>
            Early warning terhadap account berisiko.
          </li>

        </ul>

      </div>


      <!-- 06 -->

      <div class="card audit-card">

        <div class="audit-number">
          06 / FRAUD
        </div>

        <h3>
          Fraud & Irregularity Detection
        </h3>

        <ul>

          <li>
            Identifikasi indikasi manipulasi data.
          </li>

          <li>
            Review rekening pihak lain/rekening bayangan.
          </li>

          <li>
            Identifikasi potensi penyalahgunaan plafond.
          </li>

          <li>
            Review transaksi tidak sesuai profil dealer.
          </li>

          <li>
            Pemeriksaan indikasi dokumen tidak sesuai.
          </li>

          <li>
            Konfirmasi kepada pihak terkait.
          </li>

        </ul>

      </div>

    </div>


    <!-- AUDIT APPROACH -->

    <div class="card approach">

      <div class="section-number">
        Audit Approach
      </div>

      <div class="flow">

        <span class="flow-item">
          System Data
        </span>

        <span class="arrow">→</span>

        <span class="flow-item">
          Documents
        </span>

        <span class="arrow">→</span>

        <span class="flow-item">
          Transaction
        </span>

        <span class="arrow">→</span>

        <span class="flow-item">
          Physical Verification
        </span>

        <span class="arrow">→</span>

        <span class="flow-item">
          Confirmation
        </span>

        <span class="arrow">→</span>

        <span class="flow-item">
          Risk Assessment
        </span>

      </div>

      <div class="quote">
        Pendekatan audit tidak hanya menilai kelengkapan dokumen,
        tetapi membandingkan data, transaksi, dokumen, kondisi fisik,
        dan aktivitas bisnis di lapangan.
      </div>

    </div>


    <!-- RISK PERSPECTIVE -->

    <div style="margin-top:28px;">

      <div class="section-number">
        Risk-Based Audit Perspective
      </div>

      <div class="risk-grid">

        <div class="risk">Credit Risk</div>
        <div class="risk">Fraud Risk</div>
        <div class="risk">Operational Risk</div>
        <div class="risk">Compliance Risk</div>
        <div class="risk">Asset Risk</div>
        <div class="risk">Dealer Risk</div>
        <div class="risk">Recovery Risk</div>
        <div class="risk">Reputational Risk</div>

      </div>

    </div>

  </div>

</section>


<!-- ================= CORRECTIVE ================= -->

<section>

  <div class="container">

    <div class="section-header">

      <div>

        <div class="section-number">
          Corrective & Preventive
        </div>

        <h2>
          From finding to action.
        </h2>

      </div>

      <p class="section-description">
        Temuan audit diarahkan menjadi rekomendasi yang dapat
        memperbaiki proses sekaligus mencegah risiko berulang.
      </p>

    </div>


    <div class="two-column">

      <div class="card">

        <h3>
          Corrective Action
        </h3>

        <p>
          Perbaikan terhadap kondisi atau kelemahan kontrol
          yang telah ditemukan melalui pemeriksaan.
        </p>

        <div class="tags">

          <span class="tag">Process Improvement</span>
          <span class="tag">Document Validation</span>
          <span class="tag">Audit Follow-up</span>
          <span class="tag">Unit Verification</span>

        </div>

      </div>


      <div class="card">

        <h3>
          Preventive Action
        </h3>

        <p>
          Penguatan kontrol untuk mengurangi kemungkinan
          risiko yang sama terjadi kembali.
        </p>

        <div class="tags">

          <span class="tag">Early Warning</span>
          <span class="tag">Dealer Monitoring</span>
          <span class="tag">Risk Threshold</span>
          <span class="tag">SOP Enhancement</span>

        </div>

      </div>

    </div>

  </div>

</section>


<!-- ================= BUSINESS TRIP ================= -->

<section id="journey">

  <div class="container">

    <div class="section-header">

      <div>

        <div class="section-number">
          03 / Business Trip
        </div>

        <h2>
          Field Journey 2024–2026
        </h2>

      </div>

      <p class="section-description">
        Perjalanan kerja menjadi bagian dari pengalaman memahami
        karakteristik cabang, operasi, dealer, dan risiko secara langsung.
      </p>

    </div>


    <div class="card timeline">


      <div class="trip">

        <div class="trip-year">
          2026
        </div>

        <div class="trip-dot"></div>

        <div>

          <h3>
            Batam · Gorontalo · Manado · Tasikmalaya
          </h3>

          <p>
            Branch audit, operational review,
            physical verification, dan exit meeting.
          </p>

        </div>

      </div>


      <div class="trip">

        <div class="trip-year">
          2025
        </div>

        <div class="trip-dot"></div>

        <div>

          <h3>
            Palu · Jember · Banyuwangi · Surabaya · Bangka
          </h3>

          <p>
            Field audit dan pemeriksaan operasional
            di berbagai karakteristik wilayah.
          </p>

        </div>

      </div>


      <div class="trip">

        <div class="trip-year">
          2025
        </div>

        <div class="trip-dot"></div>

        <div>

          <h3>
            Bogor · Cikarang · Magelang · Bandung ·
            Cirebon · Lubuklinggau · Salatiga
          </h3>

          <p>
            Branch examination, asset verification,
            inventory, dan compliance review.
          </p>

        </div>

      </div>


      <div class="trip">

        <div class="trip-year">
          2024
        </div>

        <div class="trip-dot"></div>

        <div>

          <h3>
            Early Field Experience
          </h3>

          <p>
            Membangun fondasi pengalaman audit dan
            memahami kondisi operasional secara langsung.
          </p>

        </div>

      </div>


    </div>

  </div>

</section>


<!-- ================= CASE STUDY ================= -->

<section id="case-study">

  <div class="container">

    <div class="section-header">

      <div>

        <div class="section-number">
          04 / Case Study
        </div>

        <h2>
          From finding to early warning.
        </h2>

      </div>

      <p class="section-description">
        Pendekatan analitis untuk mengevaluasi risiko dealer,
        portfolio, unit, dan recovery.
      </p>

    </div>


    <div class="case-grid">


      <div class="card case-card">

        <div class="case-label">
          Dealer Risk
        </div>

        <h3>
          Portfolio Concentration & Unit Availability
        </h3>

        <ul>

          <li>
            Review histori repeat disbursement.
          </li>

          <li>
            Analisis kualitas pembayaran.
          </li>

          <li>
            Validasi keberadaan unit secara fisik.
          </li>

          <li>
            Membandingkan data pembiayaan dengan
            kondisi aktual dealer.
          </li>

          <li>
            Evaluasi potensi recovery.
          </li>

        </ul>

      </div>


      <div class="card case-card">

        <div class="case-label">
          Preventive Action
        </div>

        <h3>
          Early Warning Framework
        </h3>

        <ul>

          <li>
            Monitoring repeat disbursement secara berkala.
          </li>

          <li>
            Threshold berdasarkan plafond dan risk exposure.
          </li>

          <li>
            Penguatan maintenance dan unit verification.
          </li>

          <li>
            Escalation terhadap pola transaksi tidak normal.
          </li>

        </ul>

      </div>

    </div>

  </div>

</section>


<!-- ================= CAREER ================= -->

<section id="career">

  <div class="container">

    <div class="section-header">

      <div>

        <div class="section-number">
          05 / Career Journey
        </div>

        <h2>
          Experience with direction.
        </h2>

      </div>

      <p class="section-description">
        Pengalaman audit membentuk perspektif yang dapat
        diterapkan pada risk, compliance, asset management,
        dan operational control.
      </p>

    </div>


    <div class="career-grid">


      <div class="card career-card">

        <div class="career-label">
          Experience
        </div>

        <h3>
          Internal Audit
        </h3>

        <p>
          Multifinance · Branch Audit ·
          Dealer Finance · Risk-Based Audit
        </p>

      </div>


      <div class="card career-card">

        <div class="career-label">
          Focus
        </div>

        <h3>
          Risk & Control
        </h3>

        <p>
          Fraud indicators · Compliance ·
          Physical Verification · Corrective Action
        </p>

      </div>


      <div class="card career-card">

        <div class="career-label">
          Direction
        </div>

        <h3>
          Audit · Risk · Asset
        </h3>

        <p>
          Mengembangkan pengalaman menuju fungsi
          yang lebih luas dan strategic.
        </p>

      </div>


    </div>

  </div>

</section>


<!-- ================= KEY VALUE ================= -->

<section>

  <div class="container">

    <div class="card">

      <div class="section-number">
        Audit Philosophy
      </div>

      <div class="quote">

        “Audit bukan hanya menemukan kesalahan,
        tetapi memahami bagaimana suatu kondisi terjadi,
        seberapa besar risikonya bagi perusahaan,
        dan bagaimana kontrol dapat diperkuat
        agar risiko yang sama tidak berulang.”

      </div>

      <p style="margin-top:18px;">

        Pengalaman Dealer Finance & CF Audit memberikan
        pemahaman mengenai hubungan antara proses pembiayaan,
        aktivitas dealer, kondisi unit, kualitas portfolio,
        operational risk, hingga potensi fraud sehingga
        pemeriksaan dapat dilakukan dengan perspektif
        yang lebih menyeluruh dan berbasis risiko.

      </p>

    </div>

  </div>

</section>


<!-- ================= FOOTER ================= -->

<footer>

  <div class="container footer-inner">

    <div>
      © 2026 Maulana Dwi Saputro
    </div>

    <div>
      Internal Audit · Risk & Compliance · Asset Management
    </div>

  </div>

</footer>


</body>
</html>
