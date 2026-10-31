# Audio setup — exact filenames and timing

All three MP3s are already included in `assets/audio/`. No Google Drive link, external audio host, or additional download is used during gameplay.

| Exact filename | Role | Timing |
|---|---|---|
| `menu-music.mp3` | Existing menu/background music from the previous Fatty Bird build | Loops on the menu and during flight. Attempts autoplay on page load; if Chrome blocks it, retries on the first normal tap, click, or key press. Pauses during pause/game-over and resumes when play continues. |
| `gopgopgop (mp3cut.net).mp3` | Coin pickup sound effect | Plays once for each successfully collected coin. |
| `annoy rec gali (mp3cut.net).mp3` | Collision/game-over sound effect | Starts immediately after collision, alongside the short drowsy reaction. |

## Folder layout

Keep these files together in `assets/audio/`:

```text
assets/
  audio/
    menu-music.mp3
    gopgopgop (mp3cut.net).mp3
    annoy rec gali (mp3cut.net).mp3
```

## If you replace a track later

Upload the replacement MP3 into the same folder and keep the exact filename shown above. If you choose a different filename, update the matching relative path in `index.html`. Keep menu music separate from event sound effects.

## Browser autoplay note

Browsers can block audio that starts without a user gesture. The game attempts menu-music autoplay on page load and also retries on the first interaction. No web page can guarantee audible autoplay in every browser or device configuration. The audio button remains available to mute/unmute the three audio tracks.
