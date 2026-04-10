---
id: doc-design
title: "Design System & Visual Language"
type: doc
status: active
createdAt: "2026-04-10"
relatesTo: ["docs/001-vision.md", "docs/005-flows.md"]
---

# 6. Design System & Visual Language

The design language of Archidex bridges two worlds: the historic, physical reality of architecture and the precise, gamified nature of a digital collection app. The aesthetic is that of a modern field guide or a set of architectural blueprints.

## Core Principles

- **Structured & Geometric:** The interface is governed by clear grids, visible hairlines, and precise spacing. It avoids the soft, bubbly look of typical consumer apps. Corners are sharp, mimicking the intersections of buildings.
- **Typographically Driven:** Typography is critical for conveying the app's academic-but-accessible personality. A structured display font for headlines is paired with a highly legible body font and a monospace font for data points to emphasize precision.
- **Content as Hero:** Photography and illustrations are the stars. UI elements that overlay them are crisp, thin, and utilitarian, feeling like a high-end piece of specialized equipment—a tricorder for design nerds.

## Color System

The color system is designed around two themes that evoke architectural drafting materials.

### "Blueprint" Theme (Dark Mode - Default)
- **Background:** A deep, inky navy blue (`--color-bg`), not pure black.
- **Text:** Crisp, high-contrast off-white (`--color-text`).
- **Accents:** Electric cyan (`--color-primary`) and drafting-pencil yellow (`--color-accent`) make annotations and UI elements pop.

### "Drafting Paper" Theme (Light Mode)
- **Background:** A warm, textured cream (`--color-bg`).
- **Text:** Deep charcoal (`--color-text`).
- **Accents:** Terracotta (`--color-accent`) and a deep blue (`--color-primary`), evoking classic reference books and masonry.

<flex_block type="tokens" id="colors-dark">
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

<flex_block type="tokens" id="colors-light">
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

## Typography

<flex_block type="tokens" id="typography">
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

## Spacing & Sizing

<flex_block type="tokens" id="spacing">
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

<flex_block type="tokens" id="radii">
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

## Landing Page Mockup

This interactive mockup demonstrates the design system applied to the marketing landing page, including the core "scanner" interaction.

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
</style>
</head>
<body>
  <div class="container" style="padding: 4rem 2rem; text-align: center;">
    <h1 style="font-family: var(--font-display); font-size: 2.5rem; margin-bottom: 1rem;">Full Mockup Available</h1>
    <p style="color: var(--color-text-secondary); max-width: 600px; margin: 0 auto;">The complete, interactive HTML mockup has been included in the project seed and can be viewed there. This block is a placeholder to keep this document concise.</p>
  </div>
</body>
</html>
</flex_block>
