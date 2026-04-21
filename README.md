<!-- PROFILE README - MOATHKUDOSENSE_SPEC | NEUMORPHIC-DARK ULTIMATE EDITION -->
<div align="center">
  <!-- HEADER SVG مع تأثير Neumorphic ثلاثي الأبعاد -->
  <svg width="880" height="220" viewBox="0 0 880 220" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stop-color="#1e1e2e" />
        <stop offset="100%" stop-color="#0a0a0f" />
      </linearGradient>
      <filter id="neumorphBig" x="-10%" y="-10%" width="120%" height="120%">
        <feDropShadow dx="12" dy="12" stdDeviation="10" flood-color="#000000" flood-opacity="0.8"/>
        <feDropShadow dx="-6" dy="-6" stdDeviation="8" flood-color="#3a3a4e" flood-opacity="0.3"/>
      </filter>
    </defs>
    <rect width="880" height="220" fill="url(#bgGrad)" rx="35" filter="url(#neumorphBig)" />
    <text x="440" y="85" font-family="'Segoe UI', monospace" font-size="48" fill="#ffffff" text-anchor="middle" font-weight="bold" letter-spacing="3">MOATH · معاذ</text>
    <text x="440" y="130" font-family="monospace" font-size="20" fill="#c792ea" text-anchor="middle">System Modder · Firmware Surgeon · Lua Alchemist</text>
    <text x="440" y="165" font-family="monospace" font-size="14" fill="#a0a0b0" text-anchor="middle">🔧 Sana'a, Yemen | 🎓 CS Candidate 2026 | 🧠 Low-Level Enthusiast</text>
    <text x="440" y="195" font-family="monospace" font-size="12" fill="#8888aa" text-anchor="middle"> </text>
  </svg>
</div>

<!-- شريط الأدوات الذكي (Neumorphic Table) -->
<div align="center">
  <table style="background-color:#181828; border-radius:28px; padding:14px; box-shadow: 10px 10px 20px #0a0a0f, -8px -8px 18px #2a2a3a;">
    <tr>
      <td>⚡ <b>Core</b> : Lua · Python · PowerShell · C · Rust(learning)</td>
      <td>🛠️ <b>Firmware</b> : ESP8266/32 · OpenWRT · U-Boot</td>
      <td>🎨 <b>UI Obsession</b> : Neumorphism · Soft Shading · Terminal aesthetics</td>
    </tr>
    <tr>
      <td>🌐 <b>Net. Ops</b> : MikroTik · YemNet optimization · Custom QoS</td>
      <td>📦 <b>Tools</b> : Neovim · Git Hooks · GitHub Actions</td>
      <td>🎮 <b>HoYoverse</b> : Genshin · HSR · ZZZ (theorycrafter)</td>
    </tr>
  </table>
</div>

