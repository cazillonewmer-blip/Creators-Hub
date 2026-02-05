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
