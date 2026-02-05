<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Workshop | Creative Community</title>
    <style>
        :root {
            --bg-charcoal: #121417;
            --sidebar-dark: #1a1d21;
            --accent-blue: #00e5ff; /* Electric Blue */
            --accent-purple: #9d50bb; /* Neon Purple */
            --text-white: #ffffff;
            --text-dim: #a0a0a0;
            --glass: rgba(255, 255, 255, 0.03);
            --border: rgba(255, 255, 255, 0.1);
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
