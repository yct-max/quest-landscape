# VR Landscape for Meta Quest

A simple VR app showing a forest landscape with trees, built with A-Frame (WebXR).

## How to Run

### Option 1: Quick - Run in Quest Browser
1. Host this somewhere (GitHub Pages, Netlify, Vercel, etc.)
2. Open the Meta Quest Browser
3. Navigate to your hosted URL
4. Click the VR button in the bottom-right to enter immersive mode

### Option 2: Local Development
1. Install Node.js
2. Run `npx serve` in this directory
3. Access via your computer's IP on the same network
4. Or use Quest's developer mode with `adb reverse`

## Controls

- **Move:** WASD keys (desktop) / Thumbstick (VR)
- **Look:** Mouse drag (desktop) / Head movement (VR)
- **Enter VR:** Click the VR button in bottom-right corner

## Tech Stack

- [A-Frame](https://aframe.io/) - WebXR framework
- [A-Frame Environment Component](https://github.com/c-frame/aframe-environment-component) - Procedural environments

## Customization

Edit `index.html` to change:
- Tree positions, sizes, colors
- Environment preset (try: `arches`, `yavapai`, `osiris`, `poison`)
- Lighting and sky settings
