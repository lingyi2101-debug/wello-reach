# Wello Reach — Accessible Wayfinding

**Wello Reach** is a public, one-page interactive prototype for a Human-Centred Design project.

**Design statement:** *The interface adapts to your reach, not the other way around.*

## What it does

The prototype guides visitors to the **Temasek Shophouse entrance** from two starting points:

- **Dhoby Ghaut MRT** — includes the MRT B2/B1 indoor reference steps, Plaza Singapura L1 and four outdoor photo steps.
- **Plaza Singapura Level 1** — skips MRT B2/B1 and starts from Plaza L1, followed by the same four outdoor photo steps.

The concept focuses on **how people operate a phone during a journey**. Users can choose **Handheld** or **Mounted on chair**, then place the main navigation control at the **Left**, **Centre** or **Right** reach area. The choice remains available through **Adjust** during navigation, without losing the current step. It also offers **Next**, **Back**, **Pause**, **I'm lost?**, enlarged route photos/maps, keyboard controls, visible focus indicators and reduced-motion-friendly CSS.

Route A/B comparison is omitted from the required flow to reduce repeated choices.

## Use

This repository has a single self-contained **`index.html`** file containing its HTML, CSS and JavaScript. No build step or dependencies are required.

To use locally, download and open **`index.html`** in your browser.

To publish on **GitHub Pages**:

1. Open this repository on GitHub.
2. Select **Settings → Pages**.
3. Under **Build and deployment**, set **Source: Deploy from a branch**, **Branch: main**, **Folder: / (root)**, then **Save**.
4. When GitHub shows the live website link, open it. For this repository, the expected Pages address is **https://lingyi2101-debug.github.io/wello-reach/**. It will only work after GitHub Pages is enabled and deployment completes.

## Photos and map sources

The prototype uses the original maps and street photographs from the earlier Wello website at:

`https://wello-accessible-wayfinding.vercel.app/assets/`

This GitHub repository **does not contain local copies of those images**. Keep the previous website online to make sure maps and photos display in Wello Reach. If you later move the images into this repository, update the asset base URL in `index.html`.

## Important safety disclaimer

This is a **classroom prototype**, not a live GPS system. It does not detect your location, verify open lifts, or confirm that ramps, doors, crossings and pavement conditions are currently accessible. Photos and directions are reference material only. Verify all physical route details with wheelchair users on site before real-world navigation.

**Scope:** Only MRT / Plaza Singapura L1 → Temasek Shophouse entrance, not navigation inside the exhibition.
