# Stellar Dominion

A **real-time sci-fi grand strategy game in 3D** that runs entirely offline in a web browser. There is no install, no internet and no account. The whole game is one file, `index.html`.

Build an interstellar empire across a galaxy of star systems linked by hyperlanes. Colonise worlds, construct buildings, research technology, design fleets around ship counters, and deal with AI empires that make war, sue for peace and form alliances. All of this happens continuously in real time, and you can pause or speed it up whenever you like.

## Playing offline (e.g. on a plane)

**Laptop (Windows / Mac / Linux):** download `index.html` and double-click it. It opens in your browser and works with no connection.

**Phone or tablet:** phones don't run games from a downloaded HTML file very well, so install it as an app while you still have internet:
1. Put the game online once (free):
   - **Netlify Drop (easiest):** on a laptop go to https://app.netlify.com/drop and drag in the files `index.html`, `sw.js`, `manifest.webmanifest`, `icon.svg`, `icon-180.png`, `icon-192.png`, `icon-512.png` (or the `stellar-dominion-app.zip`). You get an `https://….netlify.app` address. Make a free account to keep it permanently.
   - **GitHub Pages:** only free for public repos. Settings → Pages → deploy from branch, root folder.
2. Open that address on your phone.
   - **iPhone/iPad (Safari):** Share → *Add to Home Screen*.
   - **Android (Chrome):** ⋮ menu → *Install app* / *Add to Home screen*.
3. Launch it once from the home screen while online. It is then cached and runs fully offline.

Saves are stored in the browser on each device. Saves from earlier versions of the game are converted automatically when loaded. To move a game between devices, use **☰ → Export save** and **Import save**.

## Features

- **The real solar neighbourhood:** up to 125 real stars at their true distance from Sol, with their real spectral types. Real exoplanets are included (Proxima b, the TRAPPIST-1 system, Tau Ceti e/f, Teegarden b, Ross 128 b…), and the Solar System has all eight planets. You start on Earth.
- **Full 3D with a free camera:** the stars sit at their true 3D positions, with drop-lines to the galactic plane and distance rings around Sol. Rotate, tilt, zoom and pan anywhere, or use the view presets (top-down, angled, side-on, auto-orbit, focus on selection).
- **Three zoom levels:** the local stars, then star systems with orbiting planets where battles play out ship by ship, then planets as lit globes. Earth has real continents, clouds and city lights.
- **Cyberpunk ships:** long, angular, faceted 3D hulls with neon edge lighting and engine glow. Humans fly gunmetal blades with cyan trim; aliens fly crystalline, forked hulls in their empire colours.
- **Physical damage:** ships are built from parts. Wings, armour plates, turrets, bridges and engines are torn off and tumble away as debris; hits leave glowing gashes; hulls scorch and glow red-hot; neon lights flicker and die with the crew. Destroyed ships break apart, and dead hulks drift.
- **Damage without health bars:** weapons have damage and armour penetration. Autocannons barely scratch heavy armour. Missiles and torpedoes breach hulls, so ships vent air, catch fire, lose crew and suffer engine or weapon damage, and can die slowly if damage control can't keep up. Ships report conditions like "3 hull breaches: venting atmosphere · Air 41% · Crew 212/750".
- **Ground war:** destroy a world's orbital defences, then land Troop Transports. You watch soldiers fight the garrison on the surface.
- **Economy:** energy, minerals and research. Buildings need workers, other planets in a system can host outposts, and fleet capacity limits your navy. Storage silos cap stockpiles (2,000 + 300 per system), so surpluses should be spent on **major projects** (Terraform, Orbital Habitat, Starbase, Naval Yards) or traded on the galactic market.
- **Tech tree:** 27 technologies that get pricier the more you know, plus endless repeatable research for the late game. **Diplomacy:** war, peace, defensive alliances, opinion and gifts. **AI rivals:** 1–7 alien empires with personalities, on 4 difficulty levels.
- **Real time:** pause and 1×/2×/4×/8× speed. Autosave, 3 save slots, and export/import of save files. Touch and mouse controls.

## Controls

| Action | Touch | Mouse / keyboard |
|---|---|---|
| Rotate / tilt the camera | one-finger drag | left-drag |
| Zoom / pan | pinch / two-finger drag | wheel / right-drag |
| View presets | ⤒ top · ◢ angled · ▭ side · ⟳ orbit · ◎ focus · ⟲/✋ drag mode | V cycles · O orbit · F focus · R drag mode |
| Select system, planet or fleet | tap | click |
| Enter a star system / land on a planet | double-tap (or zoom in) | double-click (or zoom in) |
| Move selected fleet | tap a star, planet or hyperlane exit | click or right-click |
| Pause / speed | top bar | Space, 1–4 |
| Tech / Diplomacy / Empire | top bar | T / D / E |
| Centre on capital | ⌂ | H |
| Deselect / menu | ✕ | Esc |

**Win** by destroying every rival or controlling 60% of the galaxy. You **lose** when your last system falls.


Built with [three.js](https://threejs.org) r147 (MIT licence), embedded in `index.html` so the game works offline.
