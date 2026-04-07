# Periodic Table Project

## Project Overview

A static HTML/CSS web application that displays **The Periodic Table of Elements**. This is a frontend-only UI project that renders all 118 chemical elements in their traditional periodic table layout, including the lanthanide and actinide series.

### Technologies
- **HTML5** - Semantic structure using tables for element grid layout
- **CSS3** - Styling with color-coded element categories and responsive design

### Features
- Complete periodic table with all 118 elements (H to Og)
- Color-coded element categories (alkali metals, noble gases, transition metals, etc.)
- Two-table layout: main table + separate lanthanide/actinide rows
- Responsive design for mobile devices (breakpoint at 546px)
- Element cells display atomic number and symbol

## Project Structure

```
periodic-table/
├── index.html      # Main HTML file with periodic table structure
├── style.css       # All styling and responsive rules
└── README.md       # This file
```

## Building and Running

This is a **static website** with no build process required.

### To Run Locally

1. **Direct file open**: Open `index.html` in any web browser
   ```
   # Windows
   start index.html
   
   # Or drag-drop index.html into browser
   ```

2. **Using a local server** (recommended for proper testing):
   ```
   # Python 3
   python -m http.server 8000
   
   # Node.js (if npx available)
   npx serve .
   
   # Then open http://localhost:8000
   ```

## Development Conventions

### Code Style
- **HTML**: Inline styles used sparingly for layout (colspan/rowspan for grid gaps)
- **CSS**: 
  - Class-based styling for element categories (`.orange`, `.pink`, `.yellow`, etc.)
  - Utility classes for text colors (`.black`, `.blue`, `.dark`)
  - Global reset on `*` selector
  - Centered layout using `text-align: center` on container

### Element Color Categories
| Class | Purpose |
|-------|---------|
| `.orange` | Nonmetals (H, N, O, C, P, S, Se) |
| `.pink` | Alkali metals (Li, Na, K, Rb, Cs, Fr) |
| `.sky` | Alkaline earth metals (Be, Mg, Ca, Sr, Ba, Ra) |
| `.yellow` | Transition metals |
| `.brown` | Metalloids (B, Si, Ge, As, Sb, Te, Po) |
| `.peach` | Halogens (F, Cl, Br, I, At) |
| `.grey` | Noble gases |
| `.green` | Post-transition metals |
| `.chocolate` | Lanthanides & Actinides |

### Responsive Design
- Breakpoint: `546px` max-width
- Tables scale down to `10%` width on mobile
- Heading font-size reduces from `500%` to `200%`

## Known Limitations

- No interactive element details (hover states, click handlers)
- No element names or atomic weights displayed
- Lanthanum (57-71) and Actinium (89-103) placeholders in main table
- Font hardcoded to 'Arial'
- Some typos in element symbols (e.g., "TI" instead of "Tl" for Thallium)

## Potential Enhancements

- Add tooltips with full element information
- Implement click/hover interactions
- Add element categories legend
- Include atomic weights and names
- Fix Thallium symbol (TI → Tl)
- Add search/filter functionality
- Expand to include element properties data
