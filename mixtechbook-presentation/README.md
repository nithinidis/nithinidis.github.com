# MixTechBook — Presentation Deck

A 17-slide research presentation deck for the AcademyEX MTFC9890 Technological Futures Project.

**Title:** MixTechBook — The Future of Immersive Learning
**Researcher:** Nithin Lanka Dissanayake
**Year:** 2026

## What's in this folder

```
mixtechbook-deck/
├── index.html           ← landing page with slide directory
├── slide-01.html        ← title slide
├── slide-02.html        ← research question
├── ...                  ← slides 03–16
├── slide-17.html        ← references & thank you
└── assets/
    ├── prototype-heart.png    ← VR heart screenshot
    ├── ar-demo.png            ← AR demo image (slide 6)
    ├── vr-demo.png            ← VR demo image (slide 6)
    └── 3d-demo.png            ← 3D simulation image (slide 6)
```

## Running it locally

Just open `index.html` in any modern browser (Chrome, Firefox, Safari, Edge). No server needed for local viewing.

## Hosting on GitHub Pages

### 1. Create a new GitHub repository

Go to github.com → **New repository**. Name it whatever you want (e.g. `mixtechbook-presentation`). Make it **Public** (free GitHub Pages requires a public repo). Don't add a README — we have one.

### 2. Upload the files

The simplest method is the web upload:

1. Open your new repo
2. Click **"uploading an existing file"** on the welcome screen
3. Drag and drop ALL the files from this folder (`index.html`, all 17 `slide-*.html` files, and the `assets/` folder) into the upload area
4. Scroll down and click **Commit changes**

Alternative: use Git CLI

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
cd YOUR_REPO_NAME
# copy all files from mixtechbook-deck into here
git add .
git commit -m "Initial deck upload"
git push origin main
```

### 3. Enable GitHub Pages

1. In your repo, go to **Settings** (top-right tabs)
2. Click **Pages** in the left sidebar
3. Under **Build and deployment**, set **Source** to **"Deploy from a branch"**
4. Set **Branch** to `main` and folder to `/ (root)`
5. Click **Save**

### 4. Wait ~1 minute, then visit

Your deck will be live at:

```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
```

The first build can take 30 seconds to 2 minutes. Refresh if it 404s the first time.

## How to navigate during a presentation

Every slide has the same controls:

- **→** or **Spacebar** or **Page Down** — Next slide
- **←** or **Page Up** or **Backspace** — Previous slide
- **Home** — Jump to first slide
- **End** — Jump to last slide
- **F11** — Toggle full-screen (works on most browsers)

You can also use the **prev/next buttons** in the bottom-right corner of every slide. They fade out when idle and reappear when you move the mouse.

If you have a clicker / wireless presenter remote, the standard ones (Logitech, etc.) typically send Page Up/Down keys, which this deck handles natively.

## Tips for presentation day

1. **Test the venue's wifi** — slide 2 has a YouTube video that needs internet. If wifi is unreliable, ask me for an offline-embedded version.
2. **Press F11 before you start** — full-screen mode hides browser chrome (URL bar, tabs) so the deck looks polished.
3. **Open slide 10's GitHub link in a separate tab beforehand** — that way clicking the link during the presentation feels instant.
4. **Slide 13 is the moment** — bring the actual phone with the VR prototype loaded. Pass it around. The slide just sets the stage.

## Built with

- HTML, CSS, vanilla JavaScript — no build step, no framework
- Google Fonts (Fraunces, Geist, Geist Mono, Caveat)
- Embedded SVG illustrations for the character throughout
- Embedded base64 images where useful (slide 13's prototype heart, slide 2's worksheets)
- YouTube iframe for the prototype video on slide 2
