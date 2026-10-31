# FATTY BIRD — GitHub Pages project

A mobile-friendly Flappy-style arcade game built with HTML5 Canvas and JavaScript. It runs as a static website: no framework, build step, server, sign-in, tracker or external game service is needed.

## Quick start

1. Extract `Fatty_Bird_GitHub_Pages.zip`.
2. Keep the structure unchanged: `index.html` must sit beside the `assets` folder.
3. All three audio files are already included in `assets/audio/`; no renaming or additional download is required.
4. Open `index.html` in Chrome to test locally, or publish the project through GitHub Pages.

## Controls

- Tap / click: start or flap.
- Space / Arrow Up: start or flap on keyboard.
- Pause: pause / resume.
- Audio: toggle the one menu-music track and the two event sounds.
- About: opens the fictional-purpose disclaimer.

## Audio map

| File | Role | Timing |
|---|---|---|
| `assets/audio/menu-music.mp3` | The one existing BGM track from the previous build; already included | Loops on the menu and during flight. Attempts autoplay on page load; if blocked, retries on the first user gesture. Pauses on pause/game-over and resumes on retry/home. |
| `assets/audio/gopgopgop (mp3cut.net).mp3` | Coin pickup SFX | Plays once for each collected coin. |
| `assets/audio/annoy rec gali (mp3cut.net).mp3` | Collision/game-over SFX | Plays once immediately after collision, during the drowsy reaction. |

All three MP3 files are physically included in this project. Nothing is fetched from Google Drive or another online music source during gameplay. If you replace a sound later, keep its filename and folder path unchanged; see `AUDIO-SETUP.md`.

## GitHub Pages publishing

1. Create a new repository on GitHub.
2. Extract the ZIP on your phone or computer.
3. Upload the **contents** of the extracted project to the repository root, not the ZIP itself. The root should contain `index.html`, `README.md`, `AUDIO-SETUP.md`, `CREDITS.md`, `.nojekyll` and the `assets` folder.
4. Open **Settings → Pages**.
5. Under **Build and deployment**, select **Deploy from a branch**.
6. Select the `main` branch and `/ (root)`, then Save.
7. Open the Pages URL shown by GitHub.

All game assets use relative paths, so GitHub Pages serves the HTML, videos, image assets and audio from the same project. No Drive URLs or separate hosting links are required.

## Gameplay and animation

- Previous flight feel preserved: original flap impulse, gravity, obstacle speed curve and smoothed bird pitch are retained.
- Main bird artwork is approximately 10% smaller in flight, with a reduced hitbox to make collisions fairer.
- Feather layers animate behind the unchanged face/body artwork. This is a visual wing-flap effect; it does not alter flight physics.
- A brief white-eyed, wobbling, drowsy reaction appears after a collision before the results panel.
- Coins spawn in short waves along the flight route, with gaps between waves; they are not restricted to pipe gaps.
- Run coins and the total coin wallet are saved locally in the browser.
- Background order: Night City → Washroom → G. B. Road / Sonagachi City → Stadium. Each MP4 plays twice before the next scene. Background playback speed increases with game difficulty.

## Disclaimer

The About screen describes the game's fictional and satirical entertainment purpose. A disclaimer cannot guarantee immunity from legal claims; content and context still matter. Avoid presenting false factual allegations about identifiable people.
