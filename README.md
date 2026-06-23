# Neon Cursor Dragon

An interactive browser dragon built with Vite, Three.js, and SVG layers. The dragon follows the cursor with segmented motion, a black background, neon glow, and colored wing accents.

## Features

- Full-screen interactive dragon animation
- Cursor and touch tracking
- Segmented snake-like dragon motion
- Neon green and pink wing glow
- Black-background presentation
- GitHub Pages-ready static build in `docs/`

## Run Locally

Install dependencies:

```bash
npm.cmd install
```

Start the development server:

```bash
npm.cmd run dev
```

Open the local URL Vite prints in the terminal, usually:

```text
http://127.0.0.1:5173/
```

## Build

Create a normal production build:

```bash
npm.cmd run build
```

Create the GitHub Pages build:

```bash
npm.cmd run build:pages
```

The GitHub Pages build outputs to:

```text
docs/
```

## GitHub Pages

This repo is ready to publish from the `docs` folder.

In GitHub:

1. Go to **Settings**.
2. Open **Pages**.
3. Set **Source** to **Deploy from a branch**.
4. Select your branch, usually `main`.
5. Set the folder to `/docs`.
6. Save.

After pushing, GitHub will publish the site from `docs/index.html`.

## Project Structure

```text
.
├── docs/                  # GitHub Pages static build
├── public/assets/          # Source static assets copied by Vite
├── src/main.js             # Three.js scene and dragon behavior
├── src/styles.css          # UI and SVG visual styling
├── index.html              # App shell
└── package.json            # Scripts and dependencies
```

## Credits

- Dragon artwork reference: **Dragon by GifHaas** on DeviantArt  
  https://www.deviantart.com/gifhaas/art/Dragon-8681899

Asset source notes are included in:

```text
public/assets/reference-dragon/SOURCE.txt
docs/assets/reference-dragon/SOURCE.txt
```

## Notes

If you change the source files, rerun:

```bash
npm.cmd run build:pages
```

Then commit the updated `docs/` folder so GitHub Pages serves the latest version.
