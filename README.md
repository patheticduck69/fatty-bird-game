# 🐦 FATTY BIRD

### A browser-based arcade flight game built around skill, timing, and changing hazards.

**Fly smart. React fast. Master every ability. Survive the unexpected.**

Fatty Bird combines six playable birds, character-specific abilities,
unlockable progression, changing obstacle patterns, and a dedicated Cave
Zone.

**Play:** https://patheticduck69.github.io/fatty-bird-game/\
**Repository:** https://github.com/patheticduck69/fatty-bird-game

------------------------------------------------------------------------

## What makes Fatty Bird stand out

The latest release brings together a set of mechanics designed to make
each run more than a repeated obstacle-dodging challenge:

-   Three sustained abilities---Sky Glide, Shadow Phase, and Time
    Warp---can be manually cancelled with a second tap.
-   A progression-based Cave Zone with variable ceiling and floor
    formations.
-   Safe corridors, warning cues, and reaction windows for major
    hazards.
-   Cave coin trails, bombs, and pressure-plate-triggered falling cage
    traps.
-   A pipe-retraction event that warns players before pipe pairs
    retract; the rotor remains hazardous.
-   A redesigned defeat effect using two red pixel crosses aligned with
    the bird's eyes.
-   A built-in, illustrated 12-slide Help & Skill Guide.
-   New obstacle artwork, guide illustrations, and additional animated
    backgrounds.

The ambition is not to claim that no other game has any one of these
features. It is to bring this particular combination of mechanics,
visual feedback, and learning tools into one lightweight browser game.

## Meet the birds

  -----------------------------------------------------------------------
  Bird                                Ability / trait
  ----------------------------------- -----------------------------------
  **Original Fatty**                  Pulse Lift --- a quick upward boost

  **Blueberry Blimp**                 Sky Glide --- sustained
                                      parachute-style descent control

  **Chili Puff**                      Ember Burst, with passive arrow
                                      immunity

  **Mint Mochi**                      Mint Bubble --- a timed protective
                                      shield

  **Midnight Dumpling**               Shadow Phase --- a sustained phase
                                      ability

  **Royal Roast**                     Time Warp, plus one extra life per
                                      run
  -----------------------------------------------------------------------

### Ability rules

-   **Sky Glide, Shadow Phase, and Time Warp:** tap again to cancel
    early. Early cancellation does not refund the cooldown.
-   **Mint Bubble:** remains active for its timed duration; a second tap
    does not switch it off.
-   **Pulse Lift and Ember Burst:** instant abilities, not sustained
    toggles.
-   **Royal Roast's extra life:** passive run benefit.

Different ability types have deliberately different rules, so players
can understand which effects are cancellable and which run their full
duration.

## The Cave Zone

The Cave Zone changes the rhythm of a run. Players navigate
variable-length formations with shifting ceiling and floor obstacles
rather than relying only on familiar pipe gaps.

It includes:

-   Variable ceiling and floor formations with a safe passage.
-   Coin trails that create optional risk-and-reward decisions.
-   Bomb hazards.
-   Pressure plates that trigger falling cage traps.
-   Warning cues and a dodge window before a cage falls.
-   A controlled cave-entry transition that waits for active projectiles
    and special hazards to clear while preserving a safe entry band.

Balloons are disabled in the Cave Zone to keep its hazard design
focused.

## Dynamic pipe-retraction event

An advance warning precedes the retraction of upcoming pipe pairs. The
rotor remains a hazard, so the event changes the obstacle layout without
turning the sequence into a free pass.

## Updated defeat effect

The revised death animation uses two red pixel crosses positioned over
the bird's eye locations, replacing the earlier hazy-eye effect.

## Illustrated Help & Skill Guide

The release includes **12 illustrated slides** explaining controls,
birds, abilities, cooldowns, manual cancellation, hazards, Cave Zone
navigation, cave coins, bombs, pressure plates, falling cage traps,
pipe-retraction events, and survival tips.

The guide is built into the game interface so players can learn the
mechanics while playing.

## Backgrounds and visual assets

The updated background manifest includes the existing MP4 backgrounds
alongside three additional GIF backgrounds:

-   `Railway_station_game_background_4c4de770.gif`
-   `Camera_racing_through_exploding_scene_128e91d1.gif`
-   `InShot_20261101_163109258.gif`

The file names and letter case must match the manifest exactly.

## Play

Fatty Bird is published as a static browser game through GitHub Pages.

**[▶ Play Fatty
Bird](https://patheticduck69.github.io/fatty-bird-game/)**

Open the in-game Help / Guide for explanations of the latest mechanics.

## Repository update map

The latest package is a **delta update**, not a complete repository
replacement.

  -------------------------------------------------------------------------------------------------------
  Package content                         GitHub destination                      Action
  --------------------------------------- --------------------------------------- -----------------------
  `index.html`                            `/index.html`                           Replace existing file

  `assets/backgrounds/backgrounds.json`   `assets/backgrounds/backgrounds.json`   Replace existing
                                                                                  manifest

  18 obstacle PNG files                   `assets/obstacles/`                     Add the new files

  12 guide PNG files                      `assets/ui/guide/`                      Create folder if
                                                                                  needed, then add files

  3 GIF backgrounds                       `assets/backgrounds/`                   Add the files
  -------------------------------------------------------------------------------------------------------

**Do not delete or replace the complete `assets/` directory.** Preserve
existing character artwork, audio, MP4 background videos, and obstacle
files unless a future release explicitly says otherwise. The original
`pixel-arrow.png` and `sky-bomb.png` assets are not duplicated in the
update package.

## Design principles

-   **Player agency:** sustained abilities can be cancelled where the
    mechanic supports it.
-   **Consistent rules:** passive, instant, timed, and toggleable
    abilities behave differently by design.
-   **Readable danger:** major hazards use warnings and reaction
    opportunities.
-   **Fair transitions:** Cave Zone entry should not place the player
    directly into an uncleared projectile or special hazard.
-   **Incremental updates:** new releases should not erase unrelated
    assets.
-   **Learnability:** the illustrated guide explains mechanics instead
    of leaving players to guess.

These are design and implementation goals, not a claim that the game is
bug-free on every browser or device. Verify the deployed build on the
target browser and device after each update.

## Post-deployment checklist

-   [ ] Game loads and the main menu works.
-   [ ] Help / Guide opens and all 12 slides display.
-   [ ] Previous / Next, page dots, and mobile swipe work.
-   [ ] Blueberry can activate and cancel Sky Glide.
-   [ ] Midnight can activate and cancel Shadow Phase.
-   [ ] Royal Roast can activate and cancel Time Warp.
-   [ ] Early cancellation does not refund cooldown.
-   [ ] Mint Bubble remains active for its timed duration.
-   [ ] Cave Zone appears during progression.
-   [ ] Cave formations leave a safe route.
-   [ ] Coins, bombs, pressure plates, and cage warnings behave
    correctly.
-   [ ] Cave entry waits for active hazards to clear.
-   [ ] Pipe-retraction warning appears and the rotor remains hazardous.
-   [ ] Updated defeat animation is visible.
-   [ ] All three GIF backgrounds load.
-   [ ] Existing characters, audio, MP4 backgrounds, and progression
    remain intact.

------------------------------------------------------------------------

**Learn the pattern. Time the ability. Find the safe line. Keep
flying.**
