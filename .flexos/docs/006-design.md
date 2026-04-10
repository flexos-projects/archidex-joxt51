---
id: doc-design
title: Archidex — Design
type: doc
subtype: design
status: published
sequence: 6
createdAt: "2026-04-10T21:02:21.436Z"
updatedAt: "2026-04-10T21:02:21.436Z"
---

# Design

Archidex is a digital field guide. The design language must bridge two worlds: the historic, physical reality of architecture, and the precise, gamified nature of a collection app. 

The visual identity is rooted in the aesthetics of architectural drafting and blueprints. The interface feels highly structured, governed by clear grids, visible hairlines, and precise spacing. It avoids the soft, bubbly, heavily shadowed look of typical consumer apps. Instead, corners have tighter radii (`--radius-sm` or `--radius-md`), mimicking the sharp intersections of buildings.

In Dark Mode (the default "Blueprint" theme), backgrounds are a deep, inky navy blue, not standard black. Accents are electric cyan and drafting-pencil yellow, making annotations and UI elements pop like chalk on a blueprint. In Light Mode (the "Drafting Paper" theme), the background is a warm, textured cream, with deep charcoal text and terracotta accents, evoking classic reference books and masonry.

Typography is critical. The display font is a structured, geometric sans-serif (Space Grotesk or Archivo) that looks like it could be on an engineering diagram. The body font is highly legible (Inter), while data points (GPS coordinates, eras, confidence scores) use a monospace font to emphasize precision.

Photography is treated as the hero. UI elements overlaying photos (like the scanner reticle or annotations) are crisp, thin, and utilitarian. The app should feel like a piece of high-end specialized equipment—a tricorder for design nerds.

