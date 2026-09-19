# A CAT IS CAT, BUT THE DOG IS MOUSE

A browser-based rule-manipulation puzzle game with a visual level designer. Rearrange word blocks to change how the world behaves, guide controlled characters to winning tiles.

https://cat-dog-mouse-puzzle.replit.app/

Also include a custom level designer compatible with the game.

The project uses an original warm toy-box presentation and emoji-based artwork. It is inspired by rule-manipulation puzzle mechanics and it lets you bend the rules of physics to win.

## Features

### Puzzle game

- Three chapters with custom playable levels
- Horizontal and vertical rule detection
- Preset rules and movable word-block rules
- Immediate transformations such as `DOG IS MOUSE`
- `YOU`, `WIN`, `STOP`, `PUSH`, `DEFEAT`, `SINK`, `HOT`, and `MELT`
- Multiple controllable entities
- Undo, restart, move counter, and star ratings
- Keyboard and touch controls
- Level import, export, editing, deletion, and reordering
- Browser persistence using `localStorage`

### Level designer

- Visual tile palette with characters, objects, nouns, and properties
- Place and erase tools with click-and-drag support
- Adjustable grids from 5×5 to 20×20
- Level name, chapter hint, and preset-rule editing
- Live rule chips, tile information, and grid statistics
- JSON export compatible with the game
- Built-in help guide

## Project outputs

The main web app provides a launcher for both tools and download links for the standalone files.

- `artifacts/cat-dog-mouse-puzzle/public/game.html` — self-contained playable game
- `artifacts/cat-dog-mouse-puzzle/public/level-designer.html` — self-contained visual level editor

Both HTML files use inline CSS and JavaScript and can be opened independently in a browser. Google Fonts are the only external resources.

## Controls

| Action | Keyboard |
| --- | --- |
| Move up | `W` or `Arrow Up` |
| Move down | `S` or `Arrow Down` |
| Move left | `A` or `Arrow Left` |
| Move right | `D` or `Arrow Right` |
| Undo | `Z` |
| Restart level | `R` |

On phones and tablets, use the on-screen directional controls.

## Creating and importing a level

1. Open the Level Designer.
2. Choose a grid size and enter a level name.
3. Select tiles from the palette and place them on the grid.
4. Add any always-active rules, one rule per line.
5. Select **Export JSON**.
6. Open the game and select **Manage Levels** or **Import Level JSON**.
7. Import the exported JSON file.

Imported levels are normalized automatically from the designer's object-based cell format to the game's string-based cell format.
## Run locally on Replit
Start or restart the managed workflow:

artifacts/cat-dog-mouse-puzzle: web

The workflow runs:

pnpm --filter @workspace/cat-dog-mouse-puzzle run dev

Useful checks:

pnpm --filter @workspace/cat-dog-mouse-puzzle run typecheck
pnpm --filter @workspace/cat-dog-mouse-puzzle run build

Project structure
artifacts/cat-dog-mouse-puzzle/
├── public/
│   ├── game.html
│   └── level-designer.html
├── src/
│   ├── App.tsx
│   ├── index.css
│   └── main.tsx
├── package.json
└── vite.config.ts

Data and privacy
Custom chapters, levels, and edits are stored locally in the browser with localStorage. The game does not require an account or send level data to a server. Export important custom levels as JSON if you want a portable backup.

Educational use
This project was created for educational and non-commercial use. Use original artwork, audio, names, and other assets if you extend or distribute it.

https://cat-dog-mouse-puzzle.replit.app/
