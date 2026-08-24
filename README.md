# Portfolio Site — Rohan

A static single-page portfolio website for a filmmaker/cinematographer. Hand-crafted with vanilla HTML, CSS, and JavaScript — no build tools, no frameworks.

## Tech Stack

- **HTML5 / CSS3 / Vanilla JS** — single `index.html` file
- **GSAP 3.12.5** — scroll-triggered animations and text reveals
- **Lenis 1.1.3** — smooth scrolling
- **Supabase JS SDK** — contact form backend (message submissions)

## Features

- **Hero Banner** — full-viewport video background with layered scrolling video strip
- **Featured Projects** — bento-grid layout with native video and YouTube embeds
- **About** — two-page bio section with stats and process
- **Photography Gallery** — horizontal drag-to-scroll marquee with hover-to-pause
- **Skills Marquee** — infinite scrolling skill strip
- **Contact Form** — submits to Supabase `messages` table
- **Viewfinder HUD** — decorative overlay with live timecode counter
- **Custom Cursor** — rotating reticle with contextual labels
- **Scroll-spy Navigation** — fixed bottom nav with active section indicator
- **Responsive Design** — mobile-friendly with touch device adaptations

## Getting Started

### Prerequisites

- Modern web browser
- Node.js / npm (only for Supabase dependency)

### Install

```bash
npm install
```

### Run

**Option A — Direct open:**

Double-click `index.html`.

**Option B — Local server (recommended):**

```bash
npx serve .
```

Then open `http://localhost:3000`.

## Project Structure

```
├── index.html                  # Entire site (HTML + CSS + JS)
├── package.json                # Supabase dependency
├── .env.local                  # Supabase credentials
├── images/
│   ├── rohan-portrait.jpg      # About section portrait
│   └── gallery/                # 6 photography images
└── videos/
    ├── hero-bg.mp4             # Hero background video
    ├── hero-bg-poster.jpg
    ├── project-one.mp4
    ├── project-one-poster.jpg
    └── strip/                  # 5 scrolling strip videos
```

## Configuration

The contact form requires Supabase credentials in `.env.local`:

```
NEXT_PUBLIC_SUPABASE_URL=your-url
NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY=your-key
```

## License

Personal portfolio — not open source.