<flex_block type="tokens">
{
  "category": "colors",
  "mode": "dark",
  "tokens": {
    "--color-primary": "oklch(75% 0.15 230)",
    "--color-primary-hover": "oklch(80% 0.15 230)",
    "--color-primary-active": "oklch(70% 0.15 230)",
    "--color-primary-muted": "oklch(75% 0.15 230 / 0.15)",
    "--color-accent": "oklch(85% 0.18 90)",
    "--color-bg": "oklch(18% 0.04 250)",
    "--color-surface": "oklch(23% 0.04 250)",
    "--color-surface-raised": "oklch(28% 0.03 250)",
    "--color-surface-overlay": "oklch(15% 0.04 250 / 0.8)",
    "--color-border": "oklch(35% 0.03 250)",
    "--color-border-subtle": "oklch(28% 0.03 250)",
    "--color-text": "oklch(95% 0.01 250)",
    "--color-text-secondary": "oklch(75% 0.02 250)",
    "--color-text-muted": "oklch(60% 0.02 250)",
    "--color-text-on-primary": "oklch(15% 0.04 250)",
    "--color-success": "oklch(75% 0.12 160)",
    "--color-warning": "oklch(85% 0.18 90)",
    "--color-error": "oklch(65% 0.15 25)"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "colors",
  "mode": "light",
  "tokens": {
    "--color-primary": "oklch(45% 0.12 250)",
    "--color-primary-hover": "oklch(40% 0.12 250)",
    "--color-primary-active": "oklch(35% 0.12 250)",
    "--color-primary-muted": "oklch(45% 0.12 250 / 0.12)",
    "--color-accent": "oklch(55% 0.15 45)",
    "--color-bg": "oklch(97% 0.01 85)",
    "--color-surface": "oklch(99% 0.005 85)",
    "--color-surface-raised": "oklch(100% 0 0)",
    "--color-surface-overlay": "oklch(95% 0.01 85 / 0.8)",
    "--color-border": "oklch(85% 0.01 85)",
    "--color-border-subtle": "oklch(90% 0.01 85)",
    "--color-text": "oklch(25% 0.02 250)",
    "--color-text-secondary": "oklch(45% 0.02 250)",
    "--color-text-muted": "oklch(60% 0.02 250)",
    "--color-text-on-primary": "oklch(98% 0 0)",
    "--color-success": "oklch(50% 0.12 160)",
    "--color-warning": "oklch(60% 0.15 45)",
    "--color-error": "oklch(55% 0.15 25)"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "typography",
  "tokens": {
    "--font-display": "'Space Grotesk', system-ui, sans-serif",
    "--font-body": "'Inter', system-ui, sans-serif",
    "--font-mono": "'JetBrains Mono', monospace",
    "--font-size-xs": "0.75rem",
    "--font-size-sm": "0.875rem",
    "--font-size-base": "1rem",
    "--font-size-lg": "1.125rem",
    "--font-size-xl": "1.25rem",
    "--font-size-2xl": "1.5rem",
    "--font-size-3xl": "2rem",
    "--font-size-4xl": "2.5rem",
    "--font-size-5xl": "3.5rem",
    "--font-weight-normal": "400",
    "--font-weight-medium": "500",
    "--font-weight-bold": "700",
    "--line-height-tight": "1.1",
    "--line-height-normal": "1.5",
    "--line-height-relaxed": "1.7"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "spacing",
  "tokens": {
    "--space-1": "0.25rem",
    "--space-2": "0.5rem",
    "--space-3": "0.75rem",
    "--space-4": "1rem",
    "--space-6": "1.5rem",
    "--space-8": "2rem",
    "--space-12": "3rem",
    "--space-16": "4rem",
    "--space-24": "6rem"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "radii",
  "tokens": {
    "--radius-sm": "0.25rem",
    "--radius-md": "0.5rem",
    "--radius-lg": "0.75rem",
    "--radius-xl": "1rem",
    "--radius-full": "9999px"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "shadows",
  "tokens": {
    "--shadow-sm": "0 2px 4px oklch(0% 0 0 / 0.1)",
    "--shadow-md": "0 4px 12px oklch(0% 0 0 / 0.15), 0 1px 3px oklch(0% 0 0 / 0.08)",
    "--shadow-lg": "0 12px 32px oklch(0% 0 0 / 0.2), 0 4px 8px oklch(0% 0 0 / 0.1)"
  }
}
</flex_block>

<flex_block type="tokens">
{
  "category": "transitions",
  "tokens": {
    "--transition-fast": "150ms ease-out",
    "--transition-base": "250ms ease-out",
    "--transition-slow": "400ms cubic-bezier(0.2, 0.8, 0.2, 1)",
    "--ease-spring": "cubic-bezier(0.34, 1.56, 0.64, 1)"
  }
}
</flex_block>

<flex_block type="mockup-html" id="landing-preview">
<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Archidex | The Field Guide to the Built World</title>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&family=JetBrains+Mono:wght@400;700&family=Space+Grotesk:wght@500;700&display=swap" rel="stylesheet">
<script src="https://unpkg.com/lucide@latest"></script>
<style>
  :root[data-theme="dark"] {
    --color-primary: oklch(75% 0.15 230);
    --color-primary-hover: oklch(80% 0.15 230);
    --color-primary-muted: oklch(75% 0.15 230 / 0.15);
    --color-accent: oklch(85% 0.18 90);
    --color-bg: oklch(18% 0.04 250);
    --color-surface: oklch(23% 0.04 250);
    --color-surface-raised: oklch(28% 0.03 250);
    --color-border: oklch(35% 0.03 250);
    --color-text: oklch(95% 0.01 250);
    --color-text-secondary: oklch(75% 0.02 250);
    --color-text-muted: oklch(60% 0.02 250);
    --color-text-on-primary: oklch(15% 0.04 250);
  }
  
  :root[data-theme="light"] {
    --color-primary: oklch(45% 0.12 250);
    --color-primary-hover: oklch(40% 0.12 250);
    --color-primary-muted: oklch(45% 0.12 250 / 0.12);
    --color-accent: oklch(55% 0.15 45);
    --color-bg: oklch(97% 0.01 85);
    --color-surface: oklch(99% 0.005 85);
    --color-surface-raised: oklch(100% 0 0);
    --color-border: oklch(85% 0.01 85);
    --color-text: oklch(25% 0.02 250);
    --color-text-secondary: oklch(45% 0.02 250);
    --color-text-muted: oklch(60% 0.02 250);
    --color-text-on-primary: oklch(98% 0 0);
  }

  :root {
    --font-display: 'Space Grotesk', system-ui, sans-serif;
    --font-body: 'Inter', system-ui, sans-serif;
    --font-mono: 'JetBrains Mono', monospace;
    --radius-sm: 0.25rem;
    --radius-md: 0.5rem;
    --radius-lg: 0.75rem;
    --radius-xl: 1rem;
    --transition-fast: 150ms ease-out;
    --transition-base: 250ms ease-out;
    --transition-slow: 400ms cubic-bezier(0.2, 0.8, 0.2, 1);
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }
  
  body {
    font-family: var(--font-body);
    background-color: var(--color-bg);
    color: var(--color-text);
    line-height: 1.5;
    transition: background-color var(--transition-base), color var(--transition-base);
    overflow-x: hidden;
    background-image: 
      linear-gradient(var(--color-border) 1px, transparent 1px),
      linear-gradient(90deg, var(--color-border) 1px, transparent 1px);
    background-size: 40px 40px;
    background-position: center top;
  }

  /* Typography */
  h1, h2, h3, .font-display { font-family: var(--font-display); font-weight: 700; line-height: 1.1; }
  .font-mono { font-family: var(--font-mono); }
  
  /* Layout */
  .container { max-width: 1200px; margin: 0 auto; padding: 0 2rem; }
  
  /* Navbar */
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.5rem 0;
    border-bottom: 1px solid var(--color-border);
    backdrop-filter: blur(10px);
    position: sticky;
    top: 0;
    z-index: 100;
  }
  .logo { font-family: var(--font-display); font-size: 1.5rem; font-weight: 700; display: flex; align-items: center; gap: 0.5rem; }
  .logo i { color: var(--color-primary); }
  
  .nav-actions { display: flex; gap: 1rem; align-items: center; }
  button {
    background: none; border: none; cursor: pointer;
    font-family: var(--font-body); font-weight: 500; font-size: 0.875rem;
    transition: all var(--transition-fast);
  }
  .btn-primary {
    background-color: var(--color-primary);
    color: var(--color-text-on-primary);
    padding: 0.75rem 1.5rem;
    border-radius: var(--radius-md);
  }
  .btn-primary:hover { background-color: var(--color-primary-hover); transform: translateY(-1px); }
  .btn-icon {
    width: 40px; height: 40px;
    border-radius: var(--radius-md);
    background-color: var(--color-surface);
    color: var(--color-text);
    display: flex; align-items: center; justify-content: center;
    border: 1px solid var(--color-border);
  }
  .btn-icon:hover { background-color: var(--color-surface-raised); }

  /* Hero Section */
  .hero {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 4rem;
    padding: 6rem 0;
    align-items: center;
    min-height: calc(100vh - 80px);
  }
  
  .hero-content h1 {
    font-size: clamp(3rem, 5vw, 4.5rem);
    margin-bottom: 1.5rem;
    letter-spacing: -0.02em;
  }
  .hero-content p {
    font-size: 1.25rem;
    color: var(--color-text-secondary);
    margin-bottom: 2.5rem;
    max-width: 480px;
  }
  
  .hero-badges {
    display: flex; gap: 1rem; margin-top: 3rem;
  }
  .badge {
    display: flex; align-items: center; gap: 0.5rem;
    padding: 0.5rem 1rem;
    background-color: var(--color-surface);
    border: 1px solid var(--color-border);
    border-radius: var(--radius-full);
    font-family: var(--font-mono); font-size: 0.75rem;
    color: var(--color-text-secondary);
  }

  /* Phone Mockup & Scanner Interactive */
  .phone-mockup {
    position: relative;
    width: 320px;
    height: 650px;
    background-color: #000;
    border-radius: 40px;
    border: 12px solid var(--color-surface-raised);
    box-shadow: 0 24px 48px rgba(0,0,0,0.4);
    margin: 0 auto;
    overflow: hidden;
    display: flex;
    flex-direction: column;
  }
  
  .phone-screen {
    position: relative;
    flex: 1;
    background-image: url('https://images.unsplash.com/photo-1552596954-c9233f2afbe8?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80');
    background-size: cover;
    background-position: center;
  }
  
  .camera-ui {
    position: absolute;
    inset: 0;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 2rem 1.5rem;
    z-index: 10;
  }
  
  .crosshairs {
    position: absolute;
    top: 50%; left: 50%;
    transform: translate(-50%, -50%);
    width: 200px; height: 200px;
    border: 1px solid rgba(255,255,255,0.3);
  }
  .crosshairs::before, .crosshairs::after {
    content: ''; position: absolute; background: white;
  }
  .crosshairs::before { top: 50%; left: -10px; right: -10px; height: 1px; }
  .crosshairs::after { left: 50%; top: -10px; bottom: -10px; width: 1px; }
  
  .scan-line {
    position: absolute;
    top: 0; left: 0; right: 0; height: 2px;
    background-color: var(--color-primary);
    box-shadow: 0 0 12px var(--color-primary);
    opacity: 0;
    transform: translateY(0);
  }
  
  .capture-btn-wrapper {
    display: flex; justify-content: center; margin-top: auto;
  }
  .capture-btn {
    width: 64px; height: 64px;
    border-radius: 50%;
    background-color: transparent;
    border: 4px solid white;
    position: relative;
  }
  .capture-btn::after {
    content: ''; position: absolute; inset: 4px;
    background-color: white; border-radius: 50%;
    transition: transform var(--transition-fast);
  }
  .capture-btn:hover::after { transform: scale(0.9); }
  .capture-btn:active::after { transform: scale(0.8); }

  /* Analysis Result Card */
  .result-card {
    position: absolute;
    bottom: 0; left: 0; right: 0;
    background-color: var(--color-surface);
    padding: 1.5rem;
    border-top-left-radius: var(--radius-xl);
    border-top-right-radius: var(--radius-xl);
    transform: translateY(100%);
    transition: transform var(--transition-slow);
    z-index: 20;
    border-top: 1px solid var(--color-border);
  }
  .result-card.active { transform: translateY(0); }
  
  .result-header { display: flex; justify-content: space-between; align-items: flex-start; margin-bottom: 1rem; }
  .result-style { font-family: var(--font-display); font-size: 1.5rem; font-weight: 700; color: var(--color-text); }
  .result-confidence { font-family: var(--font-mono); font-size: 0.75rem; color: var(--color-primary); background: var(--color-primary-muted); padding: 0.25rem 0.5rem; border-radius: var(--radius-sm); }
  .result-desc { font-size: 0.875rem; color: var(--color-text-secondary); margin-bottom: 1.5rem; }
  .result-cta { width: 100%; background: var(--color-text); color: var(--color-bg); padding: 0.75rem; border-radius: var(--radius-md); font-weight: 700; }

  /* Bounding Boxes */
  .bounding-box {
    position: absolute;
    border: 2px solid var(--color-primary);
    background: var(--color-primary-muted);
    opacity: 0;
    transition: opacity var(--transition-base);
    z-index: 15;
  }
  .box-1 { top: 20%; left: 30%; width: 40%; height: 25%; }
  .box-2 { top: 55%; left: 40%; width: 20%; height: 30%; }
  .bounding-box.active { opacity: 1; }
  .bounding-label {
    position: absolute; bottom: 100%; left: 0;
    background: var(--color-primary); color: var(--color-text-on-primary);
    font-family: var(--font-mono); font-size: 0.6rem;
    padding: 2px 6px; white-space: nowrap;
  }

  /* Animations */
  @keyframes scan {
    0% { transform: translateY(0); opacity: 1; }
    50% { transform: translateY(500px); opacity: 1; }
    100% { transform: translateY(0); opacity: 1; }
  }

  /* Field Guide Section */
  .field-guide { padding: 6rem 0; border-top: 1px solid var(--color-border); background: var(--color-surface); }
  .section-header { text-align: center; margin-bottom: 4rem; }
  .section-header h2 { font-size: 2.5rem; margin-bottom: 1rem; }
  .section-header p { color: var(--color-text-secondary); max-width: 600px; margin: 0 auto; }
  
  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
  }
  
  .style-card {
    background: var(--color-bg);
    border: 1px solid var(--color-border);
    border-radius: var(--radius-lg);
    overflow: hidden;
    transition: transform var(--transition-fast), border-color var(--transition-fast);
  }
  .style-card:hover { transform: translateY(-4px); border-color: var(--color-primary); }
  
  .style-img { height: 200px; background: var(--color-surface-raised); position: relative; }
  .style-img img { width: 100%; height: 100%; object-fit: cover; opacity: 0.8; mix-blend-mode: luminosity; }
  .style-card.locked .style-img img { opacity: 0.1; filter: blur(4px); }
  .style-card.locked .style-img::after {
    content: '?'; position: absolute; inset: 0; display: flex; align-items: center; justify-content: center;
    font-family: var(--font-display); font-size: 3rem; color: var(--color-text-muted);
  }
  
  .style-content { padding: 1.5rem; }
  .style-content h3 { font-size: 1.25rem; margin-bottom: 0.5rem; }
  .style-meta { display: flex; justify-content: space-between; font-family: var(--font-mono); font-size: 0.75rem; color: var(--color-text-muted); }

  @media (max-width: 768px) {
    .hero { grid-template-columns: 1fr; text-align: center; gap: 3rem; padding: 3rem 0; }
    .hero-content p { margin: 0 auto 2rem; }
    .hero-badges { justify-content: center; }
  }
</style>
</head>
<body>

  <div class="container">
    <nav>
      <div class="logo"><i data-lucide="scan-line"></i> Archidex</div>
      <div class="nav-actions">
        <button id="theme-toggle" class="btn-icon" aria-label="Toggle theme">
          <i data-lucide="sun"></i>
        </button>
        <button class="btn-primary">Get the App</button>
      </div>
    </nav>
  </div>

  <section class="hero container">
    <div class="hero-content">
      <h1>Read the streets.</h1>
      <p>Point your camera at any building to instantly identify its architectural style. Collect cities, learn the language of design, and see the world with new eyes.</p>
      
      <button class="btn-primary" style="font-size: 1.125rem; padding: 1rem 2rem;">Start Exploring</button>
      
      <div class="hero-badges">
        <div class="badge"><i data-lucide="camera" style="width:14px;height:14px;"></i> AI Scanner</div>
        <div class="badge"><i data-lucide="book" style="width:14px;height:14px;"></i> 80+ Styles</div>
        <div class="badge"><i data-lucide="map-pin" style="width:14px;height:14px;"></i> Global Map</div>
      </div>
    </div>
    
    <div class="phone-mockup">
      <div class="phone-screen">
        <div class="scan-line" id="scanLine"></div>
        
        <div class="bounding-box box-1" id="box1">
          <div class="bounding-label">Cresting</div>
        </div>
        <div class="bounding-box box-2" id="box2">
          <div class="bounding-label">Oriel Window</div>
        </div>

        <div class="camera-ui">
          <div style="display:flex; justify-content:space-between; color:white;">
            <i data-lucide="x"></i>
            <i data-lucide="zap"></i>
          </div>
          
          <div class="crosshairs" id="crosshairs"></div>
          
          <div class="capture-btn-wrapper">
            <button class="capture-btn" id="captureBtn" aria-label="Scan Building"></button>
          </div>
        </div>
        
        <div class="result-card" id="resultCard">
          <div class="result-header">
            <div class="result-style">Châteauesque</div>
            <div class="result-confidence">98% Match</div>
          </div>
          <p class="result-desc">Characterized by massive masonry, steep roofs with cresting, and elaborate dormers. Popularized in the late 19th century by Richard Morris Hunt.</p>
          <button class="result-cta" id="resetBtn">Add to Passport</button>
        </div>
      </div>
    </div>
  </section>

  <section class="field-guide">
    <div class="container">
      <div class="section-header">
        <h2>The Field Guide</h2>
        <p>Your personal collector's album. Discover the stories behind the facades and complete your architectural catalog.</p>
      </div>
      
      <div class="grid">
        <div class="style-card">
          <div class="style-img">
            <img src="https://images.unsplash.com/photo-1513694203232-719a280e022f?w=600&q=80" alt="Brutalist">
          </div>
          <div class="style-content">
            <h3>Brutalism</h3>
            <div class="style-meta"><span>1950s - 1970s</span><span>Collected</span></div>
          </div>
        </div>
        
        <div class="style-card">
          <div class="style-img">
            <img src="https://images.unsplash.com/photo-1541857754-557a24ed9217?w=600&q=80" alt="Art Deco">
          </div>
          <div class="style-content">
            <h3>Art Deco</h3>
            <div class="style-meta"><span>1920s - 1930s</span><span>Collected</span></div>
          </div>
        </div>
        
        <div class="style-card locked">
          <div class="style-img">
            <img src="https://images.unsplash.com/photo-1582582494705-f8ce0b0c24f0?w=600&q=80" alt="Gothic Revival">
          </div>
          <div class="style-content">
            <h3 style="color:var(--color-text-muted);">Gothic Revival</h3>
            <div class="style-meta"><span>1740s - 1800s</span><span>Undiscovered</span></div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <script>
    // Initialize Lucide icons
    lucide.createIcons();

    // Theme Toggle
    const themeToggle = document.getElementById('theme-toggle');
    const html = document.documentElement;
    
    themeToggle.addEventListener('click', () => {
      const currentTheme = html.getAttribute('data-theme');
      const newTheme = currentTheme === 'dark' ? 'light' : 'dark';
      html.setAttribute('data-theme', newTheme);
      
      // Update icon
      themeToggle.innerHTML = newTheme === 'dark' 
        ? '<i data-lucide="sun"></i>' 
        : '<i data-lucide="moon"></i>';
      lucide.createIcons();
    });

    // Scanner Interaction
    const captureBtn = document.getElementById('captureBtn');
    const scanLine = document.getElementById('scanLine');
    const crosshairs = document.getElementById('crosshairs');
    const resultCard = document.getElementById('resultCard');
    const resetBtn = document.getElementById('resetBtn');
    const boxes = document.querySelectorAll('.bounding-box');

    captureBtn.addEventListener('click', () => {
      // Hide crosshairs and button
      crosshairs.style.opacity = '0';
      captureBtn.style.opacity = '0';
      
      // Start scan
      scanLine.style.animation = 'scan 1.5s ease-in-out';
      
      // Show boxes during scan
      setTimeout(() => {
        boxes.forEach(box => box.classList.add('active'));
      }, 500);

      // Show result
      setTimeout(() => {
        scanLine.style.animation = 'none';
        scanLine.style.opacity = '0';
        resultCard.classList.add('active');
      }, 1500);
    });

    resetBtn.addEventListener('click', () => {
      resultCard.classList.remove('active');
      boxes.forEach(box => box.classList.remove('active'));
      setTimeout(() => {
        crosshairs.style.opacity = '1';
        captureBtn.style.opacity = '1';
      }, 300);
    });
  </script>
</body>
</html>
</flex_block>

---

<flex_block type="tokens" id="blk-001" name="colors">
{
  "category": "colors",
  "mode": "dark",
  "tokens": {
    "--color-primary": "oklch(75% 0.15 230)",
    "--color-primary-hover": "oklch(80% 0.15 230)",
    "--color-primary-active": "oklch(70% 0.15 230)",
    "--color-primary-muted": "oklch(75% 0.15 230 / 0.15)",
    "--color-accent": "oklch(85% 0.18 90)",
    "--color-bg": "oklch(18% 0.04 250)",
    "--color-surface": "oklch(23% 0.04 250)",
    "--color-surface-raised": "oklch(28% 0.03 250)",
    "--color-surface-overlay": "oklch(15% 0.04 250 / 0.8)",
    "--color-border": "oklch(35% 0.03 250)",
    "--color-border-subtle": "oklch(28% 0.03 250)",
    "--color-text": "oklch(95% 0.01 250)",
    "--color-text-secondary": "oklch(75% 0.02 250)",
    "--color-text-muted": "oklch(60% 0.02 250)",
    "--color-text-on-primary": "oklch(15% 0.04 250)",
    "--color-success": "oklch(75% 0.12 160)",
    "--color-warning": "oklch(85% 0.18 90)",
    "--color-error": "oklch(65% 0.15 25)"
  }
}
</flex_block>

<flex_block type="tokens" id="blk-002" name="colors">
{
  "category": "colors",
  "mode": "light",
  "tokens": {
    "--color-primary": "oklch(45% 0.12 250)",
    "--color-primary-hover": "oklch(40% 0.12 250)",
    "--color-primary-active": "oklch(35% 0.12 250)",
    "--color-primary-muted": "oklch(45% 0.12 250 / 0.12)",
    "--color-accent": "oklch(55% 0.15 45)",
    "--color-bg": "oklch(97% 0.01 85)",
    "--color-surface": "oklch(99% 0.005 85)",
    "--color-surface-raised": "oklch(100% 0 0)",
    "--color-surface-overlay": "oklch(95% 0.01 85 / 0.8)",
    "--color-border": "oklch(85% 0.01 85)",
    "--color-border-subtle": "oklch(90% 0.01 85)",
    "--color-text": "oklch(25% 0.02 250)",
    "--color-text-secondary": "oklch(45% 0.02 250)",
    "--color-text-muted": "oklch(60% 0.02 250)",
    "--color-text-on-primary": "oklch(98% 0 0)",
    "--color-success": "oklch(50% 0.12 160)",
    "--color-warning": "oklch(60% 0.15 45)",
    "--color-error": "oklch(55% 0.15 25)"
  }
}
</flex_block>

<flex_block type="tokens" id="blk-003" name="typography">
{
  "category": "typography",
  "tokens": {
    "--font-display": "'Space Grotesk', system-ui, sans-serif",
    "--font-body": "'Inter', system-ui, sans-serif",
    "--font-mono": "'JetBrains Mono', monospace",
    "--font-size-xs": "0.75rem",
    "--font-size-sm": "0.875rem",
    "--font-size-base": "1rem",
    "--font-size-lg": "1.125rem",
    "--font-size-xl": "1.25rem",
    "--font-size-2xl": "1.5rem",
    "--font-size-3xl": "2rem",
    "--font-size-4xl": "2.5rem",
    "--font-size-5xl": "3.5rem",
    "--font-weight-normal": "400",
    "--font-weight-medium": "500",
    "--font-weight-bold": "700",
    "--line-height-tight": "1.1",
    "--line-height-normal": "1.5",
    "--line-height-relaxed": "1.7"
  }
}
</flex_block>

<flex_block type="tokens" id="blk-004" name="spacing">
{
  "category": "spacing",
  "tokens": {
    "--space-1": "0.25rem",
    "--space-2": "0.5rem",
    "--space-3": "0.75rem",
    "--space-4": "1rem",
    "--space-6": "1.5rem",
    "--space-8": "2rem",
    "--space-12": "3rem",
    "--space-16": "4rem",
    "--space-24": "6rem"
  }
}
</flex_block>

<flex_block type="tokens" id="blk-005" name="radii">
{
  "category": "radii",
  "tokens": {
    "--radius-sm": "0.25rem",
    "--radius-md": "0.5rem",
    "--radius-lg": "0.75rem",
    "--radius-xl": "1rem",
    "--radius-full": "9999px"
  }
}
</flex_block>

<flex_block type="tokens" id="blk-006" name="shadows">
{
  "category": "shadows",
  "tokens": {
    "--shadow-sm": "0 2px 4px oklch(0% 0 0 / 0.1)",
    "--shadow-md": "0 4px 12px oklch(0% 0 0 / 0.15), 0 1px 3px oklch(0% 0 0 / 0.08)",
    "--shadow-lg": "0 12px 32px oklch(0% 0 0 / 0.2), 0 4px 8px oklch(0% 0 0 / 0.1)"
  }
}
</flex_block>

<flex_block type="tokens" id="blk-007" name="transitions">
{
  "category": "transitions",
  "tokens": {
    "--transition-fast": "150ms ease-out",
    "--transition-base": "250ms ease-out",
    "--transition-slow": "400ms cubic-bezier(0.2, 0.8, 0.2, 1)",
    "--ease-spring": "cubic-bezier(0.34, 1.56, 0.64, 1)"
  }
}
</flex_block>
