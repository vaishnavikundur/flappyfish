Flappy Fish — asset notes

If the fish or background images do not appear when running the game, check these:

- The game loads images from the working directory at runtime. When run from the repository root, assets are expected under `src/` (e.g. `src/fish.png` and `src/bg.png`).
- The code also tries `assets/fish.png` and `fish.png` as fallback paths for the fish image.
- If a texture file exists but fails to decode, replace it with a valid PNG/JPEG or use the included fallback images.

