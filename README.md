# Adam — AI Text-to-CAD Generator

An AI-powered CAD web app that turns plain-language prompts into 3D CAD models. Describe what you want to build — "Speak anything into existence" — and get an interactive 3D model you can inspect, rotate, and iterate on, right in the browser.

Originally generated with Lovable and refined as part of the LadeStack open-source collection.

## Features

- **AI chat-driven CAD generation** — prompt-based workflow: type a description, get a 3D model
- **Interactive 3D viewer** — real-time Three.js viewport with orbit/zoom/pan (react-three-fiber + drei)
- **Landing + chat UI** — marketing hero sections (example chips, announcement bar, YC-style badge, search bar) plus a full chat interface
- **Modern UI kit** — shadcn/ui components, Tailwind CSS, dark theme, responsive layout
- **Client-side rendering** — no backend required; everything runs in the browser

## Tech Stack

- **Framework:** Vite 5 + React 18 + TypeScript
- **3D:** Three.js, @react-three/fiber, @react-three/drei
- **UI:** shadcn/ui, Radix UI primitives, Tailwind CSS, Tailwind Animate
- **Utilities:** react-router-dom, TanStack Query, react-hook-form, Zod, recharts, Framer-style animations (vaul, cmdk)

## Project Structure

```
CAD-with-AI/
├── index.html              # HTML entry, page title "Adam"
├── src/
│   ├── main.tsx            # React entry point
│   ├── App.tsx             # App shell, routing
│   ├── pages/
│   │   ├── Index.tsx       # Landing page (hero, features, 3D showcase)
│   │   ├── Chat.tsx        # AI chat / CAD generation interface
│   │   └── NotFound.tsx    # 404 page
│   ├── components/
│   │   ├── Interactive3DViewer.tsx  # Three.js model viewer
│   │   ├── chat/           # Chat UI components
│   │   ├── ui/             # shadcn/ui components
│   │   └── ...             # Landing sections (hero, search bar, badges)
│   ├── hooks/              # Custom React hooks
│   ├── lib/                # Utilities
│   ├── index.css           # Global styles, Tailwind
│   └── App.css
├── public/                 # Static assets
├── vite.config.ts
└── tailwind.config.ts
```

## Quick Start

Requirements: Node.js 18+ and npm.

```sh
# Clone
git clone https://github.com/girishlade111/CAD-with-AI.git
cd CAD-with-AI

# Install dependencies
npm install

# Start dev server
npm run dev
```

Open http://localhost:5173 in your browser.

## Build

```sh
npm run build
```

Outputs a production bundle to `dist/`, ready to serve as a static site.

## Deployment

Static output — deploy `dist/` to any static host (Netlify, Vercel, GitHub Pages, Cloudflare Pages). No environment variables required.

## License

Open source — free to use and adapt.

---

Built by Girish Lade — https://ladestack.in
