<!DOCTYPE html>
<html lang="th">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Australia Visa Document Checklist</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;700&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --au-navy: #00205B;
    --au-red: #C8102E;
    --au-gold: #D4AF37;
    --au-light: #F4F6FA;
    --au-white: #FFFFFF;
    --pending: #94A3B8;
    --inprogress: #F59E0B;
    --done: #10B981;
    --text-main: #1E293B;
    --text-sub: #64748B;
    --border: #E2E8F0;
    --card-shadow: 0 2px 16px rgba(0,32,91,0.08);
    --radius: 14px;
  }
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  body {
    font-family: 'DM Sans', sans-serif;
    background: var(--au-light);
    color: var(--text-main);
    min-height: 100vh;
  }

  /* ===== HEADER ===== */
  .site-header {
    background: linear-gradient(135deg, var(--au-navy) 0%, #001843 100%);
    padding: 0;
    position: sticky;
    top: 0;
    z-index: 100;
    box-shadow: 0 4px 24px rgba(0,0,0,0.18);
  }
  .header-inner {
    max-width: 1100px;
    margin: 0 auto;
    padding: 18px 28px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 16px;
    flex-wrap: wrap;
  }
  .header-brand {
    display: flex;
    align-items: center;
    gap: 14px;
  }
  .flag-badge {
    width: 48px;
    height: 48px;
    border-radius: 50%;
    background: var(--au-red);
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 22px;
    border: 3px solid rgba(255,255,255,0.2);
    flex-shrink: 0;
    overflow: hidden;
  }
  .flag-badge svg { display: block; }
  .header-title { color: #fff; }
  .header-title h1 {
    font-family: 'Playfair Display', serif;
    font-size: 1.35rem;
    font-weight: 700;
    letter-spacing: 0.01em;
    line-height: 1.2;
  }
  .header-title p {
    font-size: 0.75rem;
    color: rgba(255,255,255,0.55);
    margin-top: 2px;
    letter-spacing: 0.06em;
    text-transform: uppercase;
    font-weight: 400;
  }
  .header-meta {
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .header-reset-btn {
    background: rgba(255,255,255,0.08);
    color: rgba(255,255,255,0.7);
    border: 1px solid rgba(255,255,255,0.15);
    border-radius: 8px;
    padding: 7px 16px;
    font-size: 0.78rem;
    font-family: 'DM Sans', sans-serif;
    cursor: pointer;
    transition: all 0.2s;
    letter-spacing: 0.03em;
  }
  .header-reset-btn:hover {
    background: rgba(200,16,46,0.25);
    color: #fff;
    border-color: var(--au-red);
  }

  /* ===== TAB NAV ===== */
  .tab-nav-wrap {
    background: #fff;
    border-bottom: 2px solid var(--border);
    position: sticky;
    top: 85px;
    z-index: 90;
  }
  .tab-nav {
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 28px;
    display: flex;
    gap: 0;
    overflow-x: auto;
    scrollbar-width: none;
  }
  .tab-nav::-webkit-scrollbar { display: none; }
  .tab-btn {
    padding: 14px 22px;
    font-size: 0.82rem;
    font-weight: 500;
    font-family: 'DM Sans', sans-serif;
    color: var(--text-sub);
    border: none;
    background: transparent;
    cursor: pointer;
    border-bottom: 3px solid transparent;
    margin-bottom: -2px;
    white-space: nowrap;
    transition: all 0.2s;
    letter-spacing: 0.02em;
    display: flex;
    align-items: center;
    gap: 7px;
  }
  .tab-btn:hover { color: var(--au-navy); }
  .tab-btn.active {
    color: var(--au-navy);
    border-bottom-color: var(--au-red);
    font-weight: 600;
  }
  .tab-badge {
    background: var(--au-light);
    color: var(--text-sub);
    border-radius: 20px;
    padding: 2px 8px;
    font-size: 0.7rem;
    font-weight: 600;
  }
  .tab-btn.active .tab-badge {
    background: rgba(200,16,46,0.1);
    color: var(--au-red);
  }

  /* ===== MAIN LAYOUT ===== */
  .main-wrap {
    max-width: 1100px;
    margin: 0 auto;
    padding: 28px 28px 60px;
  }
  .tab-panel { display: none; }
  .tab-panel.active { display: block; }

  /* ===== DASHBOARD STATS ===== */
  .dash-stats {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 14px;
    margin-bottom: 24px;
  }
  .stat-card {
    background: #fff;
    border-radius: var(--radius);
    padding: 18px 20px;
    border: 1.5px solid var(--border);
    display: flex;
    flex-direction: column;
    gap: 6px;
    box-shadow: var(--card-shadow);
  }
  .stat-card .stat-label {
    font-size: 0.72rem;
    text-transform: uppercase;
    letter-spacing: 0.07em;
    color: var(--text-sub);
    font-weight: 500;
  }
  .stat-card .stat-value {
    font-size: 2rem;
    font-weight: 700;
    font-family: 'Playfair Display', serif;
    line-height: 1;
  }
  .stat-card.stat-total .stat-value { color: var(--au-navy); }
  .stat-card.stat-pending .stat-value { color: var(--pending); }
  .stat-card.stat-inprog .stat-value { color: var(--inprogress); }
  .stat-card.stat-done .stat-value { color: var(--done); }

  /* ===== PROGRESS BAR ===== */
  .progress-card {
    background: #fff;
    border-radius: var(--radius);
    padding: 22px 24px;
    border: 1.5px solid var(--border);
    box-shadow: var(--card-shadow);
    margin-bottom: 24px;
  }
  .progress-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    margin-bottom: 12px;
  }
  .progress-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.05rem;
    color: var(--au-navy);
  }
  .progress-pct {
    font-size: 2rem;
    font-weight: 700;
    font-family: 'Playfair Display', serif;
    color: var(--au-navy);
    line-height: 1;
  }
  .progress-bar-track {
    height: 10px;
    background: var(--au-light);
    border-radius: 99px;
    overflow: hidden;
    margin-bottom: 8px;
  }
  .progress-bar-fill {
    height: 100%;
    background: linear-gradient(90deg, var(--au-navy), var(--au-red));
    border-radius: 99px;
    transition: width 0.5s cubic-bezier(0.34,1.56,0.64,1);
    width: 0%;
  }
  .progress-legend {
    display: flex;
    gap: 18px;
    flex-wrap: wrap;
  }
  .legend-dot {
    display: flex;
    align-items: center;
    gap: 6px;
    font-size: 0.75rem;
    color: var(--text-sub);
  }
  .dot {
    width: 9px;
    height: 9px;
    border-radius: 50%;
    flex-shrink: 0;
  }
  .dot.pending { background: var(--pending); }
  .dot.inprogress { background: var(--inprogress); }
  .dot.done { background: var(--done); }

  /* ===== FILTER BAR ===== */
  .filter-bar {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
    margin-bottom: 20px;
  }
  .filter-btn {
    padding: 7px 16px;
    border-radius: 99px;
    border: 1.5px solid var(--border);
    background: #fff;
    font-size: 0.78rem;
    font-family: 'DM Sans', sans-serif;
    color: var(--text-sub);
    cursor: pointer;
    font-weight: 500;
    transition: all 0.18s;
  }
  .filter-btn:hover { border-color: var(--au-navy); color: var(--au-navy); }
  .filter-btn.active {
    background: var(--au-navy);
    color: #fff;
    border-color: var(--au-navy);
  }

  /* ===== SECTION CARD ===== */
  .section-card {
    background: #fff;
    border-radius: var(--radius);
    border: 1.5px solid var(--border);
    box-shadow: var(--card-shadow);
    margin-bottom: 18px;
    overflow: hidden;
    transition: box-shadow 0.2s;
  }
  .section-card:hover { box-shadow: 0 6px 28px rgba(0,32,91,0.11); }
  .section-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 16px 22px;
    cursor: pointer;
    user-select: none;
    gap: 12px;
    border-bottom: 1.5px solid transparent;
    transition: background 0.15s;
  }
  .section-header:hover { background: #FAFBFD; }
  .section-header.open { border-bottom-color: var(--border); }
  .section-header-left {
    display: flex;
    align-items: center;
    gap: 12px;
    flex: 1;
    min-width: 0;
  }
  .section-num {
    width: 30px;
    height: 30px;
    border-radius: 8px;
    background: var(--au-navy);
    color: #fff;
    font-size: 0.78rem;
    font-weight: 700;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    font-family: 'Playfair Display', serif;
  }
  .section-title-wrap { flex: 1; min-width: 0; }
  .section-title {
    font-weight: 600;
    font-size: 0.92rem;
    color: var(--au-navy);
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .section-subtitle {
    font-size: 0.72rem;
    color: var(--text-sub);
    margin-top: 1px;
  }
  .section-header-right {
    display: flex;
    align-items: center;
    gap: 10px;
    flex-shrink: 0;
  }
  .sec-progress-mini {
    display: flex;
    align-items: center;
    gap: 7px;
  }
  .sec-bar-track {
    width: 72px;
    height: 5px;
    background: var(--au-light);
    border-radius: 99px;
    overflow: hidden;
  }
  .sec-bar-fill {
    height: 100%;
    background: linear-gradient(90deg, var(--au-navy), var(--au-red));
    border-radius: 99px;
    transition: width 0.4s ease;
  }
  .sec-pct-label {
    font-size: 0.72rem;
    color: var(--text-sub);
    font-weight: 600;
    min-width: 32px;
    text-align: right;
  }
  .chevron {
    width: 20px;
    height: 20px;
    color: var(--text-sub);
    transition: transform 0.25s;
    flex-shrink: 0;
  }
  .chevron.open { transform: rotate(180deg); }
  .section-body { display: none; padding: 0; }
  .section-body.open { display: block; }

  /* ===== DOC ROW ===== */
  .doc-row {
    display: grid;
    grid-template-columns: 1fr 180px 130px;
    align-items: start;
    padding: 14px 22px;
    border-bottom: 1px solid var(--border);
    gap: 14px;
    transition: background 0.15s;
  }
  .doc-row:last-child { border-bottom: none; }
  .doc-row:hover { background: #FAFBFD; }
  .doc-row.hidden-filter { display: none; }

  .doc-name-wrap { display: flex; flex-direction: column; gap: 3px; }
  .doc-name { font-size: 0.87rem; font-weight: 500; color: var(--text-main); }
  .doc-note { font-size: 0.73rem; color: var(--text-sub); }
  .doc-name.done-text { text-decoration: line-through; color: var(--text-sub); }

  /* Duration Input */
  .duration-wrap {
    display: flex;
    align-items: center;
    gap: 8px;
  }
  .duration-input {
    width: 56px;
    padding: 5px 8px;
    border: 1.5px solid var(--border);
    border-radius: 7px;
    font-size: 0.8rem;
    font-family: 'DM Sans', sans-serif;
    color: var(--text-main);
    background: var(--au-light);
    text-align: center;
    outline: none;
    transition: border-color 0.18s;
  }
  .duration-input:focus { border-color: var(--au-navy); background: #fff; }
  .duration-unit {
    font-size: 0.73rem;
    color: var(--text-sub);
    white-space: nowrap;
  }

  /* Status Selector */
  .status-select-wrap { position: relative; }
  .status-select {
    appearance: none;
    -webkit-appearance: none;
    width: 100%;
    padding: 6px 28px 6px 12px;
    border-radius: 99px;
    border: 1.5px solid var(--border);
    font-size: 0.78rem;
    font-family: 'DM Sans', sans-serif;
    font-weight: 600;
    cursor: pointer;
    outline: none;
    background: var(--au-light);
    color: var(--text-sub);
    transition: all 0.18s;
  }
  .status-select:focus { border-color: var(--au-navy); }
  .status-select.pending { background: #F1F5F9; color: #64748B; border-color: #CBD5E1; }
  .status-select.inprogress { background: #FFFBEB; color: #D97706; border-color: #FDE68A; }
  .status-select.done { background: #ECFDF5; color: #059669; border-color: #A7F3D0; }
  .select-arrow {
    position: absolute;
    right: 10px;
    top: 50%;
    transform: translateY(-50%);
    pointer-events: none;
    color: var(--text-sub);
    width: 12px;
  }

  /* ===== BANK SUB-ROWS ===== */
  .bank-sub-section {
    background: #FAFBFF;
    border-top: 1px dashed var(--border);
  }
  .bank-sub-header {
    padding: 10px 22px 10px 38px;
    display: flex;
    align-items: center;
    gap: 8px;
    cursor: pointer;
    user-select: none;
  }
  .bank-sub-header:hover { background: #F0F4FF; }
  .bank-toggle-icon {
    width: 16px;
    height: 16px;
    color: var(--au-navy);
    transition: transform 0.2s;
    flex-shrink: 0;
  }
  .bank-toggle-icon.open { transform: rotate(90deg); }
  .bank-sub-title { font-size: 0.8rem; font-weight: 600; color: var(--au-navy); }
  .bank-sub-hint { font-size: 0.71rem; color: var(--text-sub); margin-left: 4px; }
  .bank-sub-list { display: none; padding-bottom: 6px; }
  .bank-sub-list.open { display: block; }
  .bank-doc-row {
    display: grid;
    grid-template-columns: 1fr 180px 130px;
    align-items: start;
    padding: 10px 22px 10px 52px;
    border-bottom: 1px dashed #EEF2FF;
    gap: 14px;
    transition: background 0.15s;
  }
  .bank-doc-row:last-child { border-bottom: none; }
  .bank-doc-row:hover { background: #EEF2FF; }

  /* ===== TRAVEL PROCESS PANEL ===== */
  .travel-progress-card {
    background: linear-gradient(135deg, #001843 0%, #00205B 100%);
    border-radius: var(--radius);
    padding: 22px 24px;
    margin-bottom: 24px;
    color: #fff;
    box-shadow: 0 8px 32px rgba(0,32,91,0.22);
  }
  .travel-progress-title {
    font-family: 'Playfair Display', serif;
    font-size: 1.05rem;
    margin-bottom: 6px;
    opacity: 0.9;
  }
  .travel-pct-row {
    display: flex;
    align-items: flex-end;
    justify-content: space-between;
    margin-bottom: 10px;
  }
  .travel-pct {
    font-size: 2.2rem;
    font-weight: 700;
    font-family: 'Playfair Display', serif;
    line-height: 1;
  }
  .travel-pct-sub { font-size: 0.75rem; opacity: 0.55; }
  .travel-bar-track {
    height: 8px;
    background: rgba(255,255,255,0.15);
    border-radius: 99px;
    overflow: hidden;
  }
  .travel-bar-fill {
    height: 100%;
    background: linear-gradient(90deg, #D4AF37, #F59E0B);
    border-radius: 99px;
    transition: width 0.5s cubic-bezier(0.34,1.56,0.64,1);
    width: 0%;
  }

  /* ===== COLUMN HEADERS ===== */
  .col-headers {
    display: grid;
    grid-template-columns: 1fr 180px 130px;
    padding: 8px 22px;
    gap: 14px;
    background: #F8FAFC;
    border-bottom: 1.5px solid var(--border);
  }
  .col-h { font-size: 0.7rem; font-weight: 600; color: var(--text-sub); text-transform: uppercase; letter-spacing: 0.07em; }

  /* ===== LANGUAGE / NO-ITEMS ===== */
  .no-items-row {
    padding: 20px 22px;
    font-size: 0.82rem;
    color: var(--text-sub);
    text-align: center;
    font-style: italic;
  }

  /* ===== TRAVEL DOCS SECTION ===== */
  .travel-section-label {
    display: inline-flex;
    align-items: center;
    gap: 7px;
    background: rgba(212,175,55,0.12);
    color: #B8860B;
    border: 1px solid rgba(212,175,55,0.3);
    border-radius: 99px;
    padding: 3px 12px;
    font-size: 0.72rem;
    font-weight: 600;
    margin-bottom: 18px;
    letter-spacing: 0.04em;
    text-transform: uppercase;
  }

  .info-banner {
    background: #FFF7ED;
    border: 1.5px solid #FED7AA;
    border-radius: 10px;
    padding: 12px 18px;
    font-size: 0.8rem;
    color: #92400E;
    margin-bottom: 20px;
    display: flex;
    align-items: flex-start;
    gap: 10px;
  }
  .info-banner svg { flex-shrink: 0; margin-top: 1px; }
  .info-banner strong { display: block; margin-bottom: 2px; font-weight: 600; }

  /* ===== RESPONSIVE ===== */
  @media (max-width: 700px) {
    .header-inner { padding: 14px 16px; }
    .main-wrap { padding: 16px 12px 60px; }
    .tab-nav { padding: 0 12px; }
    .tab-btn { padding: 12px 14px; font-size: 0.78rem; }
    .doc-row, .bank-doc-row, .col-headers {
      grid-template-columns: 1fr;
      gap: 8px;
    }
    .doc-row { padding: 12px 14px; }
    .bank-doc-row { padding: 10px 14px 10px 28px; }
    .col-headers { display: none; }
    .duration-wrap { flex-direction: row; }
    .section-header { padding: 14px 16px; }
    .sec-bar-track { width: 50px; }
    .dash-stats { grid-template-columns: repeat(2, 1fr); }
  }
</style>
</head>
<body>

<!-- HEADER -->
<header class="site-header">
  <div class="header-inner">
    <div class="header-brand">
      <div class="flag-badge">
        <svg width="32" height="32" viewBox="0 0 32 32" fill="none">
          <circle cx="16" cy="16" r="16" fill="#00205B"/>
          <rect x="0" y="12" width="32" height="8" fill="#C8102E"/>
          <rect x="12" y="0" width="8" height="32" fill="#C8102E"/>
          <rect x="0" y="13.5" width="32" height="5" fill="white"/>
          <rect x="13.5" y="0" width="5" height="32" fill="white"/>
        </svg>
      </div>
      <div class="header-title">
        <h1>Australia Visa Document Tracker</h1>
        <p>Checklist &amp; Progress Management System</p>
      </div>
    </div>
    <div class="header-meta">
      <button class="header-reset-btn" onclick="resetAll()">Reset All</button>
    </div>
  </div>
</header>

<!-- TAB NAV -->
<div class="tab-nav-wrap">
  <nav class="tab-nav">
    <button class="tab-btn active" onclick="switchTab('visa', this)">
      Visa Documents
      <span class="tab-badge" id="tab-badge-visa">0%</span>
    </button>
    <button class="tab-btn" onclick="switchTab('travel', this)">
      Travel Preparation
      <span class="tab-badge" id="tab-badge-travel">0%</span>
    </button>
  </nav>
</div>

<!-- MAIN -->
<div class="main-wrap">

  <!-- ============== VISA TAB ============== -->
  <div class="tab-panel active" id="panel-visa">

    <!-- Stats -->
    <div class="dash-stats">
      <div class="stat-card stat-total">
        <div class="stat-label">Total Documents</div>
        <div class="stat-value" id="stat-total">0</div>
      </div>
      <div class="stat-card stat-pending">
        <div class="stat-label">Pending</div>
        <div class="stat-value" id="stat-pending">0</div>
      </div>
      <div class="stat-card stat-inprog">
        <div class="stat-label">In Progress</div>
        <div class="stat-value" id="stat-inprog">0</div>
      </div>
      <div class="stat-card stat-done">
        <div class="stat-label">Completed</div>
        <div class="stat-value" id="stat-done">0</div>
      </div>
    </div>

    <!-- Progress -->
    <div class="progress-card">
      <div class="progress-header">
        <div class="progress-title">Overall Visa Application Progress</div>
        <div class="progress-pct" id="visa-pct">0%</div>
      </div>
      <div class="progress-bar-track">
        <div class="progress-bar-fill" id="visa-bar"></div>
      </div>
      <div class="progress-legend">
        <div class="legend-dot"><span class="dot pending"></span> Pending</div>
        <div class="legend-dot"><span class="dot inprogress"></span> In Progress</div>
        <div class="legend-dot"><span class="dot done"></span> Completed</div>
      </div>
    </div>

    <!-- Filter -->
    <div class="filter-bar">
      <button class="filter-btn active" onclick="filterDocs('all', this)">All</button>
      <button class="filter-btn" onclick="filterDocs('pending', this)">Pending</button>
      <button class="filter-btn" onclick="filterDocs('inprogress', this)">In Progress</button>
      <button class="filter-btn" onclick="filterDocs('done', this)">Completed</button>
    </div>

    <!-- SECTIONS (built by JS) -->
    <div id="visa-sections"></div>
  </div>

  <!-- ============== TRAVEL TAB ============== -->
  <div class="tab-panel" id="panel-travel">

    <div class="info-banner">
      <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
        <circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="12"/><line x1="12" y1="16" x2="12.01" y2="16"/>
      </svg>
      <div>
        <strong>Travel Preparation Process (Independent)</strong>
        รายการนี้แยกออกจากเอกสารวีซ่า และไม่นำมาคำนวณรวมใน Visa Progress
      </div>
    </div>

    <!-- Travel Stats -->
    <div class="dash-stats">
      <div class="stat-card stat-total">
        <div class="stat-label">Total Items</div>
        <div class="stat-value" id="tstat-total">0</div>
      </div>
      <div class="stat-card stat-pending">
        <div class="stat-label">Pending</div>
        <div class="stat-value" id="tstat-pending">0</div>
      </div>
      <div class="stat-card stat-inprog">
        <div class="stat-label">In Progress</div>
        <div class="stat-value" id="tstat-inprog">0</div>
      </div>
      <div class="stat-card stat-done">
        <div class="stat-label">Completed</div>
        <div class="stat-value" id="tstat-done">0</div>
      </div>
    </div>

    <!-- Travel Progress -->
    <div class="travel-progress-card">
      <div class="travel-progress-title">Travel Preparation Progress</div>
      <div class="travel-pct-row">
        <div class="travel-pct" id="travel-pct">0%</div>
        <div class="travel-pct-sub">items completed</div>
      </div>
      <div class="travel-bar-track">
        <div class="travel-bar-fill" id="travel-bar"></div>
      </div>
    </div>

    <!-- Travel Filter -->
    <div class="filter-bar">
      <button class="filter-btn active" onclick="filterTravelDocs('all', this)">All</button>
      <button class="filter-btn" onclick="filterTravelDocs('pending', this)">Pending</button>
      <button class="filter-btn" onclick="filterTravelDocs('inprogress', this)">In Progress</button>
      <button class="filter-btn" onclick="filterTravelDocs('done', this)">Completed</button>
    </div>

    <div id="travel-sections"></div>
  </div>

</div><!-- /main-wrap -->

<script>
// ================================================================
// DATA DEFINITIONS
// ================================================================

const VISA_SECTIONS = [
  {
    id: 'sec1',
    num: '1',
    title: 'Travel Document',
    subtitle: 'Personal identification documents',
    docs: [
      { id: 'd1_1', name: 'Passport (current)', note: 'หนังสือเดินทางฉบับปัจจุบัน — ต้องมีอายุเหลืออย่างน้อย 6 เดือน' },
      { id: 'd1_2', name: 'ID Card', note: 'บัตรประชาชน' },
      { id: 'd1_3', name: 'Household Registration', note: 'ทะเบียนบ้าน' },
      { id: 'd1_4', name: 'Statement of Purpose', note: 'แพลนในการอยู่ออสเตรเลีย 1 ปี (SOP)' },
    ]
  },
  {
    id: 'sec2',
    num: '2',
    title: 'Evidence of Home Government Support',
    subtitle: 'หนังสือรับรองจากหน่วยงานภาครัฐ',
    docs: [
      { id: 'd2_1', name: 'Government Support Letter', note: 'หนังสือรับรองจากกรมส่งเสริมและพัฒนาคุณภาพชีวิตคนพิการ (ดย.)' },
    ]
  },
  {
    id: 'sec3',
    num: '3',
    title: 'Photograph — Passport',
    subtitle: 'รูปถ่ายสำหรับยื่นวีซ่า',
    docs: [
      { id: 'd3_1', name: 'Passport Photo', note: 'ขนาด 3.5 cm x 4.5 cm พื้นหลังขาว ถ่ายไม่เกิน 6 เดือน' },
    ]
  },
  {
    id: 'sec4',
    num: '4',
    title: 'Evidence of Funds for Stay in Australia',
    subtitle: 'เอกสารการเงินและรายได้',
    docs: [
      { id: 'd4_1', name: 'Evidence of Source of Fund', note: 'เอกสารชี้แจงแหล่งที่มาของเงิน' },
      { id: 'd4_2', name: 'Statement (6 months)', note: 'Bank Statement ย้อนหลัง 6 เดือน', isStatement: true },
      { id: 'd4_6', name: 'Book Bank Page', note: '(หน้าบัญชีธนาคาร)', isStatement: true },
      { id: 'd4_3', name: 'Bank Certificate', note: 'หนังสือรับรองยอดเงินในบัญชีจากธนาคาร' },
      { id: 'd4_4', name: 'Employment & Salary Certificate', note: 'หนังสือรับรองการทำงานและเงินเดือน' },
      { id: 'd4_5', name: 'Pay Slip (6 months)', note: 'สลิปเงินเดือนย้อนหลัง 6 เดือน' },
      { id: 'd4_5', name: 'Salary Account Change letter', note: 'หลักฐานการเปลี่ยนบัญชีรับเงินเดือน' },
      { id: 'd4_6', name: 'Tax Form (Phor.Ngor.Dor 90/91)', note: 'ภ.ง.ด.90 หรือ ภ.ง.ด.91' },
      { id: 'd4_7', name: 'Tax Payment Certificate', note: 'ใบรับรองการเสียภาษี' },
    ]
  },
  {
    id: 'sec5',
    num: '5',
    title: 'Language Ability',
    subtitle: 'หลักฐานความสามารถทางภาษา',
    docs: [
      { id: 'd5_1', name: 'English Language Test Result', note: 'เช่น IELTS, TOEFL, PTE (ถ้ามี)' },
    ]
  },
  {
    id: 'sec6',
    num: '6',
    title: 'Qualifications',
    subtitle: 'เอกสารคุณวุฒิการศึกษา',
    docs: [
      { id: 'd6_1', name: 'Degree Certificate', note: 'ใบปริญญาบัตร' },
      { id: 'd6_2', name: 'Transcript', note: 'ใบรายงานผลการเรียน (Official / Unofficial)' },
    ]
  },
  {
    id: 'sec7',
    num: '7',
    title: 'Other Documents',
    subtitle: 'เอกสารประกอบอื่น ๆ',
    docs: [
      { id: 'd7_1', name: 'Visa Fee Receipt', note: 'ใบเสร็จค่าธรรมเนียมวีซ่า' },
      { id: 'd7_2', name: 'Birth Certificate', note: 'สูติบัตร / ใบเกิด' },
      { id: 'd7_3', name: 'Drivers Licence', note: 'ใบขับขี่ (ถ้ามี)' },
      { id: 'd7_4', name: 'CV / Resume', note: 'ประวัติย่อ / Curriculum Vitae' },
      { id: 'd7_5', name: 'Supporting Evidence for SOP', note: 'หลักฐานประกอบ Statement of Purpose' },
    ]
  },
  {
    id: 'sec8',
    num: '8',
    title: 'Change of Name',
    subtitle: 'เอกสารเปลี่ยนชื่อ / นามสกุล',
    docs: [
      { id: 'd8_1', name: 'Name Change Document', note: 'เอกสารเปลี่ยนนามสกุล (ถ้ามี)' },
    ]
  },
];

const THAI_BANKS = [
  'ธนาคารกรุงเทพ (BBL)',
  'ธนาคารกสิกรไทย (KBANK)',
  'ธนาคารไทยพาณิชย์ (SCB)',
  'ธนาคารกรุงไทย (KTB)',
  'ธนาคารกรุงศรีอยุธยา (BAY)',
  'ธนาคารทหารไทยธนชาต (TTB)',
  'ธนาคารเกียรตินาคินภัทร (KKP)',
  'ธนาคารซีไอเอ็มบีไทย (CIMBT)',
  'ธนาคารยูโอบี (UOB)',
  'ธนาคารแลนด์แอนด์เฮ้าส์ (LH Bank)',
  'ธนาคารอิสลามแห่งประเทศไทย (IBANK)',
  'ธนาคารไทยเครดิตเพื่อรายย่อย',
  'ธนาคารออมสิน (GSB)',
  'ธนาคารเพื่อการเกษตรและสหกรณ์ (BAAC)',
  'ธนาคารอาคารสงเคราะห์ (GHB)',
];

const TRAVEL_SECTIONS = [
  {
    id: 'tsec1',
    num: 'A',
    title: 'Flight & Accommodation Booking',
    subtitle: 'การจองตั๋วและที่พัก',
    docs: [
      { id: 'td1_1', name: 'Flight Ticket Reservation', note: 'ตั๋วเครื่องบิน (จองล่วงหน้า)' },
      { id: 'td1_2', name: 'Accommodation Booking Confirmation', note: 'ยืนยันการจองที่พัก' },
      { id: 'td1_3', name: 'Travel Insurance', note: 'ประกันการเดินทาง' },
    ]
  },
  {
    id: 'tsec2',
    num: 'B',
    title: 'Health & Medical Preparation',
    subtitle: 'การเตรียมสุขภาพก่อนเดินทาง',
    docs: [
      { id: 'td2_1', name: 'Medical Check-up Certificate', note: 'ใบรับรองแพทย์ (ตรวจสุขภาพ)' },
      { id: 'td2_2', name: 'Vaccination Record', note: 'สมุดบันทึกวัคซีน / Yellow Card' },
      { id: 'td2_3', name: 'Prescription / Medication List', note: 'ใบสั่งยาสำหรับยาที่จำเป็น' },
    ]
  },
  {
    id: 'tsec3',
    num: 'C',
    title: 'Financial Preparation',
    subtitle: 'เตรียมเงินและบัตรสำหรับใช้ในออสเตรเลีย',
    docs: [
      { id: 'td3_1', name: 'International Debit / Credit Card', note: 'บัตรเดบิต/เครดิตสำหรับใช้ต่างประเทศ' },
      { id: 'td3_2', name: 'Cash (AUD)', note: 'เงินสดดอลลาร์ออสเตรเลียสำหรับค่าใช้จ่ายเร่งด่วน' },
      { id: 'td3_3', name: 'Wise / Revolut Account', note: 'บัญชีเงินอิเล็กทรอนิกส์ระหว่างประเทศ (ถ้ามี)' },
    ]
  },
  {
    id: 'tsec4',
    num: 'D',
    title: 'Communication & Connectivity',
    subtitle: 'การสื่อสารและการเชื่อมต่ออินเทอร์เน็ต',
    docs: [
      { id: 'td4_1', name: 'Australian SIM Card / eSIM', note: 'ซิมการ์ดออสเตรเลีย หรือ eSIM (Telstra/Optus)' },
      { id: 'td4_2', name: 'Emergency Contact List', note: 'รายชื่อผู้ติดต่อฉุกเฉินทั้งในไทยและออสเตรเลีย' },
    ]
  },
];

// ================================================================
// STATE MANAGEMENT
// ================================================================

const STORAGE_KEY = 'au_visa_tracker_v3';

function loadState() {
  try {
    const raw = localStorage.getItem(STORAGE_KEY);
    return raw ? JSON.parse(raw) : {};
  } catch(e) { return {}; }
}
function saveState(state) {
  localStorage.setItem(STORAGE_KEY, JSON.stringify(state));
}

let state = loadState();

function getDocState(id) {
  return state[id] || { status: 'pending', duration: '' };
}
function setDocState(id, key, value) {
  if (!state[id]) state[id] = { status: 'pending', duration: '' };
  state[id][key] = value;
  saveState(state);
}

// ================================================================
// RENDER HELPERS
// ================================================================

function makeStatusSelect(docId, isSmall) {
  const ds = getDocState(docId);
  return `
    <div class="status-select-wrap">
      <select class="status-select ${ds.status}" onchange="onStatusChange('${docId}', this)">
        <option value="pending" ${ds.status==='pending'?'selected':''}>Pending</option>
        <option value="inprogress" ${ds.status==='inprogress'?'selected':''}>In Progress</option>
        <option value="done" ${ds.status==='done'?'selected':''}>Done</option>
      </select>
      <svg class="select-arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="6 9 12 15 18 9"/></svg>
    </div>`;
}

function makeDurationInput(docId) {
  const ds = getDocState(docId);
  return `
    <div class="duration-wrap">
      <input class="duration-input" type="number" min="0" placeholder="0"
        value="${ds.duration || ''}"
        onchange="onDurationChange('${docId}', this.value)"
        title="ระยะเวลาในการเตรียม"
      />
      <span class="duration-unit">วัน</span>
    </div>`;
}

function secProgress(docs) {
  const total = docs.length;
  if (!total) return { pct: 0, done: 0 };
  const done = docs.filter(d => getDocState(d.id).status === 'done').length;
  return { pct: Math.round(done / total * 100), done };
}

// ================================================================
// RENDER VISA SECTIONS
// ================================================================

function renderVisaSections() {
  const container = document.getElementById('visa-sections');
  container.innerHTML = VISA_SECTIONS.map(sec => {
    const prog = secProgress(sec.docs);
    const docsHtml = sec.docs.map(doc => {
      const ds = getDocState(doc.id);
      const isDone = ds.status === 'done';
      // Statement doc gets bank sub-section
      const bankPart = doc.isStatement ? renderBankSubSection(doc.id) : '';
      return `
        <div class="doc-row" data-docid="${doc.id}" data-status="${ds.status}" data-section="visa">
          <div class="doc-name-wrap">
            <span class="doc-name ${isDone ? 'done-text' : ''}">${doc.name}</span>
            ${doc.note ? `<span class="doc-note">${doc.note}</span>` : ''}
          </div>
          ${makeDurationInput(doc.id)}
          ${makeStatusSelect(doc.id)}
        </div>
        ${bankPart}`;
    }).join('');

    return `
      <div class="section-card" id="${sec.id}">
        <div class="section-header" onclick="toggleSection('${sec.id}')">
          <div class="section-header-left">
            <div class="section-num">${sec.num}</div>
            <div class="section-title-wrap">
              <div class="section-title">${sec.title}</div>
              <div class="section-subtitle">${sec.subtitle}</div>
            </div>
          </div>
          <div class="section-header-right">
            <div class="sec-progress-mini">
              <div class="sec-bar-track">
                <div class="sec-bar-fill" style="width:${prog.pct}%" id="sb-${sec.id}"></div>
              </div>
              <span class="sec-pct-label" id="sp-${sec.id}">${prog.pct}%</span>
            </div>
            <svg class="chevron open" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="18 15 12 9 6 15"/></svg>
          </div>
        </div>
        <div class="section-body open" id="body-${sec.id}">
          <div class="col-headers">
            <div class="col-h">Document</div>
            <div class="col-h">Est. Duration</div>
            <div class="col-h">Status</div>
          </div>
          ${docsHtml}
        </div>
      </div>`;
  }).join('');
  updateVisaStats();
}

// Bank sub-section for Statement row
function renderBankSubSection(parentDocId) {
  const bankSectionId = 'bankSection_' + parentDocId;
  const banks = THAI_BANKS.map((bname, i) => {
    const bid = parentDocId + '_bank_' + i;
    const ds = getDocState(bid);
    const isDone = ds.status === 'done';
    return `
      <div class="bank-doc-row" data-docid="${bid}" data-status="${ds.status}" data-section="bank">
        <div class="doc-name-wrap">
          <span class="doc-name ${isDone ? 'done-text' : ''}">${bname}</span>
          <span class="doc-note">Statement ย้อนหลัง 6 เดือน</span>
        </div>
        ${makeDurationInput(bid)}
        ${makeStatusSelect(bid)}
      </div>`;
  }).join('');

  return `
    <div class="bank-sub-section" id="${bankSectionId}">
      <div class="bank-sub-header" onclick="toggleBankSub('${bankSectionId}')">
        <svg class="bank-toggle-icon open" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><polyline points="9 18 15 12 9 6"/></svg>
        <span class="bank-sub-title">เลือกธนาคาร</span>
        <span class="bank-sub-hint">— คลิกเพื่อขยาย/ย่อ รายชื่อธนาคารพาณิชย์ไทย</span>
      </div>
      <div class="bank-sub-list open" id="bankList_${parentDocId}">
        ${banks}
      </div>
    </div>`;
}

// ================================================================
// RENDER TRAVEL SECTIONS
// ================================================================

function renderTravelSections() {
  const container = document.getElementById('travel-sections');
  container.innerHTML = TRAVEL_SECTIONS.map(sec => {
    const prog = secProgress(sec.docs);
    const docsHtml = sec.docs.map(doc => {
      const ds = getDocState(doc.id);
      const isDone = ds.status === 'done';
      return `
        <div class="doc-row" data-docid="${doc.id}" data-status="${ds.status}" data-section="travel">
          <div class="doc-name-wrap">
            <span class="doc-name ${isDone ? 'done-text' : ''}">${doc.name}</span>
            ${doc.note ? `<span class="doc-note">${doc.note}</span>` : ''}
          </div>
          ${makeDurationInput(doc.id)}
          ${makeStatusSelect(doc.id)}
        </div>`;
    }).join('');

    return `
      <div class="section-card" id="${sec.id}">
        <div class="section-header" onclick="toggleSection('${sec.id}')">
          <div class="section-header-left">
            <div class="section-num" style="background:var(--au-gold);color:#1E293B">${sec.num}</div>
            <div class="section-title-wrap">
              <div class="section-title">${sec.title}</div>
              <div class="section-subtitle">${sec.subtitle}</div>
            </div>
          </div>
          <div class="section-header-right">
            <div class="sec-progress-mini">
              <div class="sec-bar-track">
                <div class="sec-bar-fill" style="width:${prog.pct}%;background:linear-gradient(90deg,#D4AF37,#F59E0B)" id="sb-${sec.id}"></div>
              </div>
              <span class="sec-pct-label" id="sp-${sec.id}">${prog.pct}%</span>
            </div>
            <svg class="chevron open" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="18 15 12 9 6 15"/></svg>
          </div>
        </div>
        <div class="section-body open" id="body-${sec.id}">
          <div class="col-headers">
            <div class="col-h">Item</div>
            <div class="col-h">Est. Duration</div>
            <div class="col-h">Status</div>
          </div>
          ${docsHtml}
        </div>
      </div>`;
  }).join('');
  updateTravelStats();
}

// ================================================================
// STATS / PROGRESS UPDATE
// ================================================================

function updateVisaStats() {
  // Only count visa docs (not bank sub-docs, not travel)
  let allDocs = [];
  VISA_SECTIONS.forEach(sec => sec.docs.forEach(d => allDocs.push(d)));

  const total = allDocs.length;
  const done = allDocs.filter(d => getDocState(d.id).status === 'done').length;
  const inprog = allDocs.filter(d => getDocState(d.id).status === 'inprogress').length;
  const pending = total - done - inprog;
  const pct = total ? Math.round(done / total * 100) : 0;

  document.getElementById('stat-total').textContent = total;
  document.getElementById('stat-pending').textContent = pending;
  document.getElementById('stat-inprog').textContent = inprog;
  document.getElementById('stat-done').textContent = done;
  document.getElementById('visa-pct').textContent = pct + '%';
  document.getElementById('visa-bar').style.width = pct + '%';
  document.getElementById('tab-badge-visa').textContent = pct + '%';

  // Update section mini bars
  VISA_SECTIONS.forEach(sec => {
    const prog = secProgress(sec.docs);
    const sb = document.getElementById('sb-' + sec.id);
    const sp = document.getElementById('sp-' + sec.id);
    if (sb) sb.style.width = prog.pct + '%';
    if (sp) sp.textContent = prog.pct + '%';
  });
}

function updateTravelStats() {
  let allDocs = [];
  TRAVEL_SECTIONS.forEach(sec => sec.docs.forEach(d => allDocs.push(d)));
  const total = allDocs.length;
  const done = allDocs.filter(d => getDocState(d.id).status === 'done').length;
  const inprog = allDocs.filter(d => getDocState(d.id).status === 'inprogress').length;
  const pending = total - done - inprog;
  const pct = total ? Math.round(done / total * 100) : 0;

  document.getElementById('tstat-total').textContent = total;
  document.getElementById('tstat-pending').textContent = pending;
  document.getElementById('tstat-inprog').textContent = inprog;
  document.getElementById('tstat-done').textContent = done;
  document.getElementById('travel-pct').textContent = pct + '%';
  document.getElementById('travel-bar').style.width = pct + '%';
  document.getElementById('tab-badge-travel').textContent = pct + '%';

  TRAVEL_SECTIONS.forEach(sec => {
    const prog = secProgress(sec.docs);
    const sb = document.getElementById('sb-' + sec.id);
    const sp = document.getElementById('sp-' + sec.id);
    if (sb) sb.style.width = prog.pct + '%';
    if (sp) sp.textContent = prog.pct + '%';
  });
}

// ================================================================
// EVENT HANDLERS
// ================================================================

function onStatusChange(docId, selectEl) {
  const newStatus = selectEl.value;
  setDocState(docId, 'status', newStatus);

  // Update select styling
  selectEl.className = 'status-select ' + newStatus;

  // Update doc row
  const row = document.querySelector(`[data-docid="${docId}"]`);
  if (row) {
    row.setAttribute('data-status', newStatus);
    const nameEl = row.querySelector('.doc-name');
    if (nameEl) {
      if (newStatus === 'done') nameEl.classList.add('done-text');
      else nameEl.classList.remove('done-text');
    }
  }

  // Detect which section type and update stats
  const section = row ? row.getAttribute('data-section') : 'visa';
  if (section === 'travel') {
    updateTravelStats();
  } else {
    updateVisaStats();
  }

  // Re-apply active filter
  const activeVisaFilter = document.querySelector('#panel-visa .filter-btn.active');
  const activeTravelFilter = document.querySelector('#panel-travel .filter-btn.active');
  if (activeVisaFilter && section !== 'travel') {
    applyFilter(activeVisaFilter.textContent.toLowerCase().replace(' ', ''), 'visa');
  }
  if (activeTravelFilter && section === 'travel') {
    applyFilter(activeTravelFilter.textContent.toLowerCase().replace(' ', ''), 'travel');
  }
}

function onDurationChange(docId, value) {
  setDocState(docId, 'duration', value);
}

function toggleSection(secId) {
  const body = document.getElementById('body-' + secId);
  const header = document.querySelector(`#${secId} .section-header`);
  const chevron = header.querySelector('.chevron');
  if (body.classList.contains('open')) {
    body.classList.remove('open');
    header.classList.remove('open');
    chevron.classList.remove('open');
  } else {
    body.classList.add('open');
    header.classList.add('open');
    chevron.classList.add('open');
  }
}

function toggleBankSub(sectionId) {
  const section = document.getElementById(sectionId);
  const icon = section.querySelector('.bank-toggle-icon');
  const listId = sectionId.replace('bankSection_', 'bankList_');
  const list = document.getElementById(listId);
  if (list.classList.contains('open')) {
    list.classList.remove('open');
    icon.classList.remove('open');
  } else {
    list.classList.add('open');
    icon.classList.add('open');
  }
}

// ================================================================
// FILTER
// ================================================================

function filterDocs(status, btn) {
  document.querySelectorAll('#panel-visa .filter-btn').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  applyFilter(status, 'visa');
}

function filterTravelDocs(status, btn) {
  document.querySelectorAll('#panel-travel .filter-btn').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  applyFilter(status, 'travel');
}

function applyFilter(status, scope) {
  const selector = scope === 'travel'
    ? '#panel-travel .doc-row'
    : '#panel-visa .doc-row, #panel-visa .bank-doc-row';

  document.querySelectorAll(selector).forEach(row => {
    if (status === 'all') {
      row.classList.remove('hidden-filter');
    } else {
      const rs = row.getAttribute('data-status');
      if (rs === status) row.classList.remove('hidden-filter');
      else row.classList.add('hidden-filter');
    }
  });
}

// ================================================================
// TAB SWITCHING
// ================================================================

function switchTab(tab, btn) {
  document.querySelectorAll('.tab-btn').forEach(b => b.classList.remove('active'));
  document.querySelectorAll('.tab-panel').forEach(p => p.classList.remove('active'));
  btn.classList.add('active');
  document.getElementById('panel-' + tab).classList.add('active');
}

// ================================================================
// RESET
// ================================================================

function resetAll() {
  if (!confirm('Reset all document statuses and durations? This cannot be undone.')) return;
  localStorage.removeItem(STORAGE_KEY);
  state = {};
  renderVisaSections();
  renderTravelSections();
}

// ================================================================
// INIT
// ================================================================

renderVisaSections();
renderTravelSections();
</script>
</body>
</html>
