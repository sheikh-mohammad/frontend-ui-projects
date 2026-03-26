# Mighty Web - Project Context

## Project Overview

**Mighty** is a static single-page website for a web design agency. The site showcases the agency's services, portfolio, and expertise in web technologies.

### Technologies Used

- **HTML5** - Semantic markup structure
- **CSS3** - Custom styling with `style.css`
- **Bootstrap 5.3.7** - Responsive grid system and UI components (via CDN)
- **Font Awesome 7.0.0** - Icon library (via CDN)
- **Mulish Font** - Google Font for typography

### Project Structure

```
mighty-web/
├── index.html          # Main HTML file with all page sections
├── style.css           # Custom CSS styles
├── README.md           # This file
└── assets/
    └── images/
        ├── hero.png        # Hero section background image
        ├── about.png       # About section image
        ├── work-1.png      # Portfolio item 1
        ├── work-2.png      # Portfolio item 2
        ├── work-3.png      # Portfolio item 3
        ├── work-4.png      # Portfolio item 4
        ├── work-5.png      # Portfolio item 5
        └── work-6.png      # Portfolio item 6
```

### Page Sections

1. **Header/Hero** - Full-viewport hero section with navigation and call-to-action
2. **About** - Company description with skills progress bars (Writing, WordPress, Bootstrap, jQuery)
3. **Services** - Four service cards (Web Design, Graphic Design, Web Apps, Ecommerce)
4. **Works** - Portfolio grid with 6 project thumbnails

## Building and Running

This is a static website with no build process required.

### Running Locally

1. **Direct File Open** - Open `index.html` directly in a web browser
2. **Local Server** (recommended for proper asset loading):
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (npx)
   npx serve
   
   # Using PHP
   php -S localhost:8000
   ```
3. Access at `http://localhost:8000` (or the port specified)

### Dependencies

All dependencies are loaded via CDN:
- Bootstrap 5.3.7 (CSS + JS bundle)
- Font Awesome 7.0.0
- Mulish font (Google Fonts)

No local package installation is required.

## Development Conventions

### Code Style

- **HTML**: Bootstrap utility classes combined with custom CSS classes
- **CSS**: 
  - Import statement at top for Google Fonts
  - Grouped selectors by section (header, about, services, works)
  - Consistent use of Bootstrap spacing utilities (`mt-`, `mb-`, `py-`, `px-`)
- **Color Scheme**:
  - Primary accent: `#01D28E` (green)
  - Backgrounds: White, `#F6F5F5` (light gray)
  - Text: Black/Dark gray

### Design Patterns

- **Responsive**: Bootstrap grid system (`col-lg-4`, `col-12`, etc.)
- **Components**: Offcanvas mobile menu, progress bars, cards
- **Effects**: Hover transitions on service cards, custom selection colors

### Image Assets

All images are stored in `assets/images/` and referenced with relative paths. The project uses:
- 1 hero background image
- 1 about section image
- 6 portfolio work images

## Notes

- No JavaScript framework or build tools are used
- The site is fully static and can be deployed to any static hosting service
- Bootstrap 5.3.7 is referenced via CDN (ensure internet connection for styles to load)
