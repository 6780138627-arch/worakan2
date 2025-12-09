<html lang="th">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>RSB Activity Transcript System</title>
  <style>
    :root {
      --primary: #00695c;
      --primary-light: #26a69a;
      --primary-dark: #004d40;
      --accent: #ffb300;
      --bg: #f5f7fb;
      --card-bg: #ffffff;
      --text-main: #263238;
      --text-muted: #607d8b;
      --border-soft: #e0e7ef;
      --shadow-soft: 0 8px 20px rgba(0, 0, 0, 0.06);
      --radius-lg: 18px;
      --radius-pill: 999px;
      --transition-fast: 0.2s ease-out;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: var(--bg);
      color: var(--text-main);
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    /* Layout */
    .page {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }

    .container {
      width: 100%;
      max-width: 1080px;
      margin: 0 auto;
      padding: 0 1.25rem;
    }

    /* Header / Navbar */
    header {
      position: sticky;
      top: 0;
      z-index: 50;
      background: rgba(245, 247, 251, 0.95);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid rgba(224, 231, 239, 0.8);
    }

    .nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0.9rem 0;
      gap: 1rem;
    }

    .brand {
      display: flex;
      align-items: center;
      gap: 0.6rem;
    }

    .brand-logo {
      width: 36px;
      height: 36px;
      border-radius: 30%;
      background: radial-gradient(circle at 30% 30%, #ffffff, var(--primary));
      display: flex;
      align-items: center;
      justify-content: center;
      color: #ffffff;
      font-weight: 700;
      font-size: 0.9rem;
      box-shadow: var(--shadow-soft);
    }

    .brand-text-title {
      font-weight: 700;
      font-size: 1.05rem;
      color: var(--primary-dark);
    }

    .brand-text-sub {
      font-size: 0.8rem;
      color: var(--text-muted);
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 0.75rem;
      font-size: 0.9rem;
    }

    .nav-links a {
      padding: 0.4rem 0.75rem;
      border-radius: var(--radius-pill);
      color: var(--text-muted);
      transition: background var(--transition-fast), color var(--transition-fast),
        transform var(--transition-fast);
    }

    .nav-links a:hover {
      background: rgba(0, 105, 92, 0.07);
      color: var(--primary-dark);
      transform: translateY(-1px);
    }

    .nav-cta {
      padding: 0.4rem 0.95rem;
      border-radius: var(--radius-pill);
      background: linear-gradient(135deg, var(--primary), var(--primary-light));
      color: #fff !important;
      font-weight: 600;
      box-shadow: 0 4px 12px rgba(0, 105, 92, 0.4);
    }

    /* Hero section */
    .hero {
      padding: 3.5rem 0 2.5rem;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: minmax(0, 1.4fr) minmax(0, 1.1fr);
      gap: 2.5rem;
      align-items: center;
    }

    .hero-badge {
      display: inline-flex;
      align-items: center;
      gap: 0.4rem;
      padding: 0.2rem 0.75rem;
      border-radius: var(--radius-pill);
      background: rgba(0, 105, 92, 0.06);
      color: var(--primary-dark);
      font-size: 0.8rem;
      margin-bottom: 0.8rem;
    }

    .hero-badge-dot {
      width: 7px;
      height: 7px;
      border-radius: 999px;
      background: var(--accent);
    }

    .hero-title {
      font-size: 2rem;
      font-weight: 800;
      margin-bottom: 0.6rem;
      color: var(--primary-dark);
    }

    .hero-title span {
      color: var(--accent);
    }

    .hero-subtitle {
      font-size: 1.05rem;
      color: var(--text-muted);
      margin-bottom: 1.2rem;
    }

    .hero-list {
      list-style: none;
      margin-bottom: 1.6rem;
    }

    .hero-list li {
      display: flex;
      align-items: flex-start;
      gap: 0.5rem;
      font-size: 0.95rem;
      color: var(--text-main);
      margin-bottom: 0.4rem;
    }

    .hero-list-icon {
      margin-top: 0.18rem;
      width: 18px;
      height: 18px;
      border-radius: 6px;
      background: rgba(0, 105, 92, 0.09);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 0.8rem;
      color: var(--primary-dark);
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 0.75rem;
    }

    .btn-primary {
      padding: 0.6rem 1.3rem;
      border-radius: var(--radius-pill);
      border: none;
      background: linear-gradient(135deg, var(--primary), var(--primary-light));
      color: #ffffff;
      font-size: 0.95rem;
      font-weight: 600;
      cursor: pointer;
      box-shadow: 0 6px 18px rgba(0, 105, 92, 0.5);
      transition: transform var(--transition-fast), box-shadow var(--transition-fast);
    }

    .btn-primary:hover {
      transform: translateY(-1px);
      box-shadow: 0 10px 24px rgba(0, 105, 92, 0.6);
    }

    .btn-ghost {
      padding: 0.6rem 1.2rem;
      border-radius: var(--radius-pill);
      border: 1px solid rgba(0, 105, 92, 0.4);
      background: rgba(255, 255, 255, 0.8);
      color: var(--primary-dark);
      font-size: 0.9rem;
      cursor: pointer;
      transition: background var(--transition-fast), transform var(--transition-fast);
    }

    .btn-ghost:hover {
      background: rgba(0, 105, 92, 0.04);
      transform: translateY(-1px);
    }

    .hero-meta {
      margin-top: 0.75rem;
      font-size: 0.8rem;
      color: var(--text-muted);
    }

    /* Hero mock card */
    .hero-card {
      background: radial-gradient(circle at top left, #ffffff, #e0f2f1);
      border-radius: 24px;
      padding: 1.4rem 1.3rem;
      box-shadow: var(--shadow-soft);
      border: 1px solid rgba(224, 231, 239, 0.9);
    }

    .hero-card-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 0.8rem;
    }

    .hero-card-title {
      font-size: 0.9rem;
      font-weight: 700;
      color: var(--primary-dark);
    }

    .hero-card-badge {
      font-size: 0.7rem;
      padding: 0.15rem 0.6rem;
      border-radius: var(--radius-pill);
      background: rgba(255, 179, 0, 0.1);
      color: #8c6c00;
    }

    .hero-card-body {
      background: rgba(255, 255, 255, 0.9);
      border-radius: 16px;
      padding: 0.9rem;
      border: 1px solid rgba(224, 231, 239, 0.9);
    }

    .mini-table {
      width: 100%;
      border-collapse: collapse;
      font-size: 0.78rem;
    }

    .mini-table thead {
      background: rgba(0, 105, 92, 0.06);
    }

    .mini-table th,
    .mini-table td {
      padding: 0.45rem 0.4rem;
      text-align: left;
      border-bottom: 1px solid rgba(224, 231, 239, 0.9);
    }

    .mini-table th {
      font-weight: 600;
      color: var(--text-muted);
    }

    .mini-chip {
      display: inline-flex;
      padding: 0.18rem 0.5rem;
      border-radius: var(--radius-pill);
      background: rgba(0, 105, 92, 0.07);
      color: var(--primary-dark);
    }

    .hero-card-footer {
      margin-top: 0.8rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      font-size: 0.75rem;
      color: var(--text-muted);
    }

    .status-pill {
      padding: 0.18rem 0.6rem;
      border-radius: var(--radius-pill);
      background: rgba(0, 150, 136, 0.12);
      color: var(--primary-dark);
      font-weight: 600;
      font-size: 0.75rem;
    }

    /* Sections */
    section {
      padding: 2.5rem 0;
    }

    section:nth-of-type(odd) {
      /* alternate feel */
    }

    .section-title {
      font-size: 1.4rem;
      font-weight: 700;
      margin-bottom: 0.4rem;
      color: var(--primary-dark);
    }

    .section-subtitle {
      font-size: 0.9rem;
      color: var(--text-muted);
      margin-bottom: 1.5rem;
    }

    /* Features */
    .feature-grid {
      display: grid;
      grid-template-columns: repeat(3, minmax(0, 1fr));
      gap: 1.25rem;
    }

    .card {
      background: var(--card-bg);
      border-radius: var(--radius-lg);
      padding: 1.2rem 1.1rem;
      border: 1px solid var(--border-soft);
      box-shadow: var(--shadow-soft);
      transition: transform var(--transition-fast), box-shadow var(--transition-fast),
        border-color var(--transition-fast);
    }

    .card:hover {
      transform: translateY(-3px);
      box-shadow: 0 12px 28px rgba(0, 0, 0, 0.08);
      border-color: rgba(0, 105, 92, 0.2);
    }

    .card-icon {
      width: 30px;
      height: 30px;
      border-radius: 12px;
      background: rgba(0, 105, 92, 0.08);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1rem;
      margin-bottom: 0.5rem;
    }

    .card-title {
      font-size: 0.98rem;
      font-weight: 700;
      margin-bottom: 0.3rem;
      color: var(--primary-dark);
    }

    .card-text {
      font-size: 0.86rem;
      color: var(--text-muted);
    }

    /* Workflow */
    .workflow-grid {
      display: grid;
      grid-template-columns: minmax(0, 1.4fr) minmax(0, 1.1fr);
      gap: 1.75rem;
      align-items: flex-start;
    }

    .steps {
      list-style: none;
      counter-reset: step-counter;
    }

    .steps li {
      counter-increment: step-counter;
      display: grid;
      grid-template-columns: auto 1fr;
      gap: 0.6rem 0.9rem;
      align-items: flex-start;
      padding: 0.65rem 0;
    }

    .steps li::before {
      content: counter(step-counter);
      width: 26px;
      height: 26px;
      border-radius: 999px;
      background: var(--primary);
      color: #ffffff;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 0.8rem;
      font-weight: 700;
      margin-top: 0.15rem;
      box-shadow: 0 4px 12px rgba(0, 105, 92, 0.6);
    }

    .step-title {
      font-size: 0.95rem;
      font-weight: 600;
      margin-bottom: 0.12rem;
    }

    .step-text {
      font-size: 0.85rem;
      color: var(--text-muted);
    }

    .comparison-card {
      background: var(--card-bg);
      border-radius: var(--radius-lg);
      border: 1px solid var(--border-soft);
      box-shadow: var(--shadow-soft);
      padding: 1rem;
      font-size: 0.8rem;
    }

    .comparison-card h4 {
      font-size: 0.9rem;
      margin-bottom: 0.5rem;
      color: var(--primary-dark);
    }

    .comparison-table {
      width: 100%;
      border-collapse: collapse;
      font-size: 0.78rem;
    }

    .comparison-table th,
    .comparison-table td {
      padding: 0.4rem 0.4rem;
      border-bottom: 1px solid rgba(224, 231, 239, 0.9);
      text-align: left;
    }

    .comparison-table th {
      background: rgba(0, 105, 92, 0.05);
      font-weight: 600;
      color: var(--text-muted);
    }

    /* Example transcript */
    .transcript-layout {
      display: grid;
      grid-template-columns: minmax(0, 1.2fr) minmax(0, 1fr);
      gap: 1.5rem;
      align-items: flex-start;
    }

    .transcript-card {
      background: #ffffff;
      border-radius: 18px;
      border: 1px solid var(--border-soft);
      box-shadow: var(--shadow-soft);
      padding: 1.1rem;
      font-size: 0.8rem;
    }

    .transcript-header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 0.6rem;
    }

    .transcript-title {
      font-size: 0.9rem;
      font-weight: 700;
      color: var(--primary-dark);
    }

    .transcript-meta {
      font-size: 0.75rem;
      color: var(--text-muted);
    }

    .transcript-tag {
      display: inline-flex;
      padding: 0.18rem 0.5rem;
      border-radius: var(--radius-pill);
      background: rgba(0, 105, 92, 0.06);
      color: var(--primary-dark);
      font-size: 0.75rem;
    }

    .transcript-table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 0.5rem;
    }

    .transcript-table th,
    .transcript-table td {
      padding: 0.4rem 0.35rem;
      border-bottom: 1px solid rgba(224, 231, 239, 0.9);
      text-align: left;
      font-size: 0.78rem;
    }

    .transcript-table th {
      background: rgba(0, 105, 92, 0.04);
      font-weight: 600;
      color: var(--text-muted);
    }

    .badge-soft {
      display: inline-flex;
      padding: 0.18rem 0.45rem;
      border-radius: var(--radius-pill);
      background: rgba(255, 179, 0, 0.12);
      color: #795700;
      font-size: 0.72rem;
    }

    .sidebar-note {
      font-size: 0.85rem;
      color: var(--text-muted);
    }

    .sidebar-note strong {
      color: var(--primary-dark);
    }

    .sidebar-note ul {
      margin-top: 0.5rem;
      padding-left: 1.1rem;
    }

    .sidebar-note li {
      margin-bottom: 0.25rem;
    }

    /* Footer */
    footer {
      padding: 1.5rem 0 1.8rem;
      border-top: 1px solid var(--border-soft);
      margin-top: auto;
      font-size: 0.8rem;
      color: var(--text-muted);
    }

    footer .footer-inner {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      gap: 0.75rem;
      align-items: center;
    }

    footer a {
      color: var(--primary-dark);
      font-weight: 500;
    }

    /* Responsive */
    @media (max-width: 900px) {
      .hero-grid,
      .workflow-grid,
      .transcript-layout {
        grid-template-columns: minmax(0, 1fr);
      }

      .hero {
        padding-top: 2.7rem;
      }

      .feature-grid {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }
    }

    @media (max-width: 700px) {
      .nav {
        flex-wrap: wrap;
        justify-content: center;
      }

      .hero-title {
        font-size: 1.65rem;
      }

      .feature-grid {
        grid-template-columns: minmax(0, 1fr);
      }
    }
  </style>
