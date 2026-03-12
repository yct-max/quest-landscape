# Quest Landscape

A lightweight A-Frame / WebXR landscape demo with a controllable third-person character for phone and Meta Quest.

## Live Demo

- GitHub Pages: `https://yct-max.github.io/quest-landscape/`

## Current Features

- Third-person movement on phones and desktop
- On-screen thumbstick for touch movement
- Right-side drag look on phones
- Keyboard movement on desktop (`WASD` / arrow keys)
- WebXR / Meta Quest browser support through the browser VR button
- Real 3D character model (`RobotExpressive.glb` loaded at runtime)
- Simple world collision and map boundaries
- Ground clamping so the player stays on the terrain plane
- Capacitor Android wrapper for APK-based Quest testing

## Controls

### Phone
- **Left thumb:** movement joystick
- **Right side drag:** rotate camera / look around

### Desktop
- **Move:** `WASD` or arrow keys
- **Look:** mouse / drag

### Meta Quest Browser
- Open the live URL in Quest Browser
- Tap the **VR** button to enter immersive mode
- In immersive mode the camera switches to first-person

## Collision / Boundaries

The player is constrained to a bounded grove and cannot walk through the major trees / rocks placed in the scene.

## Project Structure

- `index.html` — main web app
- `app/index.html` — copied web payload used by Capacitor Android
- `android/` — native Android wrapper project
- `capacitor.config.json` — Capacitor app config
- `.github/workflows/build-quest-apk.yml` — CI workflow that builds the debug APK

## Local Development

Quick web test:

```bash
npx serve
```

Android sync after changing `index.html`:

```bash
npm run sync:android
```

Then open the URL locally or from another device on the same network.

## APK / Quest Testing

This repo includes a Capacitor-based Android wrapper for Quest testing.

To build in GitHub Actions:
1. Open the repo Actions tab
2. Run **Build Quest APK** or use the latest push-triggered run
3. Download the artifact named **`quest-landscape-debug-apk`**
4. Extract and sideload `app-debug.apk` onto Quest

## Notes

- The current character model is loaded from a CDN rather than stored locally in the repo.
- The APK path is meant for testing and iteration, not store-ready release packaging.

## Next Good Upgrades

- Character animation state switching (idle / walk)
- Quest controller locomotion in immersive mode
- Better terrain / elevation
- Replace CDN-hosted model with a local asset in the repo
- Native Android / Quest wrapper packaging polish
- Signed release APK / AAB flow
