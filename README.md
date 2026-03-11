# Quest Landscape

A lightweight A-Frame / WebXR landscape demo that now supports a proper controllable player.

## Features

- Third-person character on phones and desktop
- Simulated on-screen thumbstick for movement on touch devices
- Right-side drag look control on phones
- Keyboard movement on desktop (`WASD` / arrow keys)
- Meta Quest / WebXR support through the browser VR button
- Automatic camera switch:
  - non-VR: third-person follow camera
  - VR: first-person head camera

## Controls

### Phone
- **Left thumb:** movement joystick
- **Right side drag:** rotate camera / look around

### Desktop
- **Move:** `WASD` or arrow keys
- **Look:** mouse drag / mouse look

### Meta Quest
- Open in Quest Browser and tap the **VR** button
- In immersive mode, the camera switches to first-person

## Local Development

```bash
npx serve
```

Then open the local URL in a browser, or from another device on the same network.

## Deployment

This repo is set up to work well with GitHub Pages as a static site.

## Next Good Upgrades

- Replace the placeholder character with a GLB avatar
- Add animation states (idle / walk)
- Add collision and terrain constraints
- Map Quest thumbstick/controller input to locomotion in immersive mode
