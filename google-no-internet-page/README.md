# Google No Internet Page - Project Context

## Project Overview

This is a **static HTML/CSS frontend project** that recreates Google Chrome's "No Internet" error page (ERR_NAME_NOT_RESOLVED). The project simulates the classic Chrome browser error screen that appears when a website's DNS cannot be resolved.

**Purpose:** A UI clone/replica of Chrome's offline error page for educational or demonstration purposes.

## Project Structure

```
google-no-internet-page/
├── index.html              # Main error page ("This site can't be reached")
├── pages/
│   └── details.html        # Expanded details view with troubleshooting steps
├── img/
│   └── sad.png             # Sad tab icon (Chrome's dinosaur alternative)
└── README.md               # This file
```

## Key Files

| File | Description |
|------|-------------|
| `index.html` | Primary error page showing the basic "No Internet" message with quick action links (Reload, Details) |
| `pages/details.html` | Detailed troubleshooting page with expanded network diagnostic suggestions |
| `img/sad.png` | Sad face icon displayed on the error pages |

## Technologies Used

- **HTML5** - Semantic markup structure
- **Inline CSS** - Basic styling via HTML attributes (center, tables, br spacing)
- **Static Assets** - PNG image for the sad icon

## Building and Running

This is a **purely static project** with no build process required.

### To View the Project

1. Open `index.html` directly in any web browser
2. Or serve it locally:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (npx)
   npx serve
   
   # Using PHP
   php -S localhost:8000
   ```
3. Navigate to `http://localhost:8000` in your browser

## Development Notes

### Current Implementation Details

- Uses `<center>` tag (deprecated HTML) for centering content
- Uses `<table>` elements for layout (older HTML practice)
- No external CSS or JavaScript files
- No build tools, package managers, or dependencies
- Links in `index.html` reference `pages/connectionCheck.html` which does not exist in the current structure

### Potential Improvements

- Replace deprecated `<center>` with CSS flexbox/grid
- Replace table-based layout with modern CSS
- Add responsive design for mobile devices
- Create missing `connectionCheck.html` page referenced in links
- Add CSS for better visual styling
- Fix typo: "Checikng" → "Checking" (appears in both HTML files)

## Testing Practices

No automated testing framework is configured. Testing is done manually by:
1. Opening the HTML files in a browser
2. Verifying visual appearance matches Chrome's error page
3. Testing link navigation between pages

## Browser Compatibility

Works in all modern browsers that support HTML5. Best experienced in Google Chrome for authentic replication.
