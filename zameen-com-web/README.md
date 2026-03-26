# Zameen.com Web - Project Documentation

## Project Overview

This is a **static frontend web project** replicating the homepage of **Zameen.com**, Pakistan's leading real estate platform. The project is built with vanilla HTML, CSS, and Bootstrap 5, designed to showcase property search functionality and real estate listings.

### Purpose
- Display a property search interface for buying, renting, and exploring projects in Pakistan
- Provide quick access to real estate tools (loan calculator, area calculator, construction cost calculator)
- Showcase property categories: Homes, Plots, and Commercial properties
- Feature explore sections for new projects, area guides, and agencies

---

## Tech Stack

| Technology | Version | Purpose |
|------------|---------|---------|
| HTML5 | - | Structure |
| CSS3 | - | Custom styling |
| Bootstrap | 5.3.8 | Responsive grid & components |
| Font Awesome | 7.0.1 | Icons |
| Lato Font | - | Custom typography |

---

## Project Structure

```
zameen-com-web/
├── index.html              # Main HTML file
├── style.css               # Custom styles
├── README.md                 # Project documentation
└── assests/
    ├── fonts/
    │   └── Lato-Regular.ttf
    └── images/
        ├── agencies/       # Agency logos (agency-1.png to agency-8.png)
        ├── explore/        # Explore section icons (explore-1.svg to explore-8.svg)
        ├── hero/           # Hero section background (image.png)
        ├── nav/            # Navigation logo (logo.svg)
        ├── projects/       # Project images (project-1.png to project-3.png)
        └── topnav/         # Top nav icons (urdu.svg)
```

---

## Building and Running

### Quick Start
Since this is a static HTML/CSS project, simply open `index.html` in a browser:

```bash
# Option 1: Direct file open
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux

# Option 2: Using a local server (recommended for proper asset loading)
npx serve .
# or
python -m http.server 8000
# or
php -S localhost:8000
```

### Development Server Recommendations
- Use a local server to avoid CORS issues with font loading
- Bootstrap and Font Awesome are loaded via CDN (requires internet connection)

---

## Key Components

### 1. Top Navigation (`<div class="top-nav">`)
- Main navbar with links: Properties, Plot Finder, Area Guides, Blog, Maps
- Dropdown menus for Tools and More options
- Search bar for Property ID lookup
- Add Property button, Urdu language toggle, Settings, User profile

### 2. Secondary Navigation (`<div class="nav-bottom">`)
- Zameen logo
- Quick links: Buy (Home, Plots, Commercial), Rent, Agents, New Projects

### 3. Hero Section (`<div class="hero-section">`)
- Full-height search interface
- Property type tabs: Buy, Rent, Projects
- Search filters: City, Location, Property Type, Price Range, Area, Bedrooms
- Advanced options: Change Currency, Change Area Unit, Reset Search

### 4. Properties Section (`<div class="properties">`)
- Three property category cards: Homes, Plots, Commercial
- Sub-categories with popular filters (5 Marla, 10 Marla, etc.)

### 5. Explore Section (`<div class="explore-section">`)
- Feature cards: New Projects, Construction Cost Calculator, Home Loan Calculator, Area Guides, Plot Finder, Property Index

### 6. Agencies Section (`<div class="agencies-section">`)
- Display of top real estate agencies (8 agency logos)

### 7. Projects Section (`<div class="projects-section">`)
- Featured new development projects

---

## CSS Variables

```css
:root {
    --primary: #33A137;  /* Main brand green color */
}
```

---

## Responsive Breakpoints

| Breakpoint | Max Width | Behavior |
|------------|-----------|----------|
| Mobile | 400px | Right top nav hidden |
| Tablet | 992px | Navbar collapsed/hidden |

---

## Development Conventions

### Naming
- BEM-inspired class names (e.g., `.property-head`, `.sub-property`)
- Descriptive, semantic naming for sections

### Styling
- Bootstrap utility classes for spacing (`py-3`, `px-4`, `mb-2`)
- Custom CSS for brand-specific styling
- Flexbox for layouts

### Assets
- Images organized by section (agencies, explore, hero, nav, projects, topnav)
- Custom font (Lato) loaded via `@font-face`

---

## Known Notes

1. **Folder Spelling**: The assets folder is spelled `assests` (not `assets`) - this is consistent throughout the codebase
2. **CDN Dependencies**: Bootstrap and Font Awesome are loaded from CDN; internet connection required
3. **Font Loading**: Local Lato font may have CORS issues when opened via `file://` protocol

---

## Future Enhancements (Potential)

- Add JavaScript for interactive search functionality
- Implement property listing pages
- Add form validation for search filters
- Create individual agency and project detail pages
- Add lazy loading for images
- Implement service worker for offline support
