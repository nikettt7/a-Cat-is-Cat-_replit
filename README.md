# A CAT IS CAT, BUT THE DOG IS MOUSE

A browser-based rule-manipulation puzzle game with a visual level designer. Rearrange word blocks to change how the world behaves, guide controlled characters to winning tiles, and create custom puzzles without writing code.

The project uses an original warm toy-box presentation and emoji-based artwork. It is inspired by rule-manipulation puzzle mechanics and does not include assets from *Baba Is You*.

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

```text
artifacts/cat-dog-mouse-puzzle: web
