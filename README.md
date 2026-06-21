<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>I'm Anjalika Tharushee</title>
    <style>
        /* --- GitHub Dark Mode Theme Variables --- */
        :root {
            --bg-color: #0d1117;
            --card-bg: #0d1117;
            --border-color: #30363d;
            --text-main: #c9d1d9;
            --text-muted: #8b949e;
            --accent-cyan: #00f2fe;
            --accent-pink: #ff5e62;
            --accent-magenta: #e91e63;
            --font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            font-family: var(--font-family);
            padding: 40px 20px;
            display: flex;
            justify-content: center;
        }

        .container {
            width: 100%;
            max-width: 850px;
        }

        hr {
            border: 0;
            border-top: 1px solid var(--border-color);
            margin: 25px 0;
        }

        /* --- Header Section --- */
        .header {
            text-align: center;
            margin-bottom: 25px;
        }

        .avatar-container {
            margin-bottom: 15px;
        }

        .avatar-container img {
            width: 120px;
            height: auto;
        }

        .header h1 {
            font-size: 2.2rem;
            font-weight: 600;
            margin-bottom: 15px;
            color: #ffffff;
        }

        .header .subtitle {
            font-size: 1.15rem;
            font-weight: 600;
            color: #ffffff;
            margin-bottom: 15px;
        }

        /* Counter and Badges */
        .counter-badge {
            background-color: #21262d;
            border: 1px solid var(--border-color);
            border-radius: 4px;
            display: inline-flex;
            font-size: 0.75rem;
            overflow: hidden;
            margin-bottom: 15px;
        }

        .counter-label {
            background-color: #444;
            color: #fff;
            padding: 4px 8px;
        }

        .counter-value {
            background-color: #007ec6;
            color: #fff;
            padding: 4px 8px;
            font-weight: bold;
        }

        .follow-btn {
            background-color: #343a40;
            border: 1px solid var(--border-color);
            color: #ffffff;
            padding: 6px 16px;
            font-size: 0.8rem;
            font-weight: bold;
            letter-spacing: 1px;
            border-radius: 4px;
            display: inline-block;
            text-transform: uppercase;
        }

        /* --- Bio Layout Split --- */
        .bio-grid {
            display: grid;
            grid-template-columns: 1.2fr 1fr;
            gap: 30px;
            align-items: center;
            margin-top: 20px;
        }

        @media (max-width: 768px) {
            .bio-grid {
                grid-template-columns: 1fr;
            }
        }

        .bio-list {
            list-style: none;
        }

        .bio-list li {
            margin-bottom: 20px;
            line-height: 1.6;
            font-size: 0.95rem;
        }

        .bio-list strong {
            color: #ffffff;
        }

        .bio-graphic img {
            width: 100%;
            border-radius: 4px;
            display: block;
        }

        /* --- Global Grid Title Styling --- */
        .section-title {
            text-align: center;
            font-size: 1.2rem;
            font-weight: 600;
            margin-bottom: 20px;
            color: #ffffff;
        }

        /* --- Custom Badges Flexbox Layout --- */
        .badge-container {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
            justify-content: center;
            margin-bottom: 25px;
        }

        .badge {
            display: inline-flex;
            align-items: center;
            padding: 5px 10px;
            font-size: 0.72rem;
            font-weight: 800;
            color: #ffffff;
            border-radius: 3px;
            letter-spacing: 0.5px;
            text-transform: uppercase;
        }

        /* Connect Badge Brand Backgrounds */
        .bg-facebook  { background-color: #1877F2; }
        .bg-instagram { background-color: #E1306C; }
        .bg-linkedin  { background-color: #0077B5; }
        .bg-tiktok    { background-color: #000000; border: 1px solid #333; }
        .bg-x         { background-color: #000000; border: 1px solid #333; }
        .bg-email     { background-color: #D14836; }

        /* Tech Stack Badge Backgrounds */
        .bg-cpp         { background-color: #00599C; }
        .bg-css3        { background-color: #1572B6; }
        .bg-html5       { background-color: #E34F26; }
        .bg-dart        { background-color: #0175C2; }
        .bg-c           { background-color: #A8B9CC; color: #000; }
        .bg-javascript  { background-color: #F7DF1E; color: #000; }
        .bg-java        { background-color: #ED8B00; }
        .bg-php         { background-color: #777BB4; }
        .bg-terminal    { background-color: #4D4D4D; }
        .bg-firebase    { background-color: #FFCA28; color: #000; }
        .bg-oracle      { background-color: #F80000; }
        .bg-gcloud      { background-color: #4285F4; }
        .bg-nodejs      { background-color: #339933; }
        .bg-nextjs      { background-color: #000000; border: 1px solid #333; }
        .bg-web3        { background-color: #F16822; }
        .bg-wordpress   { background-color: #21759B; }
        .bg-tailwind    { background-color: #06B6D4; }
        .bg-apache      { background-color: #D22128; }
        .bg-nginx       { background-color: #009639; }
        .bg-mysql       { background-color: #4479A1; }
        .bg-postgres    { background-color: #4169E1; }
        .bg-canva       { background-color: #00C4CC; }
        .bg-figma       { background-color: #F24E1E; }
        .bg-protoio     { background-color: #101010; }
        .bg-sketch      { background-color: #F7A100; }
        .bg-tensorflow  { background-color: #FF6F00; }
        .bg-git         { background-color: #F05032; }
        .bg-github      { background-color: #181717; }
        .bg-gitlab      { background-color: #FC6D26; }
        .bg-docker      { background-color: #2496ED; }
        .bg-portfolio   { background-color: #8A2BE2; }
        .bg-amd         { background-color: #ED1C24; }

        /* --- GitHub Cards Flex & Layout Grid --- */
        .stats-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 15px;
            margin-bottom: 15px;
        }

        @media (max-width: 650px) {
            .stats-grid {
                grid-template-columns: 1fr;
            }
        }

        .stats-card {
            background-color: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 6px;
            padding: 22px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .stats-card h3 {
            color: var(--accent-cyan);
            font-size: 1.05rem;
            margin-bottom: 18px;
            font-weight: 600;
        }

        .stats-left p {
            font-size: 0.88rem;
            margin-bottom: 8px;
            color: var(--accent-magenta);
            font-weight: 500;
        }

        .stats-left p strong {
            color: var(--text-main);
            float: right;
            margin-left: 35px;
        }

        /* Radial Ring Indicator Simulation */
        .circle-container {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-left: 10px;
        }

        .circle-ring {
            width: 75px;
            height: 75px;
            border-radius: 50%;
            border: 5px solid #161b22;
            border-top-color: var(--accent-cyan);
            border-right-color: var(--accent-cyan);
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-size: 1.3rem;
            color: var(--accent-magenta);
        }

        /* Streak Columns Details Layout */
        .streak-row {
            display: flex;
            width: 100%;
            justify-content: space-around;
            text-align: center;
        }

        .streak-item {
            display: flex;
            flex-direction: column;
            justify-content: center;
            position: relative;
        }

        .streak-item:not(:last-child)::after {
            content: "";
            position: absolute;
            right: -25px;
            top: 15%;
            height: 70%;
            border-right: 1px solid var(--border-color);
        }

        .streak-num {
            font-size: 1.8rem;
            font-weight: bold;
            color: var(--accent-cyan);
        }

        .streak-num.total { color: var(--accent-cyan); }
        .streak-num.current { color: var(--accent-magenta); }
        .streak-num.longest { color: var(--accent-cyan); }

        .streak-label {
            font-size: 0.72rem;
            color: var(--accent-cyan);
            margin-top: 5px;
            font-weight: 500;
        }
        .streak-date {
            font-size: 0.65rem;
            color: var(--text-muted);
            margin-top: 4px;
        }

        /* --- Language Progress Component Box --- */
        .languages-card {
            background-color: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 6px;
            padding: 22px;
            max-width: 480px;
            margin: 0 auto 25px;
        }

        .languages-card h3 {
            color: var(--accent-cyan);
            font-size: 1.1rem;
            margin-bottom: 15px;
            font-weight: 600;
        }

        .progress-bar-wrapper {
            display: flex;
            height: 10px;
            border-radius: 5px;
            overflow: hidden;
            background-color: #161b22;
            margin: 15px 0 20px;
        }

        .progress-fill {
            height: 100%;
        }

        .lang-legend-grid {
            display: flex;
            justify-content: flex-start;
            gap: 20px;
            flex-wrap: wrap;
            font-size: 0.8rem;
        }

        .legend-pill {
            display: flex;
            align-items: center;
            gap: 6px;
            color: var(--text-main);
        }

        .legend-dot {
            width: 8px;
            height: 8px;
            border-radius: 50%;
        }
    </style>
</head>
<body>

    <div class="container">

        <!-- Header Block Layout Context -->
        <header class="header">
            <div class="avatar-container">
                <!-- Using a placeholder developer illustration matching your hacker avatar -->
                <img src="https://img.icons8.com/illustrations/external-pack-flat-symbols-tanah-basah/120/external-hacker-cyber-security-pack-flat-symbols-tanah-basah.png" alt="Hacker Profile Avatar">
            </div>
            <h1>Hi 👋, I'm Kalana Neranjana</h1>
            <p class="subtitle">Passionate IT Student | Exploring the Boundless World of Technology</p>
            
            <div>
                <div class="counter-badge">
                    <span class="counter-label">Profile views</span>
                    <span class="counter-value">229</span>
                </div>
            </div>

            <div>
                <span class="follow-btn">Follow @kalanak41832</span>
            </div>
        </header>

        <hr>

        <!-- Profile Metadata Splitting Grid Context -->
        <div class="bio-grid">
            <ul class="bio-list">
                <li>🔮 I'm currently working on: <strong>innovative software solutions like the ElderCare mobile app, Learnio, and my personal portfolio (kalana.is-a.dev)</strong></li>
                <li>🧑‍🤝‍🧑 I'm looking to collaborate on: <strong>creative web development projects and AI-driven tech solutions</strong></li>
                <li>🤝 I'm looking for help with: <strong>advanced database systems and mastering modern web frameworks</strong></li>
                <li>🌱 I'm currently learning: <strong>my BSc (Hons) in Software Engineering at CINEC Campus (focusing on Web Architectures, SQA, & DSA)</strong></li>
            </ul>
            
            <div class="bio-graphic">
                <!-- Recreated your yellow technical system schematic diagram box vector -->
                <img src="https://img.icons8.com/illustrations/monochrome/400/web-development.png" style="background-color: #f4e04d; padding: 10px;" alt="Tech Architecture Workspace Design">
            </div>
        </div>

        <hr>

        <!-- Social Media Section Badges -->
        <h2 class="section-title">🌐 Connect with me</h2>
        <div class="badge-container">
            <span class="badge bg-facebook">Facebook</span>
            <span class="badge bg-instagram">Instagram</span>
            <span class="badge bg-linkedin">Linkedin</span>
            <span class="badge bg-tiktok">TikTok</span>
            <span class="badge bg-x">X</span>
            <span class="badge bg-email">Email</span>
        </div>

        <!-- Comprehensive Tech Stack Section -->
        <h2 class="section-title">💻 Tech Stack</h2>
        <div class="badge-container">
            <span class="badge bg-cpp">C++</span>
            <span class="badge bg-css3">CSS3</span>
            <span class="badge bg-html5">HTML5</span>
            <span class="badge bg-dart">Dart</span>
            <span class="badge bg-c">C</span>
            <span class="badge bg-javascript">JavaScript</span>
            <span class="badge bg-java">Java</span>
            <span class="badge bg-php">PHP</span>
            <span class="badge bg-terminal">Windows Terminal</span>
            <span class="badge bg-firebase">Firebase</span>
            <span class="badge bg-oracle">Oracle</span>
            <span class="badge bg-gcloud">Google Cloud</span>
            <span class="badge bg-nodejs">Node.js</span>
            <span class="badge bg-nextjs">Next.js</span>
            <span class="badge bg-web3">Web3.js</span>
            <span class="badge bg-wordpress">WordPress</span>
            <span class="badge bg-tailwind">Tailwind CSS</span>
            <span class="badge bg-apache">Apache</span>
            <span class="badge bg-nginx">Nginx</span>
            <span class="badge bg-mysql">MySQL</span>
            <span class="badge bg-postgres">Postgres</span>
            <span class="badge bg-canva">Canva</span>
            <span class="badge bg-figma">Figma</span>
            <span class="badge bg-protoio">Proto.io</span>
            <span class="badge bg-sketch">Sketch</span>
            <span class="badge bg-tensorflow">TensorFlow</span>
            <span class="badge bg-git">Git</span>
            <span class="badge bg-github">GitHub</span>
            <span class="badge bg-gitlab">GitLab</span>
            <span class="badge bg-docker">Docker</span>
            <span class="badge bg-portfolio">Portfolio</span>
            <span class="badge bg-amd">AMD</span>
        </div>

        <hr>

        <!-- GitHub Metrics Component Display Workspace -->
        <h2 class="section-title">📊 GitHub Stats</h2>
        
        <div class="stats-grid">
            <!-- Metric Values Card -->
            <div class="stats-card">
                <div class="stats-left">
                    <h3>Kalana Neranjana's GitHub Stats</h3>
                    <p>Total Stars Earned: <strong>0</strong></p>
                    <p>Total Commits: <strong>61</strong></p>
                    <p>Total PRs: <strong>14</strong></p>
                    <p>Total Issues: <strong>0</strong></p>
                    <p>Contributed to (last year): <strong>1</strong></p>
                </div>
                <div class="circle-container">
                    <div class="circle-ring">C</div>
                </div>
            </div>

            <!-- Streak Counter Values Card -->
            <div class="stats-card">
                <div class="streak-row">
                    <div class="streak-item">
                        <span class="streak-num total">74</span>
                        <span class="streak-label">Total Contributions</span>
                        <span class="streak-date">Aug 11, 2024 - Present</span>
                    </div>
                    <div class="streak-item">
                        <span class="streak-num current">0</span>
                        <span class="streak-label">Current Streak</span>
                        <span class="streak-date">Jun 21</span>
                    </div>
                    <div class="streak-item">
                        <span class="streak-num longest">3</span>
                        <span class="streak-label">Longest Streak</span>
                        <span class="streak-date">Jul 3, 2025 - Jul 5, 2025</span>
                    </div>
                </div>
            </div>
        </div>

        <!-- Most Used Languages Component Box -->
        <div class="languages-card">
            <h3>Most Used Languages</h3>
            
            <div class="progress-bar-wrapper">
                <!-- Exact proportional alignment block setup matching data percentages -->
                <div class="progress-fill" style="width: 73.36%; background-color: #ff5e62;"></div>
                <div class="progress-fill" style="width: 14.37%; background-color: #f7df1e;"></div>
                <div class="progress-fill" style="width: 12.27%; background-color: #8a2be2;"></div>
            </div>

            <div class="lang-legend-grid">
                <div class="legend-pill">
                    <span class="legend-dot" style="background-color: #ff5e62;"></span>
                    <span>HTML 73.36%</span>
                </div>
                <div class="legend-pill">
                    <span class="legend-dot" style="background-color: #f7df1e;"></span>
                    <span>JavaScript 14.37%</span>
                </div>
                <div class="legend-pill">
                    <span class="legend-dot" style="background-color: #8a2be2;"></span>
                    <span>CSS 12.26%</span>
                </div>
            </div>
        </div>

    </div>

</body>
</html>

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
