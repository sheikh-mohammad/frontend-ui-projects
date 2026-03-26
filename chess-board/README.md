# Chess Board - Project Context

## Project Overview

A **static HTML chess board** visualization. This is a simple frontend project that renders a standard 8x8 chess board with all pieces in their initial positions using plain HTML tables and image assets.

### Key Characteristics
- **Type**: Static HTML page (no JavaScript or CSS)
- **Board Size**: 600x600 pixels (8x8 grid, 75px per square)
- **Color Scheme**: White and green (#769656) squares
- **Assets**: PNG images for all chess pieces (white and black sets)

## Directory Structure

```
chess-board/
├── index.html          # Main HTML file with complete board layout
├── README.md           # This file
└── images/
    ├── black/          # Black piece images
    │   ├── bishop.png
    │   ├── king.png
    │   ├── knight.png
    │   ├── pawn.png
    │   ├── queen.png
    │   └── rook.png
    └── white/          # White piece images
        ├── bishop.png
        ├── king.png
        ├── knight.png
        ├── pawn.png
        ├── queen.png
        └── rook.png
```

## Running the Project

No build process required. Simply open `index.html` in a web browser:

```bash
# Windows
start index.html

# Or drag-and-drop the file into any browser
```

## Current Implementation Details

### Board Layout
- Uses HTML `<table>` with 8 rows and 8 columns
- Squares alternate between `white` and `#769656` (green) colors
- Each cell is 75x75 pixels (table is 600x600 total)
- Pieces are 40x40 pixels, centered in each square

### Initial Position
- **Rows 1-2**: Black pieces (rooks, knights, bishops, queen, king, pawns)
- **Rows 3-6**: Empty squares
- **Rows 7-8**: White pieces (pawns, rooks, knights, bishops, queen, king)

## Development Notes

### Current Limitations
- ❌ No interactivity (cannot move pieces)
- ❌ No CSS styling (inline attributes only)
- ❌ No JavaScript logic
- ❌ Uses deprecated `<center>` tag
- ❌ No responsive design

### Suggested Improvements
1. **Add CSS**: Extract styles to a separate stylesheet
2. **Add JavaScript**: Implement piece movement, drag-and-drop, game logic
3. **Modernize HTML**: Replace deprecated tags with CSS flexbox/grid
4. **Add Responsiveness**: Make board scale with viewport
5. **Game Features**: Add move validation, check/checkmate detection, game history

## Technologies Used

- HTML5
- PNG images for chess pieces