</head>
<body>
  <div class="page">
    <!-- Header -->
    <header>
      <div class="container">
        <nav class="nav">
          <div class="brand">
            <div class="brand-logo">RSB</div>
            <div>
              <div class="brand-text-title">Activity Transcript System</div>
              <div class="brand-text-sub">โรงเรียนรัตนโกสินทร์สมโภชบางเขน</div>
            </div>
          </div>
          <div class="nav-links">
            <a href="#about">แนวคิด</a>
            <a href="#features">โครงสร้าง</a>
            <a href="#workflow">ขั้นตอนการทำงาน</a>
            <a href="#example">ตัวอย่าง Transcript</a>
            <a href="#about-dev" class="nav-cta">สำหรับ GitHub / Dev</a>
          </div>
        </nav>
      </div>
    </header>

    <main>
      <!-- Hero -->
      <section class="hero" id="top">
        <div class="container">
          <div class="hero-grid">
            <div>
              <div class="hero-badge">
                <div class="hero-badge-dot"></div>
                ระบบต้นแบบเพื่อบริหารข้อมูลกิจกรรมของนักเรียนด้วย ICT
              </div>
              <h1 class="hero-title">
                จาก Google Forms กระจัดกระจาย<br />
                สู่ <span>Activity Transcript</span> แบบอัตโนมัติ
              </h1>
              <p class="hero-subtitle">
                ระบบต้นแบบเพื่อบริหารจัดการข้อมูลกิจกรรมจิตอาสาและกิจกรรมพัฒนาผู้เรียน
                โดยใช้รหัสประจำตัวนักเรียนเป็นแกนกลางของฐานข้อมูล
                สร้าง “ทรานสคริปกิจกรรม” มาตรฐานเดียวกันทั้งโรงเรียน
              </p>
              <ul class="hero-list">
                <li>
                  <span class="hero-list-icon">✓</span>
                  <span>ลดภาระการตรวจสอบซ้ำของครู และลดความคลาดเคลื่อนของข้อมูลกิจกรรม</span>
                </li>
                <li>
                  <span class="hero-list-icon">✓</span>
                  <span>เชื่อมโยงประเภทกิจกรรมหลายมิติ: จิตอาสา ภาวะผู้นำ วิชาการ คุณธรรมจริยธรรม</span>
                </li>
                <li>
                  <span class="hero-list-icon">✓</span>
                  <span>สร้าง Transcript กิจกรรมให้นักเรียนใช้เป็นส่วนหนึ่งของ Portfolio เพื่อยื่นเข้ามหาวิทยาลัย</span>
                </li>
              </ul>

              <div class="hero-actions">
                <a href="#features">
                  <button class="btn-primary">ดูโครงสร้างระบบ</button>
                </a>
                <a href="#workflow">
                  <button class="btn-ghost">ดูขั้นตอนการทำงานของระบบ</button>
                </a>
              </div>
              <div class="hero-meta">
                โปรเจกต์รายวิชา 2747745 เทคโนโลยีสารสนเทศและการสื่อสารเพื่อการบริหารการศึกษา
              </div>
            </div>

            <!-- Hero card (mockup) -->
            <div class="hero-card">
              <div class="hero-card-header">
                <div>
                  <div class="hero-card-title">Transcipt กิจกรรมนักเรียน</div>
                  <div style="font-size: 0.75rem; color: var(--text-muted);">
                    รหัสนักเรียน: 67890 | ม.5/10
                  </div>
                </div>
                <div class="hero-card-badge">Prototype UI</div>
              </div>
              <div class="hero-card-body">
                <table class="mini-table">
                  <thead>
                    <tr>
                      <th>ประเภทกิจกรรม</th>
                      <th>กิจกรรม</th>
                      <th>ชั่วโมง</th>
                    </tr>
                  </thead>
                  <tbody>
                    <tr>
                      <td><span class="mini-chip">จิตอาสา</span></td>
                      <td>จิตอาสาช่วยน้ำท่วม</td>
                      <td>12 ชม.</td>
                    </tr>
                    <tr>
                      <td><span class="mini-chip">ภาวะผู้นำ</span></td>
                      <td>ค่ายผู้นำเยาวชน รสบ.</td>
                      <td>8 ชม.</td>
                    </tr>
                    <tr>
                      <td><span class="mini-chip">วิชาการ</span></td>
                      <td>แข่งขันตอบปัญหาวิทยาศาสตร์</td>
                      <td>5 ชม.</td>
                    </tr>
                  </tbody>
                </table>
              </div>
              <div class="hero-card-footer">
                <div>สะสมชั่วโมงรวม: <strong>25 ชั่วโมง</strong></div>
                <div class="status-pill">สถานะ: พร้อมออกรายงาน</div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <!-- Section: แนวคิด -->
      <section id="about">
        <div class="container">
          <h2 class="section-title">2.1 หลักการและแนวคิดในการพัฒนาระบบ</h2>
          <p class="section-subtitle">
            ระบบนี้ออกแบบบนฐานแนวคิดการบริหารจัดการข้อมูลสารสนเทศทางการศึกษา การพัฒนาผู้เรียนอย่างรอบด้าน
            และแนวคิด Activity Transcript เพื่อให้ข้อมูลกิจกรรมกลายเป็นหลักฐานเชิงสมรรถนะที่นำไปใช้ได้จริง
          </p>

          <div class="feature-grid">
            <div class="card">
              <div class="card-icon">📊</div>
              <div class="card-title">Educational Data Management</div>
              <p class="card-text">
                ใช้ข้อมูลกิจกรรมในรูปแบบฐานข้อมูลดิจิทัลที่ถูกต้อง เป็นปัจจุบัน และตรวจสอบย้อนกลับได้
                รองรับการวิเคราะห์และการใช้ประโยชน์ด้านการบริหารจัดการข้อมูลนักเรียน
              </p>
            </div>
            <div class="card">
              <div class="card-icon">🧭</div>
              <div class="card-title">Holistic Development</div>
              <p class="card-text">
                มองผู้เรียนแบบรอบด้าน ทั้งด้านจิตอาสา ภาวะผู้นำ วิชาการ และคุณธรรมจริยธรรม
                ทำให้ Transcript กิจกรรมสะท้อนภาพตัวตนและสมรรถนะของผู้เรียนได้จริง
              </p>
            </div>
            <div class="card">
              <div class="card-icon">📄</div>
              <div class="card-title">Activity Transcript</div>
              <p class="card-text">
                แปลงข้อมูลกิจกรรมจาก Google Forms และ Spreadsheet
                ให้กลายเป็นเอกสาร “ทรานสคริปกิจกรรม” ที่มีรูปแบบมาตรฐานเดียวกันทั้งโรงเรียน
                พร้อมใช้ใน Portfolio และการศึกษาต่อ
              </p>
            </div>
          </div>
        </div>
      </section>

      <!-- Section: โครงสร้างระบบ -->
      <section id="features">
        <div class="container">
          <h2 class="section-title">2.3 โครงสร้างระบบรายงานผลการเข้าร่วมกิจกรรม</h2>
          <p class="section-subtitle">
            ใช้รหัสประจำตัวนักเรียนเป็นแกนกลาง เชื่อมโยงฐานข้อมูลนักเรียน ฐานข้อมูลกิจกรรม
            และระบบประมวลผลอัตโนมัติ เพื่อสร้าง Transcript ที่มีมาตรฐานเดียวกันทั้งโรงเรียน
          </p>

          <div class="feature-grid">
            <div class="card">
              <div class="card-icon">🧑‍🎓</div>
              <div class="card-title">1) ฐานข้อมูลนักเรียน</div>
              <p class="card-text">
                เก็บข้อมูลนักเรียนโดยใช้รหัสประจำตัวเป็นตัวระบุหลัก (Primary Key)
                ทำให้สามารถเชื่อมข้อมูลกิจกรรมย้อนกลับมาหานักเรียนแต่ละคนได้อย่างถูกต้อง
              </p>
            </div>
            <div class="card">
              <div class="card-icon">📚</div>
              <div class="card-title">2) ฐานข้อมูลกิจกรรม</div>
              <p class="card-text">
                แยกประเภทกิจกรรมออกเป็น 4 มิติ ได้แก่ ด้านจิตอาสา ภาวะผู้นำ วิชาการ
                และคุณธรรมจริยธรรม เพื่อให้การสะสมชั่วโมงมีโครงสร้างชัดเจน
              </p>
            </div>
            <div class="card">
              <div class="card-icon">⏱️</div>
              <div class="card-title">3) ระบบสะสมชั่วโมงอัตโนมัติ</div>
              <p class="card-text">
                เมื่อครูรับรองการเข้าร่วมกิจกรรม ระบบจะบันทึกและสะสมชั่วโมงแยกตามประเภทกิจกรรม
                โดยอัตโนมัติ ลดการคำนวณและตรวจสอบซ้ำด้วยมือ
              </p>
            </div>
            <div class="card">
              <div class="card-icon">🧮</div>
              <div class="card-title">4) ระบบประมวลผล Transcript</div>
              <p class="card-text">
                ประมวลผลข้อมูลกิจกรรมที่สะสมไว้ในแต่ละมิติ และสร้างเป็นทรานสคริปกิจกรรมรายบุคคล
                ซึ่งสามารถออกรายงานได้ทั้งในรูปแบบดิจิทัลและสำหรับพิมพ์
              </p>
            </div>
            <div class="card">
              <div class="card-icon">📤</div>
              <div class="card-title">5) การออกรายงานและเชื่อมต่อ</div>
              <p class="card-text">
                รองรับการส่งออกข้อมูลในรูปแบบไฟล์ (เช่น PDF / CSV) และการเชื่อมต่อกับระบบอื่นในอนาคต
                เช่น ระบบ SIS หรือระบบ Portfolio ดิจิทัลของโรงเรียน
              </p>
            </div>
            <div class="card">
              <div class="card-icon">🔐</div>
              <div class="card-title">6) การกำกับดูแลข้อมูล</div>
              <p class="card-text">
                กำหนดสิทธิ์การใช้งานตามบทบาท เช่น นักเรียน ครูที่ปรึกษา ผู้ดูแลระบบ
                เพื่อให้ข้อมูลมีความถูกต้องและปลอดภัยในการใช้งานจริง
              </p>
            </div>
          </div>
        </div>
      </section>

      <!-- Section: Workflow -->
      <section id="workflow">
        <div class="container">
          <h2 class="section-title">2.4 ขั้นตอนการทำงานของระบบ (System Workflow)</h2>
          <p class="section-subtitle">
            จากเดิมที่ครูต้องไล่ตรวจรูปจาก Google Forms ทีละรายการ
            ระบบใหม่ออกแบบให้การบันทึก รับรอง และออกรายงานทำได้เป็นลำดับที่ชัดเจนและลดภาระงานลงอย่างเห็นได้ชัด
          </p>

          <div class="workflow-grid">
            <div>
              <ol class="steps">
                <li>
                  <div>
                    <div class="step-title">นักเรียนเข้าร่วมกิจกรรมพัฒนาผู้เรียน</div>
                    <div class="step-text">
                      นักเรียนเข้าร่วมกิจกรรมจิตอาสา กิจกรรมภาวะผู้นำ วิชาการ หรือกิจกรรมอื่นที่โรงเรียนกำหนด
                      โดยมีผู้รับผิดชอบกิจกรรมบันทึกข้อมูลไว้เป็นหลักฐานเบื้องต้น
                    </div>
                  </div>
                </li>
                <li>
                  <div>
                    <div class="step-title">ผู้รับผิดชอบกิจกรรมบันทึกข้อมูลเข้าสู่ระบบ</div>
                    <div class="step-text">
                      บันทึกข้อมูลการเข้าร่วมกิจกรรมของนักเรียนโดยใช้รหัสประจำตัวนักเรียนเป็นตัวเชื่อมโยง
                      พร้อมระบุประเภทกิจกรรม วันเวลา และจำนวนชั่วโมง
                    </div>
                  </div>
                </li>
                <li>
                  <div>
                    <div class="step-title">ครูที่ปรึกษาหรือครูผู้รับผิดชอบตรวจสอบและรับรอง</div>
                    <div class="step-text">
                      ครูตรวจสอบความถูกต้องของข้อมูลและหลักฐานประกอบ จากนั้นจึงทำการ “รับรอง” การเข้าร่วมกิจกรรมผ่านระบบ
                    </div>
                  </div>
                </li>
                <li>
                  <div>
                    <div class="step-title">ระบบบันทึกและสะสมชั่วโมงกิจกรรมอัตโนมัติ</div>
                    <div class="step-text">
                      เมื่อมีการรับรอง ระบบจะอัปเดตชั่วโมงกิจกรรมของนักเรียน แยกตามประเภทกิจกรรมในฐานข้อมูลโดยอัตโนมัติ
                    </div>
                  </div>
                </li>
                <li>
                  <div>
                    <div class="step-title">ออกรายงาน Transcript กิจกรรมรายบุคคล</div>
                    <div class="step-text">
                      นักเรียนและครูสามารถสั่งออกรายงานทรานสคริปกิจกรรมได้ในรูปแบบเอกสารดิจิทัล
                      เพื่อนำไปใช้ประกอบแฟ้มสะสมผลงาน (Portfolio) หรือการรายงานผลต่อผู้บริหาร
                    </div>
                  </div>
                </li>
              </ol>
            </div>

            <div class="comparison-card">
              <h4>ตารางเปรียบเทียบ: ระบบเดิม vs ระบบ Activity Transcript</h4>
              <table class="comparison-table">
                <thead>
                  <tr>
                    <th>ประเด็น</th>
                    <th>ระบบเดิม (Google Forms + Sheet)</th>
                    <th>ระบบใหม่ (Activity Transcript)</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td>การบันทึกข้อมูล</td>
                    <td>นักเรียนกรอกเอง แนบรูปหลากหลายรูปแบบ</td>
                    <td>ผู้รับผิดชอบบันทึกผ่านรหัสนักเรียน โครงสร้างข้อมูลชัดเจน</td>
                  </tr>
                  <tr>
                    <td>การตรวจสอบ</td>
                    <td>ครูไล่ดูรูปทีละรายการ ภาระงานสูง</td>
                    <td>ครูตรวจเฉพาะข้อมูลที่เข้าระบบอย่างเป็นทางการ</td>
                  </tr>
                  <tr>
                    <td>การสะสมชั่วโมง</td>
                    <td>คำนวณและรวมชั่วโมงด้วยมือ</td>
                    <td>ระบบสะสมชั่วโมงแยกตามประเภทกิจกรรมอัตโนมัติ</td>
                  </tr>
                  <tr>
                    <td>รูปแบบรายงาน</td>
                    <td>ไม่มี Transcript กิจกรรมมาตรฐาน</td>
                    <td>มีทรานสคริปกิจกรรม พร้อมใช้ใน Portfolio นักเรียน</td>
                  </tr>
                  <tr>
                    <td>การใช้ประโยชน์ข้อมูล</td>
                    <td>ใช้เพื่อผ่านเกณฑ์กิจกรรมเป็นหลัก</td>
                    <td>ใช้เพื่อประเมินสมรรถนะและสนับสนุนการศึกษาต่อได้จริง</td>
                  </tr>
                </tbody>
              </table>
            </div>

          </div>
        </div>
      </section>

      <!-- Section: Example Transcript -->
      <section id="example">
        <div class="container">
          <h2 class="section-title">ตัวอย่างหน้าจอ Transcript กิจกรรม (Mockup)</h2>
          <p class="section-subtitle">
            ส่วนนี้เป็นตัวอย่างโครงหน้าจอ (UI Mockup) สำหรับใช้เป็นแนวทางออกแบบหน้าเว็บจริงของระบบ
            สามารถปรับแต่งต่อในโค้ด HTML / CSS หรือเฟรมเวิร์กที่ต้องการได้
          </p>

          <div class="transcript-layout">
            <div class="transcript-card">
              <div class="transcript-header">
                <div>
                  <div class="transcript-title">ทรานสคริปกิจกรรม – โรงเรียนรัตนโกสินทร์สมโภชบางเขน</div>
                  <div class="transcript-meta">
                    ชื่อนักเรียน: นายตัวอย่าง ระบบดีเยี่ยม | รหัส: 67890 | ระดับชั้น: ม.5/10
                  </div>
                </div>
                <div class="transcript-tag">รุ่นปีการศึกษา 2568</div>
              </div>
              <table class="transcript-table">
                <thead>
                  <tr>
                    <th>ประเภทกิจกรรม</th>
                    <th>ชื่อกิจกรรม</th>
                    <th>บทบาท</th>
                    <th>ชั่วโมง</th>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td>จิตอาสา</td>
                    <td>จิตอาสาช่วยน้ำท่วม จังหวัดสงขลา</td>
                    <td><span class="badge-soft">ผู้เข้าร่วม</span></td>
                    <td>12</td>
                  </tr>
                  <tr>
                    <td>ภาวะผู้นำ</td>
                    <td>ค่ายผู้นำนักเรียน รส.บ. รุ่นที่ 5</td>
                    <td><span class="badge-soft">ประธานกลุ่ม</span></td>
                    <td>8</td>
                  </tr>
                  <tr>
                    <td>วิชาการ</td>
                    <td>เข้าร่วมอบรมโครงงานวิทยาศาสตร์ระดับมัธยมศึกษา</td>
                    <td><span class="badge-soft">ผู้เข้าร่วม</span></td>
                    <td>5</td>
                  </tr>
                  <tr>
                    <td>คุณธรรมจริยธรรม</td>
                    <td>กิจกรรมวันสำคัญทางศาสนาในโรงเรียน</td>
                    <td><span class="badge-soft">จิตอาสา</span></td>
                    <td>3</td>
                  </tr>
                </tbody>
                <tfoot>
                  <tr>
                    <th colspan="3">รวมชั่วโมงกิจกรรมทั้งหมด</th>
                    <th>28</th>
                  </tr>
                </tfoot>
              </table>
            </div>

            <div class="sidebar-note">
              <strong>หมายเหตุสำหรับนักพัฒนา (สำหรับ GitHub)</strong>
              <ul>
                <li>โครงสร้างหน้านี้สามารถแยกออกเป็น component ย่อย ๆ ได้หากใช้ React / Vue</li>
                <li>ข้อมูลในตารางอาจดึงจากฐานข้อมูล หรือไฟล์ JSON ผ่าน API</li>
                <li>สามารถเพิ่มปุ่ม “ดาวน์โหลดเป็น PDF” หรือ “Export CSV” สำหรับใช้งานจริง</li>
                <li>แนะนำให้แยกไฟล์ <code>style.css</code> และ <code>script.js</code> เมื่อโปรเจกต์เติบโต</li>
              </ul>
            </div>
          </div>
        </div>
      </section>

      <!-- Section: Dev Note -->
      <section id="about-dev">
        <div class="container">
          <h2 class="section-title">สำหรับ GitHub และการพัฒนาต่อยอด</h2>
          <p class="section-subtitle">
            ส่วนนี้เป็นโน้ตสั้น ๆ สำหรับใช้ใน README ของ GitHub หรือสำหรับอธิบายต่อกับทีมพัฒนาระบบ
          </p>

          <div class="card">
            <div class="card-title">โครงสร้างพื้นฐานที่แนะนำ</div>
            <p class="card-text" style="margin-top: 0.4rem;">
              โปรเจกต์นี้สามารถเริ่มจาก static page (HTML + CSS + JS) และค่อยต่อยอดสู่ระบบฐานข้อมูลเต็มรูปแบบได้ภายหลัง
              เช่น:
            </p>
            <ul style="margin-top: 0.5rem; padding-left: 1.2rem; font-size: 0.86rem; color: var(--text-muted);">
              <li><strong>Frontend:</strong> HTML / CSS / JavaScript (หรือ React / Vue ตามความถนัด)</li>
              <li><strong>Backend (ทางเลือก):</strong> Node.js, Django, Laravel หรือ Firebase</li>
              <li><strong>Database:</strong> MySQL / PostgreSQL / Firestore / Supabase</li>
              <li><strong>Deployment:</strong> GitHub Pages (สำหรับ frontend) + Render / Railway / Firebase Hosting</li>
            </ul>
            <p class="card-text" style="margin-top: 0.6rem;">
              ในระยะเริ่มต้น สามารถใช้หน้าเว็บนี้เป็น<strong>หน้าแนะนำระบบ (Landing Page)</strong>
              และเพิ่มหน้าใหม่สำหรับหน้า Login / Dashboard นักเรียน / Dashboard ครูในขั้นถัดไปได้
            </p>
          </div>
        </div>
      </section>
    </main>

    <!-- Footer -->
    <footer>
      <div class="container">
        <div class="footer-inner">
          <div>
            © 2568 RSB Activity Transcript System — โปรเจกต์ต้นแบบเพื่อการบริหารกิจการนักเรียนด้วย ICT
          </div>
          <div>
            พัฒนาโดย <strong>นายวรกานต์ โอภาสวัฒนา</strong> | รายวิชา 2747745
          </div>
        </div>
      </div>
    </footer>
  </div>
</body>
</html>
