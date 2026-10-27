# FLAMEBITE — Built Hot. Served Loud.

Complete standalone download of the expanded FLAMEBITE website.
React + TypeScript + Tailwind CSS, packaged with Vite. No GSAP or backend required.

## Run on your computer
1. Install Node.js 22.13 or later (Node 24 LTS also works).
2. Extract this ZIP and open the FLAMEBITE folder in VS Code.
3. Open the VS Code terminal in that folder and run:

```bash
npm install
npm run dev
```

4. Open the local address printed by Vite (normally http://localhost:5173).

Do not double-click index.html: React/TypeScript requires the development server or a production build.

## Build / publish
```bash
npm run build
npm run preview
```
Upload the contents of `dist` to a static web host, or connect the project to Vercel/Netlify with build command `npm run build` and output directory `dist`. Serve from a domain root; image URLs are root-relative. Do not upload node_modules.

## Edit
- `src/App.tsx`: sections, menu, customizer, cart, scroll effects, and contact configuration.
- `src/index.css`: colors, typography, animations, desktop/mobile layouts.
- `public/images`: all included optimized food images.
- `index.html`: title, description and favicon.

At the top of App.tsx, change CONFIG.whatsapp from the placeholder 923000000000 to your actual WhatsApp number (country code, digits only). Also change CONFIG.instagram, CONFIG.directions and the footer social URLs to your real business accounts and address.

## Features
Burger assembly scroll animation; chapter-based grill story; horizontal desktop menu; category filters; burger customizer; Perfect Pair add-to-cart; FAQ accordions; responsive navbar with active sections and progress bar; animated footer; persistent local cart; itemized WhatsApp checkout; mobile and reduced-motion fallbacks.

## Important details
- This is a frontend website. WhatsApp opens a prepared order; the customer must send it.
- No payment is collected, and no backend order database is included.
- Prices and customizable extras are local data. Shakes show a coming-soon state.
- Pair prices are the sum of the two menu items, without an invented discount.
- Food images are serving inspiration, including AI-generated photorealistic assets and Unsplash photos.
- Google Fonts and WhatsApp need an internet connection. Food assets are included locally.
- This export uses standalone Vite rather than the managed hosting runtime. The live website was not modified by this export.

## Verification
TypeScript and the standalone production build were checked before packaging. Interactive browser testing was not available in the export environment.
