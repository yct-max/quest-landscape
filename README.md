# Quest Landscape

A lightweight A-Frame / WebXR landscape demo with a controllable character for phone and Meta Quest.

## Current Features

- Third-person movement on phones and desktop
- On-screen thumbstick for touch movement
- Right-side drag look on phones
- Keyboard movement on desktop (`WASD` / arrow keys)
- WebXR / Meta Quest browser support
- Real 3D character model (`RobotExpressive.glb`)
- Simple world collision and map boundaries
- Ground clamping so the player stays on the terrain plane

## Controls

### Phone
- **Left thumb:** movement joystick
- **Right side drag:** rotate camera / look around

### Desktop
- **Move:** `WASD` or arrow keys
- **Look:** mouse / drag

### Meta Quest
- Open in Quest Browser and tap the **VR** button
- In immersive mode the camera switches to first-person

## Collision / Boundaries

The player is constrained to a bounded grove and cannot walk through the major trees / rocks placed in the scene.

## Local Development

```bash
npx serve
```

Then open the URL locally or from another device on the same network.

## Next Good Upgrades

- Character animation state switching (idle / walk)
- Quest controller locomotion in immersive mode
- Better terrain / elevation
- Replace CDN-hosted model with a local asset in the repo
- Native Android / Quest wrapper packaging polish
