# Fahaadi Portfolio

A lightweight, responsive personal portfolio built with plain HTML, CSS, JavaScript, and a small local audio file.

## Features

- Minimal dark theme with restrained red accents.
- Two fast, seamless technology rails combining HTML5, CSS3, JavaScript, MySQL, Discord.js, Git/GitHub, Vercel, Railway, Cloud/cPanel hosting, NPM, terminal, SQL, webhooks, system architecture, Git workflow, bug fixing, and frontend/backend development.
- Lightweight entrance animations and scroll reveals.
- Programmed AI face illustration made entirely with inline SVG and CSS (the reference portrait is not embedded as a raster image).
- Subtle 3D tilt interactions on the AI illustration and project cards.
- Discord profile card with display name `! Fahad`, username `eh.s`, status, bio, member-since date, avatar, and banner.
- X and Kick links; GitHub and Store remain marked as coming soon.
- Work showcase for Discord System Bot, PHUB / Police Hub, Dispatch UI, website design, and logo/brand design.
- Background music player with play/pause controls and autoplay fallback.
- Responsive layout and Riyadh local clock.
- No project download buttons.

## Preview locally

Keep the `assets` folder next to `index.html`, then open `index.html` in a modern browser. The background track is `assets/midnight-signal.mp3`.

The Discord avatar and banner currently reference the two Discord CDN URLs supplied for this update. Those links are signed and temporary; if Discord expires them, save the images locally in `assets/` and replace the two `src` values in `index.html` with `assets/discord-avatar.webp` and `assets/discord-banner.webp` respectively.

## Deploy for free

### Cloudflare Pages
1. Create a Cloudflare account.
2. Open **Workers & Pages** → **Create application** → **Pages** → **Upload assets**.
3. Upload the contents of this folder, including the `assets` folder. Keep `index.html` at the project root.
4. Deploy. Cloudflare will provide a `*.pages.dev` address.

### Vercel
1. Import this folder into a GitHub repository or use Vercel's supported deployment flow.
2. Choose the project and deploy it as a static site.
3. Vercel will provide a `*.vercel.app` address.

## Customize

- Change the profile content and social links in `index.html`.
- Replace the Discord avatar/banner image URLs with local files for permanent hosting.
- Replace `assets/midnight-signal.mp3` with your own licensed audio if desired; keep the filename or update the `<audio>` source.
- Add or edit projects by copying a `<article class="work-card">` block.


## AI visual
The AI portrait is the original artwork (`assets/ai-agent.png`), now rendered live in WebGL with Three.js. The face is lifted into a 3D relief that follows the pointer, and the circuits, eyes, central bar and background rings animate. The Three.js library loads from cdnjs, and the artwork is also embedded in `index.html` so it works when opened directly from disk. If WebGL or the library is unavailable, the static image in `assets/ai-agent.png` is shown instead. Motion is reduced when the visitor prefers reduced motion.
