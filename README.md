<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Oscar's DIY Portfolio</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;700&family=Plus+Jakarta+Sans:wght@400;500;600&display=swap" rel="stylesheet">
    
    <style>
        /* 1. DESIGN SYSTEM VARIABLES */
        :root {
            --bg-color: #0f172a;       /* Dark slate background */
            --card-bg: #1e293b;        /* Lighter slate for cards */
            --text-main: #f8fafc;      /* Crisp white for headings */
            --text-muted: #94a3b8;     /* Muted grey for descriptions */
            --accent: #38bdf8;         /* Electric sky blue for highlights */
            --border-color: #334155;   /* Subtle card borders */
        }

        /* 2. BASE STYLES */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.6;
            padding: 3rem 1.5rem;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        /* Keeps your portfolio neatly centered on wide screens */
        .container {
            max-width: 800px;
            width: 100%;
        }

        /* 3. HERO / HEADER SECTION */
        header {
            margin-bottom: 3.5rem;
        }

        h1 {
            font-family: 'Space Grotesk', sans-serif;
            font-size: 2.8rem;
            font-weight: 700;
            margin-bottom: 0.5rem;
            /* Cool gradient text trick */
            background: linear-gradient(to right, #38bdf8, #818cf8);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .subtitle {
            font-size: 1rem;
            color: var(--text-muted);
            font-family: monospace;
            margin-bottom: 1.5rem;
        }

        .bio {
            font-size: 1.1rem;
            color: var(--text-main);
            border-left: 3px solid var(--accent);
            padding-left: 1.2rem;
            max-width: 600px;
        }

        /* 4. THE CARD GRID (The core layout) */
        .nav-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
        }

        /* 5. SLEEK CARD STYLING & ANIMATIONS */
        .card {
            background-color: var(--card-bg);
            border: 1px solid var(--border-color);
            border-radius: 12px;
            padding: 1.75rem;
            text-decoration: none;
            color: var(--text-main);
            /* Smooth transitions for hover effects */
            transition: transform 0.2s ease, border-color 0.2s ease, box-shadow 0.2s ease;
            display: flex;
            flex-direction: column;
        }

        /* Interactive Hover State */
        .card:hover {
            transform: translateY(-5px); /* Tiny lift effect */
            border-color: var(--accent);
            box-shadow: 0 10px 25px rgba(56, 189, 248, 0.15); /* Subtle glow */
        }

        .card h2 {
            font-family: 'Space Grotesk', sans-serif;
            font-size: 1.25rem;
            color: var(--accent);
            margin-bottom: 0.5rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        /* Adds a little arrow next to the card title */
        .card h2::after {
            content: '→';
            transition: transform 0.2s ease;
        }

        .card:hover h2::after {
            transform: translateX(4px); /* Pushes arrow right on hover */
        }

        .card p {
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        /* 6. FOOTER */
        footer {
            margin-top: 5rem;
            text-align: center;
            font-size: 0.85rem;
            color: var(--text-muted);
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>Oscar’s DIY Portfolio</h1>
            <p class="subtitle">portfolio-v1 // main_branch</p>
            <p class="bio">
                Hello, I’m Oscar 👋 I’m a first-year engineering student here at Monash.
                This repository features the projects, builds, and experiments I’m working on to develop my technical skills.
            </p>
        </header>

        <main class="nav-grid">
            <a href="/portfolio-v1/SKILLS.html" class="card">
                <h2>SKILLS</h2>
                <p>Technical competencies, software toolsets, and fabrication methods I use.</p>
            </a>

            <a href="/portfolio-v1/project.html" class="card">
                <h2>PROJECTS</h2>
                <p>A showcase of my engineering designs, calculations, and active physical builds.</p>
            </a>

            <a href="/portfolio-v1/CONTACTS.html" class="card">
                <h2>CONTACTS</h2>
                <p>Reach out for collaborations, technical discussion, or network connections.</p>
            </a>

            <a href="/portfolio-v1/backyardscience.html" class="card">
                <h2>BACKYARD SCIENCE</h2>
                <p>Just for fun. Unconventional experiments, quick prototypes, and informal side-quests.</p>
            </a>
        </main>

        <footer>
            <p>© 2026 Oscar. Built with HTML & CSS.</p>
        </footer>
    </div>

</body>
</html>
