# Wello Reach — Accessible Wayfinding

**Wello Reach** is an interactive, mobile-friendly navigation *prototype* built for a design project. Its core idea is **“The interface adapts to your reach, not the other way around.”**

The app presents a journey from **Dhoby Ghaut MRT or Plaza Singapura Level 1 to the entrance of Temasek Shophouse**. It focuses on how people use their phones while travelling, including handheld and wheelchair-mounted phones.

## Features

- Two starting locations: Dhoby Ghaut MRT (includes station levels) and Plaza Singapura L1 (skips lower MRT levels).
- Handheld or wheelchair-mounted phone mode.
- Left, Centre or Right comfortable-touch area selection.
- Main navigation button moves to the selected side; the centre mounted mode uses an extra-wide button.
- Step-by-step image and map directions with Back, Pause, “I'm lost” and Adjust controls. Adjusting the reach zone keeps the current step.
- Enlarged reference photos/maps, responsive phone layout, visible focus states, keyboard navigation and reduced-motion support.
- Route A/B comparison intentionally removed from the required flow to reduce unnecessary selections.

## Open locally

Open `index.html` in a browser. No build system, dependencies, accounts or API keys required. Use a local HTTP server if your browser restricts local resources, for example:

```bash
python3 -m http.server 8000
```

then open <http://localhost:8000>.

## Publish publicly on GitHub Pages

1. Sign in to GitHub. Create a **new public repository**, such as `wello-reach`.
2. Upload `index.html`, `styles.css`, `app.js`, and `README.md` to the repository root, then commit.
3. Open **Settings → Pages** in the repository, set **Source: Deploy from a branch**, **Branch: main**, **Folder: / (root)**, and Save.
4. Open the URL GitHub Pages displays, normally `https://YOUR_USERNAME.github.io/wello-reach/`.

> **Note:** The GitHub repository being public does **not** publish a website automatically; GitHub Pages must be enabled separately.

## Images and route safety

This code displays the original map illustrations and location photos from the previously published Wello website, through image URLs of the form:

`https://wello-accessible-wayfinding.vercel.app/assets/street_1.png`

The assets are **not included in this source archive**; the original Wello deployment must stay available for these images to appear. To make this project fully standalone, download authorized copies of those images into an `assets/` folder and update `ORIGINAL_ASSET_BASE` in `app.js` to `./assets/`.

**This is a static classroom prototype, not real-time GPS navigation.** It does not track location, confirm current lift availability, or validate ramps, crossings, accessible door clearances or route safety. The route references should be checked on site with wheelchair users before real-world use. The demo asks users to make adjustments while stationary.

## Files

- `index.html` — page markup and metadata
- `styles.css` — responsive UI styling and accessible focus states
- `app.js` — route data, state, controls and screen transitions
- `README.md` — instructions and limitations

## Demo flow

Home → Choose start → Choose Handheld or Mounted → Choose Reach zone → Journey overview → Directions (Next / Back / Pause / I'm lost / Adjust) → Arrival.