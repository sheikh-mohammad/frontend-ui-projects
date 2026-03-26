# Frontend UI Projects

A collection of static frontend UI projects built with **HTML**, **CSS**, and **Bootstrap**. This directory contains multiple independent website templates and clones, each demonstrating different design patterns and layouts.

## Project Overview

This is a **non-code project** directory containing multiple standalone frontend web projects. Each subdirectory is a self-contained website built primarily with HTML5, CSS3, and Bootstrap 5. These projects serve as portfolio pieces, practice exercises, or template demonstrations.

### Technologies Used

- **HTML5** - Semantic markup and structure
- **CSS3** - Custom styling, animations, and responsive design
- **Bootstrap 5** - Responsive grid system and UI components (versions 5.3.7/5.3.8)
- **Font Awesome** - Icon library (versions 6.x/7.x)
- **Google Fonts** - Custom typography (Raleway, Roboto)

## Directory Structure

```
frontend-ui-projects/
├── chess-board/              # Interactive chess board UI
├── depot-web/                # Transportation & logistics website
├── google-no-internet-page/  # Chrome "No Internet" error page clone
├── mighty-web/               # Web design agency portfolio
├── periodic-table/           # Interactive periodic table of elements
├── petvet-web/               # Veterinary services website
├── roberto-web/              # Hotel & resort booking website
└── zameen-com-web/           # Real estate property portal clone
```

## Key Projects

### 1. Chess Board (`chess-board/`)
A static chess board layout built with HTML tables and CSS.
- **Files:** `index.html`, `images/` (piece images)
- **Features:** 8x8 grid with alternating colors, all chess pieces positioned

### 2. Depot Web (`depot-web/`)
Transportation and logistics company website template.
- **Files:** `index.html`, `style.css`, `assests/`
- **Features:** Hero section, service cards, navigation with Bootstrap, custom font (Raleway)
- **Dependencies:** Bootstrap 5.3.8, Font Awesome 7.0.1

### 3. Google No Internet Page (`google-no-internet-page/`)
A clone of Chrome's "No Internet" error page.
- **Files:** `index.html`, `img/`, `pages/details.html`
- **Features:** Error message layout, troubleshooting links

### 4. Mighty Web (`mighty-web/`)
Web design agency portfolio website.
- **Files:** `index.html`, `style.css`, `assets/`
- **Features:** Hero section, about section with skill progress bars, services grid, work gallery
- **Dependencies:** Bootstrap 5.3.7, Font Awesome 7.0.0

### 5. Periodic Table (`periodic-table/`)
Interactive periodic table of chemical elements.
- **Files:** `index.html`, `style.css`, `README.md`
- **Features:** Full periodic table layout with element groups color-coded, lanthanides/actinides
- **Live Demo:** https://sheikh-mohammad.github.io/Periodic-Table/

### 6. PetVet Web (`petvet-web/`)
Veterinary services and pet care website.
- **Files:** `index.html`, `style.css`, `README.md`, `assets/`
- **Features:** Hero section, services cards, groomers gallery, testimonials carousel, pricing plans, appointment form
- **Dependencies:** Bootstrap 5.3.8, Font Awesome 7.0.1, Google Fonts (Roboto)
- **Live Demo:** https://final-petvet.netlify.app/

### 7. Roberto Web (`roberto-web/`)
Hotel and resort booking website template.
- **Files:** `index.html`, `style.css`, `assets/`
- **Features:** Carousel hero, booking form, room listings, testimonials, blog section, contact section
- **Dependencies:** Bootstrap 5.3.8, Font Awesome 7.0.1

### 8. Zameen.com Web (`zameen-com-web/`)
Real estate property portal clone (Pakistan property website).
- **Files:** `index.html`, `style.css`, `assests/`
- **Features:** Property search with filters, property type cards, explore section, advanced search options
- **Dependencies:** Bootstrap 5.3.8, Font Awesome 7.0.1

## Usage

### Viewing a Project

1. Navigate to the desired project folder:
   ```bash
   cd frontend-ui-projects/<project-name>
   ```

2. Open `index.html` in a web browser:
   - Double-click the file in your file explorer
   - Or use a local development server:
     ```bash
     # Python
     python -m http.server 8000
     
     # Node.js
     npx serve
     npx live-server
     ```

### Development

Each project is self-contained. To modify a project:

1. Edit HTML files for structure changes
2. Edit CSS files for styling changes
3. Replace images in the respective `assets/` or `images/` folders

## Common Patterns

### Bootstrap Usage
All projects use Bootstrap 5 via CDN with similar patterns:
```html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.x/dist/css/bootstrap.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.x/dist/js/bootstrap.bundle.min.js"></script>
```

### Font Awesome Integration
```html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.0.x/css/all.min.css">
```

### Responsive Design
- Mobile-first approach using Bootstrap's grid system
- Custom media queries in project-specific CSS files
- Flexbox utilities for layout

## Color Schemes (Project-Specific)

| Project | Primary Color | Secondary Color |
|---------|---------------|-----------------|
| depot-web | #377aff (Blue) | #00d9ff (Cyan) |
| petvet-web | #FD4C82 (Pink) | #91c235 (Green) |
| zameen-com-web | #00a651 (Green) | #7ED8AA (Mint) |

## Notes

- All projects are **static websites** with no backend functionality
- Images and assets are stored locally in each project's folder
- Some projects have README files with additional documentation
- Projects may use placeholder content (Lorem ipsum text)
- Font Awesome 7.x is used via CDN (note: this is a newer version)

## Contributing

This is a portfolio/practice project collection. For modifications:
1. Keep changes within the respective project folder
2. Maintain existing file structure
3. Preserve Bootstrap and Font Awesome CDN links
4. Test responsiveness after CSS changes
