# V3.0 — Complete 24-Skin Interface Repair

This repair uses 24 separately generated fantasy UI components (12 newly generated and 12 retained from the first generated sheet), with shape-matched bars and tiles, framed text-first modals, no full-frame image stretching, no decorated background behind long text, reduced header collisions, and iPad/iPhone responsive sizing. All embedded in CSS to maintain the strict 100-file limit. Game assets, saved games, songs, dogs, odds, prices, and seasonal schedules are unchanged.

# My Singing Dogs — V3.0: Five-Island Symphony

A self-contained, original browser music/creature-collection game. **No npm, server build, external library or account required.** Publish these files directly from a GitHub repository root using **Settings → Pages → Deploy from main / (root)**. A GitHub Pages website is public unless you use a separate authenticated hosting system.

## The first major content update

- **Five playable islands, all with FOUR elements and separate rich illustrated backgrounds:**
  - **Plant:** Wind, Stone, Tech, Water — *The Green Overture*, 2:17.
  - **Ice:** Wind, Stone, Tech, Cold — *Aurora Nocturne*, 2:40.
  - **Wind:** Wind, Stone, Cold, Water — *Cloudborne Symphony*, 2:28.
  - **Water:** Wind, Tech, Cold, Water — *Tidal Overture*, 2:34. Original generated reef artwork, atmospheric strings, sustained leads and gentle percussion.
  - **Rock:** Stone, Tech, Cold, Water — *Crimson Riff*, 2:10. Original generated volcanic-rock arena art, overdriven sustained guitar-like synthesizers, bass and drums.
- **Four elements per island** with 4 singles, 6 doubles, 4 triples, 1 quad, 1 Mythical, 1 Legendary and 1 Celestial: **18 main species per island**. The original V2 dog types, songs and save entries are retained. The collection now has **210 island/rarity entries**.
- **Legendary dogs:** Breed a **single + double**. 8% special-class success chance (no torch modifier). These dogs are not Howltron requirements.
- **Mythicals:** Breed a **double + triple**. 5% base, +1.5 percentage points per lit island torch, maximum 20%.
- **Celestials:** Breed a **quad + triple**. **2%** base, +1 percentage point per lit torch, **12%** with all ten lit. **Rare Celestial is 15%–35%** conditional on Celestial success, +2 percentage points per torch.
- **Rares:** Ordinary dogs: 4%–19% with torches. All five **Rare seasonals** have a special **15%–35%** conditional Rare-form roll.
- **All incubations cap at 4 hours** and speedups cost 1 gem per remaining hour, rounded up.
- **Howltron / Rare Howltron:** Shells still require 210,000 / 950,000 coins. Activation now consumes one of each of the **16 natural/quad/Mythical main dogs**, matching Common or Rare rarity. Legendaries, Celestials, Seasonals, wheel and ticket exclusives are excluded. Rare Howltron has a more elaborate generated clockwork sprite.

## Seasonals — always use America/New_York local time

Each active seasonal is a **12% special breeding result** from its named parent combination; the separate Rare roll is 15% with no lit torches, +2 percentage points per lit torch to 35% with all ten.

| Island | Seasonal | Annual availability | Weekly availability | Breeding parents |
| --- | --- | --- | --- | --- |
| Plant | **Springpup** | April 15–22 | Friday 3 PM–11 PM | Bitbit + Copperleaf |
| Ice | **Jinglepup** | December 15–30 | Thursday 11 PM–Friday 8 AM | Frostle + Glacierhorn |
| Wind | **Autumnpup** | October 1–13 | Friday 11 PM–Saturday 8 AM | Ripplet + Stormcaller |
| Water | **Valentail** | February 7–18 | Saturday 8 AM–7 PM | Ripplet + Oceanova (Water Quad) |
| Rock | **Summerpup** | May 18–June 3 | Saturday 7 PM–Sunday 5 AM | Boulder + Magmabyte (Rock Quad) |

DST/standard-time changes are handled using the actual America/New_York timezone, not an incorrectly fixed UTC offset. Seasonal eggs are 3h normal, 3h30 Rare.

## Diamond Deals (coins → diamonds/gems)

- 5,000 → 1
- 12,500 → 3
- 25,000 → 6
- 50,000 → 12
- 110,000 → 30
- 350,000 → 100
- 800,000 → 200

All seven deals exchange **earned in-game coins only**, with no payment processing or real money involved. Open **More → Diamond Deals**.

## Clearer interface

To avoid overwhelming new players, the main rail has **five controls**: Islands, Breed, Nursery, Collection and Market. The compact dock has **Bakery, Build, Events and More**. The More panel groups Wishing Torches, Spin, Scratch, Howltron, Gem Boutique, Diamond Deals, Goals, Rookie Gems, Storage and Settings. Dog selection, feeding, moving, coins and music playback remain visible.

## Save migration and deployment

- Save slot remains `my-singing-dogs-v1`. V1 and V2 saves can be migrated to V3, including old dogs, currencies, rare discoveries, incubators, castle jobs and achievements; new islands start locked in an older save.
- **Back up first** in game Settings → Export. Browser localStorage is specific to the exact website origin. A different GitHub repository URL is a different save location; use Export/Import to carry progress over.
- Files were repacked into a **single generated dog sprite atlas** with transparent character cutouts to remain within the **100-file ZIP limit**, without changing the appearance of already owned originals.
- Every musical island contains a multi-section 64-bar composition. Water and Rock use newly rendered individually mixed instrumental Ogg stems; on the three older islands, new added types temporarily reuse synchronized existing stem arrangements to preserve the original songs (these can be rerecorded in future releases).
- All art comes from generated images; some newly introduced character variations share the same generated source designs and are **not yet individually hand-animated**. This is a real limitation rather than claiming an entirely unique final sprite/animation for every new creature.
- The PWA caches the app shell and sprites offline; audio stems cache on demand when first played online. Five-island gameplay has been tested in Chromium, not physical iPad Safari or a live GitHub Pages deployment.

## Original version 2.1 systems still present

30 starter gems, V2 Rare Jinglepup odds (now extended to all seasonals), bakery times and gem speedups, castle-construction wait times, Rookie one-time early gem awards, wishing torches, normal Rares, Mythicals, Scratchpaw ticket exclusive, Luckypaw wheel exclusive, all prior seasonals, individual mute and volume, music playback, local autosave, backup import/export, a full collection, selling dogs, offline coin generation, coin vault and monuments, and song-based dog animations are retained.

## What was fixed from the iPad screenshots
- Currency counters and level bar have correctly sized backgrounds, with all icons, numbers, and XP meter positioned inside their frame.
- Square buttons use square generated textures and wide pills use wide generated textures; no giant whole-panel image is stretched into random aspect ratios.
- Five seasonal cards display clear art and readable dates and odds, with actual scrolling when content exceeds the window.
- Bakery, settings, breeding, dog details, Collection and Diamond Deals use clean text panes, decorative generated frames, and responsive spacing.
- Large modal windows scale for iPad landscape; mobile keeps two-column grids or scrolls vertically without sideways overflow.
- The in-game tutorial note no longer overlaps the quick-action dock.
- UI skins are embedded in style.css to maintain exactly 100 files; existing game code, songs, dog sprites, island environments and autosave format are untouched.

Before changing GitHub repositories or clearing Safari website data, export a backup in Options & Save Data. Replace the root files with this archive and wait for Pages redeploy. The service worker cache is versioned to load the updated design.
