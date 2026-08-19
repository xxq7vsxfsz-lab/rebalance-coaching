<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Re:Balance｜介護する人の生活を立て直すオンライン相談｜初回30分無料</title>
  <meta
    name="description"
    content="Re:Balanceは、介護する人が介護を続けながら自分の生活も守れるよう、仕事・家事・休息・身体の負担を一緒に見直し、生活を立て直すためのオンライン相談サービスです。理学療法士・保健医療学博士の有本くにひろが相談を担当します。"
  >

  <link rel="icon" type="image/png" href="favicon.png">

  <style>
    :root {
      /*
        Re:Balance 専用ブランドパレット
        1. Deep Navy   #17324D  信頼・専門性
        2. Calm Teal   #356B73  安心・落ち着き
        3. Mist Blue   #DCE7EA  やわらかさ
        4. Warm Ivory  #F7F4EE  温かい背景
        5. Soft Sand   #C7A56B  温もりのアクセント
      */
      --brand-navy: #17324D;
      --brand-teal: #356B73;
      --brand-mist: #DCE7EA;
      --brand-ivory: #F7F4EE;
      --brand-sand: #C7A56B;

      --bg: var(--brand-ivory);
      --surface: #ffffff;
      --text: var(--brand-navy);
      --muted: #5E6F79;
      --line: #D6DEE0;
      --accent: var(--brand-teal);
      --accent-dark: var(--brand-navy);
      --accent-2: var(--brand-mist);
      --soft: #EEF3F4;
      --cream: #FBF7F0;
      --max: 1120px;
      --radius: 24px;
      --shadow: 0 14px 36px rgba(23, 50, 77, 0.10);
    }

    * {
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      margin: 0;
      font-family:
        -apple-system,
        BlinkMacSystemFont,
        "Hiragino Sans",
        "Hiragino Kaku Gothic ProN",
        "Yu Gothic",
        "Noto Sans JP",
        sans-serif;
      color: var(--text);
      background: var(--bg);
      line-height: 1.75;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    img {
      max-width: 100%;
      display: block;
    }

    .container {
      width: min(calc(100% - 32px), var(--max));
      margin: 0 auto;
    }

    header {
      position: sticky;
      top: 0;
      z-index: 50;
      background: rgba(255, 255, 255, 0.94);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid rgba(217, 223, 218, 0.9);
    }

    .nav {
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 14px 0;
      gap: 20px;
    }

    .brand {
      font-family: Georgia, "Times New Roman", serif;
      font-weight: 700;
      font-size: 1.7rem;
      line-height: 1.1;
      color: var(--accent-dark);
      letter-spacing: 0.02em;
    }

    .brand span {
      display: block;
      font-size: 0.82rem;
      font-weight: 500;
      color: var(--muted);
      text-align: center;
      letter-spacing: 0.12em;
      margin-top: 2px;
    }

    .nav-links {
      display: flex;
      gap: 18px;
      flex-wrap: wrap;
      align-items: center;
      font-size: 0.94rem;
      font-weight: 700;
      color: var(--text);
    }

    .nav-links a:hover {
      color: var(--accent);
    }

    .nav-cta {
      background: var(--accent);
      color: #ffffff !important;
      padding: 10px 18px;
      border-radius: 999px;
      box-shadow: var(--shadow);
    }

    section {
      padding: 58px 0;
    }

    .hero {
      padding: 0 0 58px;
      background:
        radial-gradient(circle at 0% 15%, rgba(53, 107, 115, 0.14), transparent 28%),
        radial-gradient(circle at 85% 15%, rgba(199, 165, 107, 0.18), transparent 30%),
        linear-gradient(180deg, #FBF9F5 0%, #EEF3F4 100%);
      overflow: hidden;
    }

    .hero-main {
      display: grid;
      grid-template-columns: 1.05fr 0.95fr;
      gap: 30px;
      align-items: center;
      min-height: 600px;
      padding: 40px 0 24px;
      position: relative;
    }

    .hero-copy {
      position: relative;
      z-index: 2;
    }

    .hero-logo {
      margin-bottom: 24px;
    }

    .hero-logo-main {
      font-family: Georgia, "Times New Roman", serif;
      font-size: clamp(4rem, 8vw, 7.2rem);
      line-height: 0.95;
      color: var(--accent-dark);
      font-weight: 700;
      letter-spacing: 0.01em;
    }

    .hero-logo-sub {
      color: var(--accent);
      font-size: clamp(1rem, 2vw, 1.25rem);
      letter-spacing: 0.35em;
      font-weight: 700;
      margin-top: 14px;
      text-align: center;
      max-width: 620px;
    }

    .eyebrow {
      display: inline-block;
      background: rgba(255, 255, 255, 0.78);
      border: 1px solid #AFC6CB;
      color: var(--accent);
      padding: 8px 18px;
      border-radius: 999px;
      font-size: 0.94rem;
      font-weight: 800;
      margin-bottom: 18px;
    }

    h1 {
      font-size: clamp(2.2rem, 4.2vw, 3.9rem);
      line-height: 1.3;
      margin: 0 0 18px;
      letter-spacing: -0.02em;
      color: #17324D;
    }

    h1 .green {
      color: var(--accent);
    }

    h2 {
      font-size: clamp(1.7rem, 3vw, 2.4rem);
      line-height: 1.35;
      margin: 0 0 10px;
    }

    h3 {
      margin-top: 0;
      line-height: 1.4;
    }

    .lead {
      font-size: 1.04rem;
      color: var(--text);
      margin: 0 0 24px;
      font-weight: 600;
    }

    .lead .muted-line {
      color: var(--muted);
      font-weight: 500;
    }

    .cta-row {
      display: flex;
      gap: 14px;
      flex-wrap: wrap;
      margin: 22px 0 14px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 14px 24px;
      border-radius: 999px;
      font-weight: 800;
      transition: 0.25s ease;
      border: 1px solid transparent;
      text-align: center;
    }

    .btn-primary {
      background: var(--accent);
      color: #ffffff;
      box-shadow: var(--shadow);
    }

    .btn-secondary {
      background: rgba(255, 255, 255, 0.86);
      border-color: #AFC6CB;
      color: var(--text);
    }

    .btn-note {
      background: var(--accent-2);
      border-color: #C7D9DD;
      color: var(--accent);
    }

    .btn:hover {
      transform: translateY(-1px);
      opacity: 0.96;
    }

    .hero-meta {
      display: flex;
      gap: 18px;
      flex-wrap: wrap;
      color: var(--muted);
      font-weight: 700;
      font-size: 0.95rem;
      margin-top: 14px;
    }

    .hero-visual {
      position: relative;
      min-height: 520px;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .hero-visual::before {
      content: "";
      position: absolute;
      inset: 2% -12% 2% -10%;
      background:
        radial-gradient(
          circle at center,
          rgba(255, 255, 255, 0.9),
          rgba(255, 255, 255, 0.25) 60%,
          transparent 76%
        );
      z-index: 0;
    }

    .hero-profile-image {
      position: relative;
      z-index: 1;
      width: min(78%, 450px);
      border-radius: 28px;
      object-fit: cover;
      box-shadow: 0 18px 42px rgba(23, 50, 77, 0.14);
      border: 1px solid rgba(217, 223, 218, 0.85);
    }

    .profile-mini {
      position: absolute;
      z-index: 3;
      right: 0;
      bottom: 40px;
      width: min(84%, 310px);
      background: rgba(255, 255, 255, 0.92);
      border: 1px solid rgba(217, 223, 218, 0.9);
      border-radius: 14px;
      padding: 16px 20px;
      box-shadow: var(--shadow);
    }

    .profile-mini strong {
      display: block;
      font-size: 1.15rem;
      color: var(--accent-dark);
      margin-bottom: 4px;
    }

    .profile-mini span {
      display: block;
      font-size: 0.92rem;
      color: var(--text);
      font-weight: 700;
    }

    .problem-strip {
      margin-top: 18px;
      text-align: center;
    }

    .problem-strip h2 {
      color: var(--accent-dark);
      font-size: clamp(1.45rem, 2.6vw, 2rem);
      margin-bottom: 26px;
    }

    .problem-feature {
      display: grid;
      grid-template-columns: 0.85fr 1.15fr;
      gap: 22px;
      align-items: stretch;
      margin-bottom: 22px;
    }

    .problem-photo-wrap {
      min-height: 100%;
    }

    .problem-photo {
      width: 100%;
      height: 100%;
      min-height: 300px;
      object-fit: cover;
      border-radius: 20px;
      border: 1px solid var(--line);
      box-shadow: 0 8px 24px rgba(23, 50, 77, 0.08);
    }

    .problem-feature .problem-cards {
      grid-template-columns: repeat(2, 1fr);
      gap: 14px;
    }

    .problem-cta-row {
      display: flex;
      justify-content: center;
      margin-top: 18px;
    }

    .gain-visual {
      display: grid;
      grid-template-columns: 1.05fr 0.95fr;
      gap: 24px;
      align-items: center;
      background: var(--surface);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 24px;
      margin-bottom: 22px;
    }

    .gain-visual-copy h3 {
      font-size: clamp(1.25rem, 2.3vw, 1.7rem);
      margin-bottom: 10px;
      color: var(--accent-dark);
    }

    .gain-visual-copy p {
      margin-bottom: 0;
    }

    .gain-visual-image {
      width: 100%;
      height: 260px;
      object-fit: cover;
      border-radius: 18px;
      border: 1px solid var(--line);
    }

    .problem-cards {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 14px;
      align-items: stretch;
    }

    .problem-card {
      background: rgba(255, 255, 255, 0.88);
      border: 1px solid var(--line);
      border-radius: 18px;
      padding: 20px 14px;
      min-height: 140px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      box-shadow: 0 8px 24px rgba(23, 50, 77, 0.06);
      font-weight: 800;
    }

    .problem-icon {
      width: 44px;
      height: 44px;
      margin: 0 auto 10px;
      border-radius: 50%;
      background: var(--accent-2);
      color: var(--accent);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      font-size: 1.4rem;
      font-weight: 900;
    }

    .section-head {
      margin-bottom: 26px;
    }

    .section-head p {
      margin: 0;
      color: var(--muted);
      font-size: 1.02rem;
    }

    .grid-3 {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 18px;
    }

    .grid-2 {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 18px;
    }

    .card {
      background: var(--surface);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 24px;
    }

    .section-image {
      width: 100%;
      height: 220px;
      object-fit: cover;
      border-radius: 18px;
      margin-bottom: 16px;
      border: 1px solid var(--line);
    }

    .wide-image {
      width: 100%;
      height: 320px;
      object-fit: cover;
      border-radius: var(--radius);
      border: 1px solid var(--line);
      box-shadow: var(--shadow);
      margin-bottom: 28px;
    }

    .muted {
      color: var(--muted);
    }

    .problem-list,
    .gain-list,
    .faq-list {
      display: grid;
      gap: 14px;
    }

    .problem-item,
    .gain-item,
    .flow-item,
    .faq-item {
      background: var(--surface);
      border: 1px solid var(--line);
      border-radius: 16px;
      padding: 18px 20px;
    }

    .problem-item {
      position: relative;
      padding-left: 46px;
    }

    .problem-item::before {
      content: "✓";
      position: absolute;
      left: 18px;
      top: 18px;
      color: var(--accent);
      font-weight: 900;
    }

    .gain-item {
      display: flex;
      gap: 14px;
      align-items: flex-start;
    }

    .gain-icon {
      min-width: 34px;
      width: 34px;
      height: 34px;
      border-radius: 50%;
      background: var(--accent-2);
      color: var(--accent);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      font-weight: 900;
    }

    .flow-number {
      width: 36px;
      height: 36px;
      border-radius: 50%;
      background: var(--accent-2);
      color: var(--accent);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      font-weight: 800;
      margin-bottom: 10px;
    }

    .case-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 18px;
    }

    .case-grid-single {
      grid-template-columns: 1fr;
      max-width: 820px;
      margin: 0 auto;
    }

    .case-card {
      background: var(--surface);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      padding: 24px;
    }

    .case-label {
      display: inline-block;
      padding: 6px 10px;
      border-radius: 999px;
      background: var(--brand-mist);
      color: var(--brand-teal);
      font-size: 0.82rem;
      font-weight: 800;
      margin-bottom: 12px;
    }


    .case-note {
      margin-top: 18px;
      font-size: 0.9rem;
      color: var(--muted);
    }

    .profile {
      display: grid;
      grid-template-columns: 0.82fr 1.18fr;
      gap: 28px;
      align-items: stretch;
    }

    .profile-image-wrap {
      display: flex;
      align-items: center;
      justify-content: center;
      min-height: 100%;
    }

    .profile-photo {
      width: 100%;
      aspect-ratio: 4 / 5;
      max-height: 560px;
      object-fit: cover;
      object-position: center 42%;
      border-radius: 20px;
      border: 1px solid var(--line);
      box-shadow: var(--shadow);
      background: #ffffff;
    }

    .badge {
      display: inline-block;
      padding: 6px 10px;
      border-radius: 999px;
      background: var(--accent-2);
      color: var(--accent);
      font-size: 0.82rem;
      font-weight: 800;
      margin-bottom: 10px;
    }

    .price {
      font-size: 1.8rem;
      font-weight: 900;
      margin: 12px 0;
      color: var(--accent-dark);
    }

    .campaign {
      background: linear-gradient(180deg, #ffffff, #EEF3F4);
      border: 1px solid #C7D9DD;
    }

    .contact-box {
      text-align: center;
      padding: 36px;
      background: linear-gradient(180deg, #ffffff, #EEF3F4);
    }

    .small {
      font-size: 0.9rem;
      color: var(--muted);
    }

    .note {
      background: #fffaf0;
      border: 1px solid #DFD0B5;
      color: #6A5737;
      border-radius: 16px;
      padding: 16px 18px;
      margin-top: 18px;
      font-size: 0.95rem;
    }

    footer {
      padding: 28px 0 42px;
      color: var(--muted);
      font-size: 0.93rem;
    }

    @media (max-width: 980px) {
      .hero-main,
      .grid-3,
      .grid-2,
      .profile,
      .case-grid {
        grid-template-columns: 1fr;
      }

      .hero-main {
        min-height: auto;
      }

      .hero-visual {
        min-height: auto;
      }

      .hero-profile-image {
        width: min(88%, 440px);
      }

      .profile-mini {
        position: relative;
        right: auto;
        bottom: auto;
        width: 100%;
        margin-top: 14px;
      }

      .problem-feature,
      .gain-visual {
        grid-template-columns: 1fr;
      }

      .problem-photo {
        min-height: 260px;
        max-height: 360px;
      }

      .problem-cards {
        grid-template-columns: repeat(2, 1fr);
      }

      .floating-cta {
        width: 100%;
        height: auto;
        border-radius: 18px;
        padding: 18px;
      }

      .profile-photo {
        width: min(100%, 520px);
        margin: 0 auto;
      }
    }

    @media (max-width: 700px) {
      .nav {
        flex-direction: column;
        align-items: flex-start;
      }

      .nav-links {
        gap: 12px;
        font-size: 0.88rem;
      }

      .nav-cta {
        width: 100%;
        text-align: center;
      }

      .hero-logo-main {
        font-size: 3.6rem;
      }

      .hero-logo-sub {
        text-align: left;
        letter-spacing: 0.22em;
      }

      .btn {
        width: 100%;
      }

      .cta-row {
        flex-direction: column;
      }
      .problem-feature .problem-cards,
      .problem-cards {
        grid-template-columns: 1fr;
      }

      .gain-visual-image {
        height: 220px;
      }

      .wide-image {
        height: 240px;
      }

      .section-image {
        height: 200px;
      }

      .profile-photo {
        max-height: 520px;
      }

      section {
        padding: 44px 0;
      }
    }
  </style>
</head>

<body>
  <header>
    <div class="container nav">
      <a href="#" class="brand">
        Re:Balance
        <span>ー介護者サポートー</span>
      </a>

      <nav class="nav-links" aria-label="メインナビゲーション">
        <a href="#problem">お悩み</a>
        <a href="#gain">相談内容</a>
        <a href="#cases">相談例</a>
        <a href="#service">サービス・料金</a>
        <a href="#profile">プロフィール</a>
        <a href="#faq">FAQ</a>
        <a href="#contact">申し込み</a>
        <a
          class="nav-cta"
          href="https://forms.gle/f9Ps6GVnfz3L6eC47"
          target="_blank"
          rel="noopener"
        >
          初回30分無料で相談してみる
        </a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container">
        <div class="hero-main">
          <div class="hero-copy">
            <div class="hero-logo">
              <div class="hero-logo-main">Re:Balance</div>
              <div class="hero-logo-sub">ー 介護者サポート ー</div>
            </div>

            <div class="eyebrow">初回オンライン相談 30分無料</div>

            <h1>
              介護を続けながら、<br>
              <span class="green">自分の生活も守る</span>ために。
            </h1>

            <p class="lead">
              家族の介護が始まると、仕事、家事、休息、自分の時間まで、<br>
              少しずつ生活のペースが崩れてしまうことがあります。<br>
              <span class="muted-line">
                介護をひとりで抱え込まないために、家族への頼り方、仕事との両立、休む時間のつくり方に加え、理学療法士の視点から身体の負担を減らす工夫も一緒に考えます。
              </span>
            </p>

            <div class="cta-row">
              <a
                class="btn btn-primary"
                href="https://forms.gle/f9Ps6GVnfz3L6eC47"
                target="_blank"
                rel="noopener"
              >
                初回30分無料で相談してみる
              </a>

              <a class="btn btn-secondary" href="#service">
                料金・サービスを見る
              </a>
            </div>

            <div class="hero-meta">
              <span>オンラインで実施します</span>
              <span>主に土日、一部平日夜に対応</span>
            </div>
          </div>

          <div class="hero-visual">
            <img
              src="hero-profile.png"
              alt="介護者サポートを行う有本くにひろのイラスト"
              class="hero-profile-image"
              fetchpriority="high"
            >

            <div class="profile-mini">
              <strong>有本くにひろ（アリ先生）</strong>
              <span>Re:Balance 代表</span>
              <span>理学療法士・保健医療学博士</span>
              <span>在宅リハビリの経験をもとに、介護する方の生活と身体を支えます。</span>
            </div>
          </div>
        </div>

        <div id="problem" class="problem-strip">
          <h2>介護で、こんな不安や疲れを感じていませんか？</h2>

          <div class="problem-feature">
            <div class="problem-photo-wrap">
              <img
                src="family-care-image.png"
                alt="ベッド上で上体を起こした母親に家族が寄り添う介護のイメージ"
                class="problem-photo"
                loading="lazy"
              >
            </div>

            <div class="problem-cards">
              <div class="problem-card">
                <div class="problem-icon">人</div>
                一人で介護を<br>抱えるのが不安
              </div>

              <div class="problem-card">
                <div class="problem-icon">体</div>
                介護で体の疲れが<br>続いている
              </div>

              <div class="problem-card">
                <div class="problem-icon">仕</div>
                介護と仕事の<br>両立に不安がある
              </div>

              <div class="problem-card">
                <div class="problem-icon">休</div>
                自分の時間を取ることに<br>罪悪感がある
              </div>
            </div>
          </div>

          <div class="problem-cta-row">
            <a
              class="btn btn-primary"
              href="https://forms.gle/f9Ps6GVnfz3L6eC47"
              target="_blank"
              rel="noopener"
            >
              初回30分無料で相談してみる
            </a>
          </div>
        </div>
      </div>
    </section>

    <section id="gain">
      <div class="container">
        <div class="section-head">
          <h2>相談では、こんなことを一緒に考えます</h2>
          <p>
            今いちばん困っていることから、生活の中で実際に変えられることを一つずつ考えます。
          </p>
        </div>

        <div class="gain-visual">
          <div class="gain-visual-copy">
            <div class="case-label">理学療法士の視点も活かします</div>
            <h3>介護する人の「生活」と「身体」の両方を見ます</h3>
            <p class="muted">
              家族への頼り方や仕事との両立だけでなく、介助による腰や肩の負担、
              休み方、姿勢など、身体への負担を減らす工夫も一緒に考えます。
            </p>
          </div>
          <div class="gain-visual-image-wrap">
            <img
              src="body-care-image.png"
              alt="介護による腰や身体の負担を感じている人のイメージ"
              class="gain-visual-image"
              loading="lazy"
            >
          </div>
        </div>

        <div class="grid-2">
          <div class="card">
            <div class="gain-list">
              <div class="gain-item">
                <div class="gain-icon">1</div>
                <div>
                  <strong>家族や介護サービスに頼れることを考える</strong>
                  <div class="muted">
                    自分で抱えていることの中から、家族や周囲に任せられること、利用できるサービスを確認します。
                  </div>
                </div>
              </div>

              <div class="gain-item">
                <div class="gain-icon">2</div>
                <div>
                  <strong>介護・仕事・家事の優先順位を考える</strong>
                  <div class="muted">
                    「全部やる」前提を見直し、今やること、任せること、後回しにすることを一緒に決めます。
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="card">
            <div class="gain-list">
              <div class="gain-item">
                <div class="gain-icon">3</div>
                <div>
                  <strong>休む時間や自分の時間を確保する方法を考える</strong>
                  <div class="muted">
                    休息や自分の用事を「時間が余ったら」ではなく、生活の中にどう確保するかを考えます。
                  </div>
                </div>
              </div>

              <div class="gain-item">
                <div class="gain-icon">4</div>
                <div>
                  <strong>理学療法士の視点から、身体の負担を減らす工夫を考える</strong>
                  <div class="muted">
                    介助の仕方や姿勢、休み方など、日常生活の中で取り入れられる方法を一緒に考えます。
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="cta-row">
          <a
            class="btn btn-primary"
            href="https://forms.gle/f9Ps6GVnfz3L6eC47"
            target="_blank"
            rel="noopener"
          >
            初回30分無料で相談してみる
          </a>
        </div>
      </div>
    </section>

    <section id="change">
      <div class="container">
        <img
          src="online-session-image.png"
          alt="オンライン相談後に少し気持ちが軽くなった女性のイメージ"
          class="wide-image"
          loading="lazy"
        >

        <div class="section-head">
          <h2>相談すると、こんな変化を目指します</h2>
          <p>
            すべてを一度に変えるのではなく、今の生活でできるところから少しずつ変えていきます。
          </p>
        </div>

        <div class="card">
          <div class="problem-list">
            <div class="problem-item">一人で抱え込まず、頼れるところを頼れる</div>
            <div class="problem-item">仕事・家事・介護の優先順位が見える</div>
            <div class="problem-item">休む時間や自分の時間を確保できる</div>
            <div class="problem-item">身体の負担に早めに気づき、無理を続ける前に調整できる</div>
            <div class="problem-item">今、何から始めればよいかが分かる</div>
          </div>
        </div>
      </div>
    </section>

    <section id="cases">
      <div class="container">
        <div class="section-head">
          <h2>たとえば、こんなご相談</h2>
          <p>
            ご相談内容をイメージしていただくための一例です。
          </p>
        </div>

        <div class="case-grid case-grid-single">
          <div class="case-card">
            <div class="case-label">想定例</div>
            <h3>仕事を続けながら、家族の介護をしている50代の方</h3>
            <p class="muted">
              仕事を続けながら母親を介護。休日も家事と介護で終わり、腰痛も続いている。
              「自分がやらなければ」と思い、家族にもなかなか頼れず、自分の時間がほとんど取れない。
            </p>
            <p class="muted">
              このような場合、家族に頼れること、介護サービスの活用、仕事との両立、
              休む時間の確保、身体の負担を減らす工夫など、今の生活で変えられるところから一緒に考えます。
            </p>
          </div>
        </div>

        <p class="case-note">
          ※上記はサービス内容をイメージしていただくための想定例であり、実際のお客様の声・事例ではありません。
        </p>
      </div>
    </section>

    <section id="service">
      <div class="container">
        <div class="section-head">
          <h2>サービス内容・料金</h2>
          <p>
            初めての方が相談しやすいよう、初回は30分無料でお話を伺います。
          </p>
        </div>

        <div class="grid-2">
          <div class="card campaign">
            <div class="badge">初めての方へ</div>
            <h3>初回オンライン相談</h3>
            <p class="muted">
              介護・仕事・家事・休息・身体の負担など、現在の生活状況をお聞きし、
              どこから見直すと負担を減らせそうかを一緒に確認します。
            </p>
            <div class="price">30分 無料</div>
            <p class="small">
              初めての方向けの導入相談です。
              ご感想をいただいた方は、次回セッションを500円割引でご利用いただけます。
            </p>
            <a
              class="btn btn-primary"
              href="https://forms.gle/f9Ps6GVnfz3L6eC47"
              target="_blank"
              rel="noopener"
              style="width: 100%; margin-top: 16px;"
            >
              初回30分無料で相談してみる
            </a>
          </div>

          <div class="card">
            <div class="badge">2回目以降</div>
            <h3>個別相談</h3>
            <p class="muted">
              介護・仕事・家事・休息の優先順位を見直し、
              今の生活の中で実行できる具体的な方法を一緒に考えます。
            </p>
            <div class="price">60分 12,000円</div>
            <p class="small">
              2回目以降の単発相談料金です。
              主に土日、一部平日夜に対応しています。
            </p>
            <a
              class="btn btn-secondary"
              href="https://b-book.run/@rebalance.selfcare-c18a0996429f807c"
              target="_blank"
              rel="noopener"
              style="width: 100%; margin-top: 16px;"
            >
              2回目以降の予約をする
            </a>
          </div>
        </div>

        <div class="note">
          ※本サービスは相談によるサポートであり、医療行為や診断を行うものではありません。
          必要に応じて、医療機関や地域包括支援センター等の専門機関の利用をご検討ください。
        </div>
      </div>
    </section>

    <section id="flow">
      <div class="container">
        <div class="section-head">
          <h2>相談の流れ</h2>
          <p>
            初めての方でも安心して相談できるよう、シンプルな流れにしています。
          </p>
        </div>

        <div class="grid-2">
          <div class="flow-item">
            <div class="flow-number">1</div>
            <strong>フォームからお申し込み</strong>
            <div class="muted">
              現在のお悩みや相談したいことをご記入いただきます。
            </div>
          </div>

          <div class="flow-item">
            <div class="flow-number">2</div>
            <strong>日程調整</strong>
            <div class="muted">
              ご都合の良い日時を確認し、オンライン相談をご案内します。
            </div>
          </div>

          <div class="flow-item">
            <div class="flow-number">3</div>
            <strong>オンライン相談</strong>
            <div class="muted">
              今の状況や悩みをお聞きし、一緒に考えます。
            </div>
          </div>

          <div class="flow-item">
            <div class="flow-number">4</div>
            <strong>行動の具体化</strong>
            <div class="muted">
              相談後に何をどう実行するかを、無理のない形で明確にします。
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="profile">
      <div class="container">
        <div class="section-head">
          <h2>相談を担当します</h2>
          <p>
            医療・教育・在宅支援の経験を土台に、
            介護を続けながら自分の生活も守れるよう、暮らしの組み直しを一緒に考えます。
          </p>
        </div>

        <div class="profile">
          <div class="profile-image-wrap">
            <img
              src="profile-online.png"
              alt="オンラインで介護相談を行う有本くにひろ"
              class="profile-photo"
              loading="lazy"
            >
          </div>

          <div class="card">
            <div style="display: flex; gap: 8px; flex-wrap: wrap; margin-bottom: 14px;">
              <span class="badge">介護者の心身サポーター</span>
              <span class="badge">理学療法士</span>
              <span class="badge">保健医療学博士</span>
            </div>

            <h3 style="font-size: 1.9rem; margin-bottom: 8px;">
              有本くにひろ（アリ先生）
            </h3>

            <p
              style="
                font-weight: 800;
                margin-top: 0;
                margin-bottom: 16px;
                color: var(--accent);
              "
            >
              Re:Balance 代表
            </p>

            <p>
              理学療法士として在宅リハビリテーションの現場で、
              多くの利用者様とご家族に関わってきました。
              その中で、介護を支える人ほど、自分の心身を後回しにしやすい現実を
              数多く見てきました。
            </p>

            <p>
              理学療法士養成校教員として人材育成に携わり、
              保健医療学博士として専門性を深めてきました。
              現場感のある理解と専門的な視点の両方を活かし、
              介護・仕事・家事・休息・身体の負担を一緒に見直し、
              介護を続けながら自分の生活も守れる形へ立て直すための相談を行っています。
            </p>

            <div class="cta-row">
              <a
                class="btn btn-primary"
                href="https://forms.gle/f9Ps6GVnfz3L6eC47"
                target="_blank"
                rel="noopener"
              >
                初回30分無料で相談してみる
              </a>

              <a
                class="btn btn-secondary"
                href="https://www.instagram.com/arimoto.coach/"
                target="_blank"
                rel="noopener"
              >
                Instagramを見る
              </a>

              <a
                class="btn btn-note"
                href="https://note.com/rebalance_care08"
                target="_blank"
                rel="noopener"
              >
                noteを読む
              </a>
            </div>

            <p class="small">
              初回オンライン相談30分無料／オンライン対応／主に土日対応
            </p>
          </div>
        </div>
      </div>
    </section>

    <section id="faq">
      <div class="container">
        <div class="section-head">
          <h2>よくあるご質問</h2>
          <p>初めての方からよくいただくご質問をまとめています。</p>
        </div>

        <div class="faq-list">
          <div class="faq-item">
            <strong>Q. 相談では何を話せばよいですか？</strong>
            <div class="muted">
              A. まとまっていなくても大丈夫です。
              今感じていることや困っていることから一緒に考えていきます。
            </div>
          </div>

          <div class="faq-item">
            <strong>Q. 介護のこと以外でも相談できますか？</strong>
            <div class="muted">
              A. はい。行動習慣、働き方、人間関係など、
              介護と関連するテーマも含めてご相談いただけます。
            </div>
          </div>

          <div class="faq-item">
            <strong>Q. オンラインが苦手でも大丈夫ですか？</strong>
            <div class="muted">
              A. 事前に接続方法をご案内します。
              できるだけ不安なく参加できるよう配慮します。
            </div>
          </div>

          <div class="faq-item">
            <strong>Q. 医療行為や治療相談はできますか？</strong>
            <div class="muted">
              A. 本サービスは相談によるサポートであり、
              医療行為や診断を行うものではありません。
              必要に応じて適切な医療機関等の利用をご検討ください。
            </div>
          </div>

          <div class="faq-item">
            <strong>Q. 家族介護を始めたばかりでも相談できますか？</strong>
            <div class="muted">
              A. はい。介護が始まったばかりで
              何から考えればよいかわからない方にも対応しています。
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="contact">
      <div class="container">
        <div class="card contact-box">
          <div class="section-head">
            <h2>介護で崩れた生活のペースを、少しずつ立て直しませんか。</h2>
            <p>
              初回相談は30分無料です。
              介護・仕事・家事・身体の疲れなど、今いちばん困っていることからお聞きします。
            </p>
          </div>

          <div class="cta-row" style="justify-content: center;">
            <a
              class="btn btn-primary"
              href="https://forms.gle/f9Ps6GVnfz3L6eC47"
              target="_blank"
              rel="noopener"
            >
              初回30分無料で相談してみる
            </a>

            <a
              class="btn btn-secondary"
              href="https://www.instagram.com/arimoto.coach/"
              target="_blank"
              rel="noopener"
            >
              Instagramを見る
            </a>

            <a
              class="btn btn-note"
              href="https://note.com/rebalance_care08"
              target="_blank"
              rel="noopener"
            >
              noteを読む
            </a>
          </div>

          <p class="small">
            お問い合わせには通常2〜3日以内に返信いたします。
          </p>
        </div>
      </div>
    </section>

    <section id="privacy">
      <div class="container">
        <div class="card">
          <div class="section-head">
            <h2>プライバシーポリシー</h2>
            <p>
              安心してご相談いただくために、
              個人情報の取り扱いについて明示しています。
            </p>
          </div>

          <p>
            お問い合わせ時にご提供いただいた氏名・メールアドレス・ご相談内容は、
            返信およびサービス提供に必要な範囲でのみ利用します。
          </p>

          <p>
            取得した個人情報は、法令に基づく場合を除き、
            本人の同意なく第三者へ提供しません。
          </p>

          <p>
            個人情報の管理には十分配慮し、安全に取り扱います。
          </p>

          <p>お問い合わせ：rebalance.selfcare@gmail.com</p>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <div>© Re:Balance</div>
      <div class="small">
        このサイトは、家族を介護している方・介護やリハビリの仕事をしている方向けのオンライン相談サービスの案内ページです。
      </div>
    </div>
  </footer>
</body>
</html>
