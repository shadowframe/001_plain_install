# Copilot instructions (auto-generated)

Overview
- Minimal three.js app served by Vite.
- Entry point: `main.js` (ES module). `index.html` loads `/main.js` as module; `public/` holds static assets.

Build, test, and lint commands
- Install dependencies: `npm install`.
- Start dev server (dev): `npx vite`.
- Build production bundle: `npx vite build`.
- Preview production build: `npx vite preview`.
- Tests: none configured in this repo. Suggested commands if adding a test runner:
  - Vitest (example single test): `npx vitest -t "<pattern>" --run`
  - Jest (example single test): `npx jest -t "<name>"`
- Lint: none configured. If ESLint is added, lint a single file with `npx eslint path/to/file.js`.

High-level architecture
- Runtime: Vite dev server serves a static `index.html` and ES modules.
- Rendering: `main.js` creates a `THREE.Scene`, `PerspectiveCamera`, and `WebGLRenderer`, adds a Mesh (cube), and uses `renderer.setAnimationLoop(animate)` to render.
- Dependencies: `three` is the only production dependency; `vite` is a dev dependency.
- File layout conventions: project root contains `index.html` and `main.js`; `public/` for static assets. Consider adding a `src/` folder if the project grows.

Key conventions and patterns
- ES modules: always `import * as THREE from 'three';`.
- Formatting: 2-space indentation; try to keep lines under ~80 chars (per AGENTS.md).
- No TypeScript currently; introduce it intentionally and incrementally if desired.
- Animation loop: prefer `renderer.setAnimationLoop` (used in code) to manage the render loop and VR compatibility.
- Assets: place static files in `public/` so Vite serves them at root.
- When adding tests, place them beside implementation files (e.g., `main.test.js`) and configure `vitest` or `jest` in package.json scripts.

Agent and AI-related docs
- See `AGENTS.md` for additional guidelines (build/start suggestions and style rules). There are no other AI assistant config files detected (e.g., CLAUDE.md, .cursorrules) in the repository root.

Notes for future Copilot sessions
- Primary intent: small, modular three.js examples using Vite.
- Keep changes minimal and create `src/` when adding more code; update `index.html` import if moving `main.js`.


