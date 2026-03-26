# Depot Web - Project Context

## Project Overview

**Depot** is a static frontend landing page for a transportation and logistics company. The site provides information about shipping services (truck, plane, sea freight) and includes a package tracking interface.

### Tech Stack

| Technology | Version | Purpose |
|------------|---------|---------|
| HTML5 | - | Semantic markup |
| CSS3 | - | Custom styling |
| Bootstrap | 5.3.8 | Responsive layout, components, utilities |
| Font Awesome | 7.0.1 | Icons |
| Raleway Font | - | Custom typography (local TTF) |

### Architecture

Single-page static website with no build process or backend dependencies. All resources load via CDN except local font and images.

## Building and Running

This is a **static website** - no build step required.

### To View Locally

**Option 1: Direct Open**
- Open `index.html` directly in any web browser

**Option 2: Local Server (Recommended)**
```bash
# Python
python -m http.server 8000

# Node.js (npx)
npx serve

# PHP
php -S localhost:8000
```
Then navigate to `http://localhost:8000`

### Testing
- Manual browser testing only
- No automated test suite configured

## File Structure

```
depot-web/
├── index.html              # Main HTML document
├── style.css               # Custom CSS styles
└── assests/                # Note: typo in folder name (should be "assets")
    ├── fonts/
    │   └── Raleway-Regular.ttf
    └── images/
        ├── hero.png        # Hero section background image
        ├── view-1.png      # Truck Insurance card image
        ├── view-2.png      # Plane Transportation card image
        └── view-3.png      # Sea & Ear Freight card image
```

## Page Sections

1. **Top Bar** (`#upperbar`) - Contact info and social links (hidden on mobile < 777px)
2. **Navbar** - Sticky navigation with brand "Depot" and 7 menu items
3. **Hero Section** - Full-viewport banner with tracking input field
4. **Views Section** - Three service cards with hover animations
5. **Services Section** - Additional services (incomplete)

## Development Conventions

### CSS Patterns
- Bootstrap utility classes preferred for layout (`d-flex`, `py-2`, `text-center`, `gap-4`)
- Custom styles in `style.css` for project-specific needs
- Mobile-first responsive design with breakpoint at `777px`
- CSS transitions for hover effects (`0.3s ease-in-out`)

### HTML Patterns
- Semantic HTML5 elements (`<nav>`, `<section>` implied via divs)
- Bootstrap grid and component classes
- Font Awesome icons via `<i>` tags with appropriate classes

### Styling Approach
```css
/* Gradient overlay pattern */
.hero-section::before {
    content: "";
    position: absolute;
    background: linear-gradient(45deg, #377aff, #00d9ff);
    opacity: 0.15;
}
```

## Known Issues / TODOs

1. **Folder name typo**: `assests` → should be `assets`
2. **Incomplete Services Section**: `.services-head` is empty, only one service card visible
3. **Missing content**: Navbar links (About Us, Why Us, Testimonials, Blog, Contact) have no corresponding sections
4. **Placeholder text**: Lorem ipsum throughout needs replacement with real content
5. **No JavaScript**: No custom JS file; tracking functionality not implemented

## Dependencies (CDN Links)

```html
<!-- Bootstrap CSS -->
https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css

<!-- Font Awesome -->
https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.0.1/css/all.min.css

<!-- Bootstrap JS Bundle -->
https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js
```

## Color Palette

| Color | Hex | Usage |
|-------|-----|-------|
| Primary Blue | `#377aff` | Gradient start, primary buttons |
| Cyan | `#00d9ff` | Gradient end |
| Light Gray | `#EEEEEE` | Top bar background |
| Text Gray | `#666666` | Top bar text, secondary text |
