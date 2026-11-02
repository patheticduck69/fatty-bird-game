# Audio setup — exact filenames and timing

All four MP3s live in `assets/audio/`. No external audio host or additional download is used during gameplay.

| Exact filename | Role | Timing |
|---|---|---|
| `menu-music.mp3` | Menu/background music | Loops on the menu and during flight. Attempts autoplay on page load; if the browser blocks it, retries on the first tap, click, or key press. Pauses during pause/game-over and resumes when play continues. |
| `gopgopgop (mp3cut.net).mp3` | Coin pickup sound effect | Plays once for each successfully collected coin. |
| `annoy rec gali (mp3cut.net).mp3` | Collision/game-over sound effect | Starts immediately after a collision, alongside the short drowsy reaction. |
| `Risa.mp3` | Cave monster sound (about 2.8 s) | Plays once when the flying monster appears at the start of the cave entrance, before it opens its mouth and bites the bird. Respects the AUDIO ON/OFF button. |

## Folder layout

Keep these files together in `assets/audio/`:

```text
assets/
  audio/
    menu-music.mp3
    gopgopgop (mp3cut.net).mp3
    annoy rec gali (mp3cut.net).mp3
    Risa.mp3
```

Filenames are case-sensitive on GitHub Pages. `Risa.mp3` must start with a capital R.

## Related monster images

The cave monster uses two images in `assets/ui/` (not audio, listed here so the set stays together):

```text
assets/
  ui/
    monster-closed.png    closed mouth: flying in and after the bite
    monster-open.png      open mouth: as the bird approaches and during the bite
```

The game loads these images and `Risa.mp3` when the page opens, so they are ready long before the cave entrance appears. If an image is missing or still not loaded after about 25 seconds, the game falls back to the built-in drawn dragon instead of freezing. The sound is not checked, so a slow connection can make the first monster silent.

## If you replace a track later

Upload the replacement MP3 into the same folder and keep the exact filename shown above. If you choose a different filename, update the matching relative path in `index.html`. Keep menu music separate from event sound effects.

## Browser autoplay note

Browsers can block audio that starts without a user gesture. The game attempts menu-music autoplay on page load and also retries on the first interaction. No web page can guarantee audible autoplay in every browser or device configuration. The audio button remains available to mute/unmute all audio tracks.
