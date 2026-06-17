# Built To Order Bots

A single-file browser game where you build a monster, arm it with weapons and enhancements, and send it to fight across multiple battlefields and game modes.

Open `BuiltToOrderBots.html` directly in any modern browser - no build step, no server, no dependencies beyond a single Tailwind CDN script.

## Play

```
open BuiltToOrderBots.html
```

Or just double-click the file.

## Controls

| Action | Keyboard | Touch |
|---|---|---|
| Move | Arrow keys / WASD | on-screen ◀ ▶ |
| Jump | Up / W / Space (double-jump with Wings enhancement) | ▲ |
| Shoot | Space / click / tap | red ● button |
| Pause | Esc | - |

## What's in the game

- **12 monster types**: Tyro, Hominid, Arachnid, Worm, Wasp, Golem, Imp, Beast, Drakon, Specter, Brute, Sprite
- **11 weapons**: Rifle, Laser Gun, Flamethrower, Sword, Bow, Cannon, Crossbow, Plasma Rifle, Shotgun, Tesla Coil, Plasma Blade
- **11 enhancements**: Tentacles, Sting, Fiery Breath, Shell, Wings, Camouflage, Horns, Quills, Acid Spit, Berserk, Regeneration
- **3 battlefields**: Desert, Jungle, Swamp (with parallax backgrounds and platform layouts)
- **3 game modes**: Destruction, Flag Capture, The Horde
- **3 difficulty levels**: Beginner (prebuilt), Intermediate (build + fight), Tournament (career mode with corrals, healing, recruiting, localStorage save)

## Architecture

- Single self-contained HTML file
- Tailwind via CDN for UI
- Canvas 2D for the battle scene
- All game state, monsters, weapons, enhancements, and AI in vanilla JS
- 16-bit pixel-art sprites drawn procedurally per monster type
- Tournament save persists in `localStorage`

## Development

There is no build process. Edit the file, refresh the browser.

For local serving (optional):

```
python3 -m http.server 8000
# then open http://localhost:8000/BuiltToOrderBots.html
```

## License

Personal project - license TBD.
