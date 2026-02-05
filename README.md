<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Creative Community Hub</title>
    <style>
        /* --- CSS VARIABLES & RESET --- */
        :root {
            --bg-color: #1a1a1d; /* Dark Charcoal */
            --card-bg: #252529;
            --neon-purple: #b026ff;
            --electric-blue: #00ffff;
            --amethyst-text: #cbb4e6; /* Light Amethyst for readability */
            --heading-white: #ffffff;
            --glass-border: rgba(176, 38, 255, 0.3);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-color);
            color: var(--amethyst-text);
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* --- TYPOGRAPHY --- */
        h1, h2, h3 {
            color: var(--heading-white);
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        h2 {
            border-bottom: 2px solid var(--electric-blue);
            display: inline-block;
            margin-bottom: 20px;
            padding-bottom: 5px;
            text-shadow: 0 0 10px rgba(0, 255, 255, 0.5);
        }

        p {
            font-size: 0.95rem; /* Small text as requested */
            margin-bottom: 15px;
        }

        /* --- BUTTONS --- */
        .cta-btn {
            background: transparent;
            border: 2px solid var(--neon-purple);
            color: var(--electric-blue);
            padding: 12px 30px;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
            text-transform: uppercase;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
            box-shadow: 0 0 10px var(--neon-purple);
            border-radius: 5px;
            margin-top: 10px;
        }

        .cta-btn:hover {
            background: var(--neon-purple);
            color: #fff;
            box-shadow: 0 0 20px var(--neon-purple), 0 0 40px var(--electric-blue);
            transform: translateY(-2px);
        }

        /* --- LAYOUT SECTIONS --- */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* HERO SECTION */
        .hero {
            height: 90vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            background: radial-gradient(circle at center, #2a2a2e 0%, var(--bg-color) 70%);
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            background: -webkit-linear-gradient(left, var(--electric-blue), var(--neon-purple));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero-icons {
            font-size: 2rem;
            margin: 20px 0;
            letter-spacing: 15px;
        }

        .hero-desc {
            max-width: 600px;
            font-size: 1.1rem;
            color: var(--amethyst-text);
            margin-bottom: 30px;
        }

        .core-pillars {
            display: flex;
            gap: 20px;
            margin-top: 30px;
            flex-wrap: wrap;
            justify-content: center;
        }

        .pillar {
            background: rgba(255, 255, 255, 0.05);
            padding: 10px 20px;
            border-radius: 20px;
            border: 1px solid var(--glass-border);
        }

        /* SECTIONS GRID */
        .grid-section {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            padding: 50px 0;
        }

        .card {
            background: var(--card-bg);
            padding: 25px;
            border-radius: 10px;
            border-left: 4px solid var(--electric-blue);
            transition: transform 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
        }

        .card h3 {
            color: var(--electric-blue);
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .channel-list {
            list-style: none;
        }

        .channel-list li {
            margin-bottom: 8px;
            padding-left: 10px;
            border-left: 1px solid var(--neon-purple);
            font-size: 0.9rem;
        }

        /* TEAM SECTION */
        .team-section {
            text-align: center;
            padding: 60px 0;
            border-top: 1px solid #333;
        }

        .team-grid {
            display: flex;
            justify-content: center;
            gap: 40px;
            flex-wrap: wrap;
            margin-top: 30px;
        }

        .team-member {
            text-align: center;
        }

        .role {
            color: var(--electric-blue);
            font-size: 0.8rem;
            text-transform: uppercase;
            font-weight: bold;
        }

        .name {
            color: #fff;
            font-weight: bold;
            font-size: 1.2rem;
        }

        /* FOOTER */
        footer {
            text-align: center;
            padding: 40px;
            border-top: 1px solid var(--neon-purple);
            margin-top: 50px;
            font-size: 0.8rem;
        }

        /* RESPONSIVE */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2.5rem; }
            .grid-section { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

    <section class="hero">
        <div class="container">
            <h1>The Creative Cycle</h1>
            <div class="hero-icons">🛠️ 🎨 💻 ✍️ 🎬 🎵 🚀</div>
            <p class="hero-desc">
                Build things. Share work. Get feedback. Learn skills. Collaborate.<br>
                This isn't just a chatroom. It's a studio.
            </p>
            
            <div class="core-pillars">
                <div class="pillar">🛠️ A Workshop</div>
                <div class="pillar">🎓 A Learning Space</div>
                <div class="pillar">🤝 A Studio</div>
                <div class="pillar">🚀 A Launchpad</div>
            </div>

            <br><br>
            <a href="https://discord.gg/VKNYpkTt" class="cta-btn" target="_blank">Join The Community</a>
        </div>
    </section>

    <div class="container">
        
        <div class="grid-section">
            <div class="card">
                <h3>🌍 START HERE</h3>
                <ul class="channel-list">
                    <li>#welcome – What this server is about</li>
                    <li>#rules – Guidelines</li>
                    <li>#announcements – Updates</li>
                    <li>#introductions – "What do you create?"</li>
                </ul>
                <a href="https://discord.gg/VKNYpkTt" class="cta-btn" style="font-size:0.8rem; padding: 5px 15px;">Read Rules</a>
            </div>

            <div class="card">
                <h3>💬 COMMUNITY</h3>
                <ul class="channel-list">
                    <li>#general-chat – Hangout</li>
                    <li>#creative-talk – Ideas & Inspiration</li>
                </ul>
                <a href="https://discord.gg/VKNYpkTt" class="cta-btn" style="font-size:0.8rem; padding: 5px 15px;">Chat Now</a>
            </div>
        </div>

        <h2 style="margin-top: 20px;">🛠️ CREATE ZONES</h2>
        <div class="grid-section">
            <div class="card">
                <h3>Visual & Code</h3>
                <ul class="channel-list">
                    <li>🎨 #art-design</li>
                    <li>💻 #coding-tech</li>
                    <li>🎮 #game-dev</li>
                </ul>
                <a href="https://discord.gg/VKNYpkTt" class="cta-btn" style="font-size:0.8rem; padding: 5px 15px;">Share Art</a>
            </div>
            
            <div class="card">
                <h3>Audio & Story</h3>
                <ul class="channel-list">
                    <li>✍️ #writing-story</li>
                    <li>🎵 #music-audio</li>
                    <li>🎬 #video-editing</li>
                </ul>
                <a href="https://discord.gg/VKNYpkTt" class="cta-btn" style="font-size:0.8rem; padding: 5px 15px;">Share Story</a>
            </div>
        </div>

        <div class="grid-section">
            <div class="card" style="border-left-color: var(--neon-purple);">
                <h3>🧪 WORK MODE</h3>
                <p>Turn passive members into active creators.</p>
                <ul class="channel-list">
                    <li>#wip-projects – Unfinished work</li>
                    <li>#feedback-zone – Critique only</li>
                    <li>#idea-lab – Random project ideas</li>
                </ul>
                <a href="https://discord.gg/VKNYpkTt" class="cta-btn" style="font-size:0.8rem; padding: 5px 15px;">Get Feedback</a>
            </div>

            <div class="card" style="border-left-color: var(--neon-purple);">
                <h3>🤝 COLLABORATION</h3>
                <p>Where the magic happens.</p>
                <ul class="channel-list">
                    <li>#looking-for-team</li>
                    <li>#collab-projects</li>
                    <li>#project-updates</li>
                </ul>
                <a href="https://discord.gg/VKNYpkTt" class="cta-btn" style="font-size:0.8rem; padding: 5px 15px;">Find Team</a>
            </div>

            <div class="card" style="border-left-color: var(--neon-purple);">
                <h3>🧠 LEARN & GROW</h3>
                <ul class="channel-list">
                    <li>#resources</li>
                    <li>#tutorials</li>
                    <li>#tools-and-software</li>
                    <li>#creative-challenges ⭐</li>
                </ul>
                <a href="https://discord.gg/VKNYpkTt" class="cta-btn" style="font-size:0.8rem; padding: 5px 15px;">Start Learning</a>
            </div>
        </div>

    </div>

    <section class="team-section">
        <div class="container">
            <h2>Server Staff</h2>
            <div class="team-grid">
                <div class="team-member">
                    <div class="role">Owner</div>
                    <div class="name">Vixey leos</div>
                </div>
                <div class="team-member">
                    <div class="role">Co-Owner</div>
                    <div class="name">Mizvillian</div>
                </div>
                <div class="team-member">
                    <div class="role">Co-Owner</div>
                    <div class="name">2xTkazz</div>
                </div>
                <div class="team-member">
                    <div class="role">Co-Owner</div>
                    <div class="name">Lonewolf</div>
                </div>
                <div class="team-member">
                    <div class="role">Head Mod</div>
                    <div class="name">Diablo</div>
                </div>
            </div>
            <br><br>
            <div class="team-member">
                <div class="role">Web Developer</div>
                <div class="name">Zeyonahh</div>
            </div>
            
            <br><br>
            <a href="https://discord.gg/VKNYpkTt" class="cta-btn">Join The Server</a>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Creative Community. All Rights Reserved.</p>
        <p>Built for creators, by creators.</p>
    </footer>

</body>
</html>
        }

        * { box-sizing: border-box; }

        body {
            margin: 0;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            background-color: var(--bg-charcoal);
            color: var(--text-white);
            display: flex;
            height: 100vh;
            overflow: hidden;
        }

        /* SIDEBAR */
        .sidebar {
            width: 280px;
            background-color: var(--sidebar-dark);
            border-right: 1px solid var(--border);
            display: flex;
            flex-direction: column;
            overflow-y: auto;
        }

        .sidebar-brand {
            padding: 30px 20px;
            font-size: 1.4rem;
            font-weight: 800;
            color: var(--accent-blue);
            letter-spacing: -1px;
            border-bottom: 1px solid var(--border);
        }

        .category {
            padding: 20px 20px 5px;
            font-size: 0.7rem;
            text-transform: uppercase;
            color: var(--text-dim);
            letter-spacing: 1.5px;
            font-weight: bold;
        }

        .channel {
            padding: 10px 20px;
            display: flex;
            align-items: center;
            text-decoration: none;
            color: #ddd;
            font-size: 0.95rem;
            transition: 0.2s;
        }

        .channel:hover {
            background: var(--glass);
            color: var(--accent-blue);
        }

        .channel span { margin-right: 12px; font-size: 1.1rem; }

        /* MAIN AREA */
        .main {
            flex: 1;
            display: flex;
            flex-direction: column;
            background: radial-gradient(circle at top right, #1e2229, #121417);
        }

        /* STAFF BAR */
        .top-header {
            height: 70px;
            padding: 0 40px;
            display: flex;
            justify-content: flex-end;
            align-items: center;
            border-bottom: 1px solid var(--border);
        }

        .staff-chip {
            background: var(--glass);
            padding: 10px 20px;
            border-radius: 50px;
            border: 1px solid var(--border);
            font-size: 0.85rem;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
        }

        .staff-chip b { color: var(--accent-blue); margin-right: 5px; }
        .staff-chip span { color: var(--text-dim); margin: 0 10px; }

        /* HERO CONTENT */
        .content {
            padding: 40px;
            overflow-y: auto;
        }

        .hero-banner {
            background: linear-gradient(135deg, var(--accent-blue), var(--accent-purple));
            padding: 40px;
            border-radius: 20px;
            margin-bottom: 40px;
            color: #000;
        }

        .hero-banner h1 { margin: 0; font-size: 2.5rem; }
        .hero-banner p { font-size: 1.1rem; font-weight: 500; opacity: 0.9; }

        /* DASHBOARD GRID */
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        .card {
            background: var(--glass);
            border: 1px solid var(--border);
            padding: 30px;
            border-radius: 15px;
            transition: 0.3s;
            cursor: pointer;
            text-decoration: none;
            color: white;
        }

        .card:hover {
            background: rgba(255,255,255,0.06);
            border-color: var(--accent-blue);
            transform: translateY(-5px);
        }

        .card h3 { 
            margin-top: 0; 
            display: flex; 
            align-items: center; 
            color: var(--accent-blue);
        }

        .card p { color: var(--text-dim); line-height: 1.6; }

        .discord-btn {
            display: inline-block;
            background: var(--accent-blue);
            color: #000;
            padding: 12px 24px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: bold;
            margin-top: 15px;
            transition: 0.2s;
        }

        .discord-btn:hover { background: #fff; transform: scale(1.05); }

    </style>
</head>
<body>

    <aside class="sidebar">
        <div class="sidebar-brand">🛠️ THE WORKSHOP</div>
        
        <div class="category">🌍 START HERE</div>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>#</span> welcome</a>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>#</span> rules</a>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>#</span> introductions</a>

        <div class="category">🛠️ CREATE ZONES</div>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>🎨</span> art-design</a>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>💻</span> coding-tech</a>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>✍️</span> writing-story</a>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>🎵</span> music-audio</a>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>🎬</span> video-editing</a>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>🎮</span> game-dev</a>

        <div class="category">🧪 WORK MODE</div>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>#</span> wip-projects</a>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>#</span> feedback-zone</a>
        <a href="https://discord.gg/VKNYpkTt" class="channel"><span>#</span> idea-lab</a>
    </aside>

    <main class="main">
        <header class="top-header">
            <div class="staff-chip">
                <b>Owner:</b> Vixey leo <span>|</span>
                <b>Co-Owner:</b> Mizvillan, 2xTKazzz <span>|</span>
                <b>Mod:</b> Zeyonahh
            </div>
        </header>

        <div class="content">
            <section class="hero-banner">
                <h1>Build. Share. Grow.</h1>
                <p>A studio for collaborators and a launchpad for your next big project.</p>
                <a href="https://discord.gg/VKNYpkTt" class="discord-btn">JOIN COMMUNITY</a>
            </section>

            <div class="grid">
                <a href="https://discord.gg/VKNYpkTt" class="card">
                    <h3>🤝 Collaboration Studio</h3>
                    <p>Stop chatting, start building. Find team members for game-dev, coding, or art projects here.</p>
                </a>

                <a href="https://discord.gg/VKNYpkTt" class="card">
                    <h3>🎓 Learning Space</h3>
                    <p>Access curated resources, tutorials, and community-led software challenges.</p>
                </a>

                <a href="https://discord.gg/VKNYpkTt" class="card">
                    <h3>🧪 The Feedback Zone</h3>
                    <p>Drop your WIPs (Work in Progress) and get honest, high-quality critique from fellow creators.</p>
                </a>

                <a href="https://discord.gg/VKNYpkTt" class="card">
                    <h3>🚀 Launchpad</h3>
                    <p>Ready to release? Showcase your finished projects to the entire community.</p>
                </a>
            </div>
        </div>
    </main>

</body>
</html>