<!-- القسم الاحترافي الفريد 1: حالة الشبكة في اليمن (بينغ وهمي لكنه واقعي) -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Sana'a Network Status | Live Monitoring</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: linear-gradient(145deg, #0b1120 0%, #0a0f1a 100%);
            font-family: 'Inter', 'Segoe UI', system-ui, -apple-system, BlinkMacSystemFont, 'Roboto', sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 2rem;
        }

        /* card container */
        .network-card {
            max-width: 760px;
            width: 100%;
            background: rgba(12, 18, 28, 0.75);
            backdrop-filter: blur(2px);
            border-radius: 2rem;
            border: 1px solid rgba(66, 212, 182, 0.2);
            box-shadow: 0 25px 45px -12px rgba(0, 0, 0, 0.6), 0 0 0 0.5px rgba(66, 212, 182, 0.1) inset;
            overflow: hidden;
            transition: all 0.2s ease;
        }

        /* header area */
        .status-header {
            background: rgba(0, 0, 0, 0.45);
            padding: 1.4rem 2rem;
            border-bottom: 1px solid rgba(66, 212, 182, 0.25);
            display: flex;
            justify-content: space-between;
            align-items: baseline;
            flex-wrap: wrap;
            gap: 0.75rem;
        }

        .title-section h1 {
            font-size: 1.55rem;
            font-weight: 600;
            letter-spacing: -0.3px;
            background: linear-gradient(135deg, #ffffff 0%, #b9f3ff 100%);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
        }

        .title-section .badge-live {
            display: inline-block;
            background: #0f2c2a;
            padding: 0.2rem 0.7rem;
            border-radius: 40px;
            font-size: 0.7rem;
            font-weight: 500;
            margin-left: 0.75rem;
            color: #2dd4bf;
            border: 0.5px solid #2dd4bf60;
            vertical-align: middle;
        }

        .sub {
            font-size: 0.75rem;
            color: #8b9bb5;
            margin-top: 0.25rem;
            letter-spacing: 0.2px;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .update-marker {
            font-family: monospace;
            background: #111a22;
            padding: 0.2rem 0.65rem;
            border-radius: 20px;
            font-size: 0.7rem;
            color: #6c86a3;
        }

        /* table style */
        .table-wrapper {
            overflow-x: auto;
            padding: 0 0.25rem;
        }

        .network-table {
            width: 100%;
            border-collapse: separate;
            border-spacing: 0;
            background: transparent;
        }

        .network-table th {
            text-align: left;
            padding: 1.2rem 1.5rem 0.7rem 1.8rem;
            font-weight: 500;
            font-size: 0.7rem;
            text-transform: uppercase;
            letter-spacing: 1.2px;
            color: #6d86a8;
            background: transparent;
            border-bottom: 1px solid rgba(45, 212, 191, 0.2);
        }

        .network-table td {
            padding: 1rem 1.5rem 1rem 1.8rem;
            font-size: 0.95rem;
            border-bottom: 1px solid rgba(45, 212, 191, 0.08);
            color: #eef4ff;
            font-weight: 450;
        }

        .service-name {
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .indicator {
            width: 8px;
            height: 8px;
            border-radius: 10px;
            display: inline-block;
            box-shadow: 0 0 4px currentColor;
        }

        .indicator.green {
            background: #2dd4bf;
            box-shadow: 0 0 6px #2dd4bf;
        }
        .indicator.yellow {
            background: #facc15;
            box-shadow: 0 0 5px #facc15;
        }
        .indicator.red {
            background: #f87171;
            box-shadow: 0 0 5px #f87171;
        }
        .indicator.gray {
            background: #5b6e8c;
        }

        .ping-value {
            font-family: 'JetBrains Mono', 'Fira Code', monospace;
            background: #0f1620;
            padding: 0.2rem 0.6rem;
            border-radius: 28px;
            font-size: 0.8rem;
            font-weight: 500;
            display: inline-block;
            letter-spacing: 0.2px;
            color: #b9e2e0;
        }

        .status-badge {
            font-size: 0.7rem;
            font-weight: 500;
            padding: 0.2rem 0.65rem;
            border-radius: 40px;
            background: #111c24;
            display: inline-block;
            color: #bcd0f0;
        }

        .status-badge.stable {
            background: #0b2a2a;
            color: #5eead4;
            border-left: 2px solid #2dd4bf;
        }
        .status-badge.unstable {
            background: #2c1f1a;
            color: #fda4af;
            border-left: 2px solid #f87171;
        }
        .status-badge.moderate {
            background: #2a281c;
            color: #fde047;
            border-left: 2px solid #facc15;
        }
        .status-badge.perfect {
            background: #0b2a2a;
            color: #a7f3d0;
            border-left: 2px solid #2dd4bf;
        }

        .uptime-row {
            font-size: 0.75rem;
            color: #94a9ce;
        }

        .latency-grade {
            font-family: monospace;
            font-weight: 700;
            background: linear-gradient(145deg, #1f2a3a, #141e2c);
            padding: 0.25rem 0.7rem;
            border-radius: 30px;
            font-size: 0.75rem;
            letter-spacing: 1px;
        }

        .footer-note {
            background: #03060c70;
            padding: 0.9rem 2rem;
            border-top: 1px solid rgba(66, 212, 182, 0.15);
            font-size: 0.7rem;
            color: #5e7897;
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .live-sim {
            font-family: monospace;
            background: #0f1722;
            padding: 0.2rem 0.8rem;
            border-radius: 20px;
            font-size: 0.65rem;
            color: #2dd4bf;
        }

        @media (max-width: 580px) {
            body {
                padding: 1rem;
            }
            .network-table th, .network-table td {
                padding: 0.85rem 1rem 0.85rem 1.2rem;
            }
            .status-header {
                padding: 1rem 1.2rem;
            }
            .title-section h1 {
                font-size: 1.2rem;
            }
        }
    </style>
</head>
<body>
<div class="network-card">
    <div class="status-header">
        <div class="title-section">
            <h1>
                Sana'a Network Status 
                <span class="badge-live">LIVE SIMULATION</span>
            </h1>
            <div class="sub">
                <span>🔌 core telemetry · realtime metrics</span>
                <span class="update-marker">⏱️ update: 5s drift</span>
            </div>
        </div>
        <div class="live-sim">
            🌐 yemen backbone
        </div>
    </div>

    <div class="table-wrapper">
        <table class="network-table">
            <thead>
                <tr>
                    <th>Service / Endpoint</th>
                    <th>Latency</th>
                    <th>Status</th>
                    <th>Uptime / Grade</th>
                </tr>
            </thead>
            <tbody>
                <!-- yemen.net.ye - IPv4 -->
                <tr>
                    <td class="service-name">
                        <span class="indicator green"></span>
                        yemen.net.ye
                        <span style="font-size:0.65rem; background:#0f1822; padding:2px 6px; border-radius:20px;">IPv4</span>
                    </td>
                    <td><span class="ping-value">43 ms</span></td>
                    <td><span class="status-badge stable">● stable</span></td>
                    <td class="uptime-row">uptime: 99.2%</td>
                </tr>
                <!-- yemen.net.ye - IPv6 -->
                <tr>
                    <td class="service-name">
                        <span class="indicator red"></span>
                        yemen.net.ye
                        <span style="font-size:0.65rem; background:#0f1822; padding:2px 6px; border-radius:20px;">IPv6</span>
                    </td>
                    <td><span class="ping-value" style="background:#261a1f; color:#f9acbc;">timeout</span></td>
                    <td><span class="status-badge unstable">⚠️ unstable</span></td>
                    <td class="uptime-row">status: partial</td>
                </tr>
                <!-- tele-yemen.com -->
                <tr>
                    <td class="service-name">
                        <span class="indicator yellow"></span>
                        tele-yemen.com
                    </td>
                    <td><span class="ping-value">67 ms</span></td>
                    <td><span class="status-badge moderate">◔ moderate</span></td>
                    <td class="uptime-row">uptime: 97.8%</td>
                </tr>
                <!-- local gateway -->
                <tr>
                    <td class="service-name">
                        <span class="indicator green"></span>
                        local gateway
                    </td>
                    <td><span class="ping-value" style="background:#0e2a24; color:#6ee7d0;">2 ms</span></td>
                    <td><span class="status-badge perfect">★ perfect</span></td>
                    <td class="uptime-row"><span class="latency-grade">latency: A+</span></td>
                </tr>
            </tbody>
        </table>
    </div>

    <div class="footer-note">
        <span>🔄 live simulation — based on Sana'a IXP probes</span>
        <span>📡 metrics: ping / icmp · route stability</span>
    </div>
</div>
</body>
</html>

<!-- القسم الفريد 2: عدادات تقدم اللغة بنمط Neumorphic -->
<div align="center">
  <h3>📖 Polyglot Progress (English · 汉语)</h3>
  <table style="background-color:#181828; border-radius:30px; padding:16px; box-shadow: 8px 8px 16px #0a0a0f, -8px -8px 16px #2c2c3a;">
    <tr>
      <td width="50%">
        🇬🇧 <b>English (C1 → C2)</b><br>
        <progress value="85" max="100" style="width:80%; height:14px; border-radius:10px;"></progress> 85%
        <br><sub>IELTS target: 8.0 · Technical writing advanced</sub>
      </td>
      <td width="50%">
        🇨🇳 <b>汉语 (HSK4 → HSK5)</b><br>
        <progress value="68" max="100" style="width:80%; height:14px; border-radius:10px;"></progress> 68%
        <br><sub>Reading tech docs · Next: HSK5 in 6 months</sub>
      </td>
    </tr>
  </table>
</div>
<br>

<!-- القسم الفريد 3: عد تنازلي لاختبارات القبول الجامعي (ديناميكي عبر API) -->
<div align="center">
  <h3>⏳ University Entrance Exam Countdown</h3>
  <img src="https://custom-countdown-api.vercel.app/api?target=2026-06-15T00:00:00&color=bb86fc&bg=1a1a2e&label=Days%20left&style=for-the-badge" alt="Countdown" />
  <br><sub>Target: June 15, 2026 · Computer Science faculty</sub>
</div>
<br>

<!-- القسم الفريد 4: إحصائيات متقدمة (مع بطاقات نادرة) -->
<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=moathkudosense-spec&show_icons=true&count_private=true&include_all_commits=true&theme=dark&bg_color=15152a&title_color=ffffff&icon_color=bb86fc&text_color=bbbbbb&border_color=2a2a3a&border_radius=20&ring_color=ff79c6" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=moathkudosense-spec&layout=compact&theme=dark&bg_color=15152a&title_color=ffffff&text_color=bbbbbb&border_color=2a2a3a&border_radius=20&hide=html,css,javascript&langs_count=6" width="41%" />
</div>
<br>
<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=moathkudosense-spec&theme=darkhub&no-frame=true&row=2&column=4&margin-w=8&margin-h=8" width="80%" />
</div>

<!-- القسم الفريد 5: Black Tools (الأدوات السوداء التي صنعها بنفسه) -->
<h2 align="center">🖤 Black Tools (Self-crafted)</h2>
<div align="center">
  <table style="background-color:#0b0b14; border-radius:30px; padding:12px; box-shadow: 8px 8px 18px #000, -6px -6px 12px #22223a;">
    <tr>
      <td align="center"><b>🎬 mpv-uosc-pro</b><br>Lua script · 847 lines<br><img src="https://img.shields.io/badge/UI-Touch_ready-9B59B6"/></td>
      <td align="center"><b>⚡ PS-Neumorphic</b><br>PowerShell profile · 320 aliases<br><img src="https://img.shields.io/badge/Terminal-Art-1e3a8a"/></td>
      <td align="center"><b>🔌 ESP-FlashTool</b><br>Python firmware flasher · 530 lines<br><img src="https://img.shields.io/badge/Error_Proof-FF6F00"/></td>
    </tr>
    <tr>
      <td align="center"><b>🌐 Y-Net Optimizer</b><br>OpenWRT QoS script · 290 lines<br><img src="https://img.shields.io/badge/Sana'a_Approved-00B5AD"/></td>
      <td align="center"><b>🎮 HoYo-API-Client</b><br>Python wrapper · 410 lines<br><img src="https://img.shields.io/badge/Async-3776AB"/></td>
      <td align="center"><b>📄 Neumorphic-Readme</b><br>This very template · reusable<br><img src="https://img.shields.io/badge/Open_Source-181717"/></td>
    </tr>
  </table>
</div>

<!-- القسم الفريد 6: خريطة المساهمات الحرارية (Neumorphic) -->
<h2 align="center">🔥 Contribution Heatmap (Last 30 days)</h2>
<div align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=moathkudosense-spec&theme=github-dark&bg_color=15152a&color=bb86fc&line=c792ea&point=ffffff&area=true&hide_border=true&radius=16" width="90%" />
</div>

<!-- القسم الفريد 7: آخر الإنجازات + مفتاح PGP -->
<div align="center">
  <table style="background-color:#15152a; border-radius:28px; padding:12px; width:90%;">
    <tr>
      <td width="50%">
        🏆 <b>Recent GitHub Achievements</b><br>
        <img src="https://github.githubassets.com/images/modules/profile/achievements/pull-shark-default.png" width="40" /> Pull Shark x2
        <img src="https://github.githubassets.com/images/modules/profile/achievements/quickdraw-default.png" width="40" /> Quickdraw
        <img src="https://github.githubassets.com/images/modules/profile/achievements/yolo-default.png" width="40" /> YOLO
      </td>
      <td width="50%">
        🔐 <b>PGP Public Key (Fingerprint)</b><br>
        <code>3E5F 8A9C 2B14 7F92  1A8E 5C4B 9D6F 8A21</code><br>
        <sub>Available on keyserver.ubuntu.com</sub>
      </td>
    </tr>
  </table>
</div>

<!-- القسم الفريد 8: أحدث 3 مشاريع مفتوحة المصدر تم زيارتها -->
<h2 align="center">📂 Recently active on</h2>
<div align="center">
  <img src="https://img.shields.io/badge/Lua-mpv--player--scripts-2C2D72?style=flat-square&logo=lua" />
  <img src="https://img.shields.io/badge/Python-HoYo--API-3776AB?style=flat-square&logo=python" />
  <img src="https://img.shields.io/badge/PowerShell-dotfiles-5391FE?style=flat-square&logo=powershell" />
  <br><br>
  <a href="#"><img src="https://img.shields.io/badge/📋_Copy_my_dotfiles-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="#"><img src="https://img.shields.io/badge/📡_Live_Network_Stats-00B5AD?style=for-the-badge&logo=grafana&logoColor=white" /></a>
</div>

<!-- تذييل مع عداد زوار فريد -->
<div align="center">
  <br>
  <img src="https://komarev.com/ghpvc/?username=moathkudosense-spec&label=👁️%20Neumorphic%20Visitors&color=bb86fc&style=flat-square" />
  <br><br>
  <svg width="400" height="30">
    <rect width="400" height="30" fill="none" rx="15" stroke="#bb86fc" stroke-width="1.5" stroke-dasharray="4 2" />
    <text x="200" y="20" font-family="monospace" font-size="12" fill="#bb86fc" text-anchor="middle">⚡ Last firmware tweak: 2026-04-21 21:01 UTC+3</text>
  </svg>
  <p><i>“Every line of code is a signature.” — Moath</i></p>
</div>
<!--
**moathkudosense-spec/moathkudosense-spec** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
