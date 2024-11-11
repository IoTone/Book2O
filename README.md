# Immersive Book 2.0

This is the **Immersive Book 2.0** project, an Immerse The Bay 2024 team project at Stanford on 11/8-10, 2024.

Original project idea is described [here](https://qiita.com/truedata_iotone/items/e73aa5dc98a9fba46a60#book20---a-rethinking-of-books-in-xr)

## Team
- David Kordsmeier
- Kazuki Yoda
- Victor Arroyo
- Youssif Seisa

# Get Started
## Build & Launch Server
```
cd ImmersiveBook2\prototypes\elixr-poc1
npm install
npm serve
```

## Demo
1. On Meta Quest3 (or similar versions), connect to the same local WiFi network as the web server (`XR Hackathon 5GHz` at the venue)
2. Open the browser and type the local IPv4 address + port, such as `https://10.20.30.40:8081/`
3. Allow VR mode on the browser. (Enable if not yet by the browser settings.)
4. Click the gray `Enter VR` button at the top-left with the Meta Quest controller.

# Architecture
### Hardware Requirements
- Meta Quest 3/3s (VR)
- Chrome Browser/PC/Mac/Linux
- NVIDIA GPU

### Software Requirements
- Node.js (Web server)
- Three.js (3D rendering)
- WebXR (VR mode on WEB browser)
- Python (backend/ML)

### External AI/ML Tools
- Stable Diffusion (SDXL) (Image Generation)
- A1111 WebUI (Pipeline/API for Stable Diffusion)
- [ControlNet](https://github.com/lllyasviel/ControlNet) (Guided image generation on Stable Diffusion)
- [DUSt3R: Geometric 3D Vision Made Easy](https://github.com/naver/dust3r) (Image to multi-view consistent poing cloud)
- [LucidDreamer: Domain-free Generation of 3D Gaussian Splatting Scenes](https://github.com/luciddreamer-cvlab/LucidDreamer) (point cloud)
- [DreamScene360: Unconstrained Text-to-3D Scene Generation with Panoramic Gaussian Splatting](https://github.com/ShijieZhou-UCLA/DreamScene360)
- OpenAI API (GPT-4o/4V) (Preprocessing of book/texts and Stable Diffusion's prompt generation)
- [RunPod](https://www.runpod.io/) (cloud GPU server)

## Code struecture
- src : the final source code
- assets: a JSON file containing links to any static assets
- pipeline: this is the generative AI pipeline in combination with the graphics pipeline
- prototypes: these are early prototypes that may later be thrown out or kept for historical reasons


# Additional Information
## Attributions

- Elixr Prototype: https://elixrjs.io/index.html
- Meta WebXR example for Quest: https://github.com/meta-quest/webxr-first-steps
- AFrame examples: https://glitch.com/~aframe-basic-guide
- Content: https://sketchfab.com/3d-models/cartoon-lowpoly-small-city-free-pack-edd1c604e1e045a0a2a552ddd9a293e6
- sky.jpg from Basic Scene - A-Frame

## Further Reading

- https://developers.meta.com/horizon/documentation/web/webxr-bp/
- https://threejs.org/manual/#en

## Inspirations

- AR.js prototype: https://ar-js-org.github.io/AR.js-Docs/

## License

MIT/X
