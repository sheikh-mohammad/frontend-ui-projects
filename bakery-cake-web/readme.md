# SweetCake

A modern, responsive landing page for a cake and bakery brand, built using HTML and CSS. The project demonstrates clean UI design, responsive layouts, and organized asset management.

### Live Demo
Check out the live version here:
👉 [SweetCake Live Demo](https://bakery-cake-website.netlify.app/)

### Features
- Responsive Layout — adapts to mobile, tablet, and desktop screens
- Navigation Bar — Home, About, Shop, Pages, Blog, Contact
- Hero Section — bold introduction with call-to-action
- About Section — progress bars for skills/metrics
- Categories Showcase — circular tiles: Cupcake, Butter, Red Velvet, Biscuit, Donut
- Featured Dishes — product grid with prices and hover “Add to cart”
- Order Section — styled form and promotional banner
- Team Members — cards with hover social links
- Testimonials — client quotes with star ratings
- Instagram Gallery — image grid and handle
- Map + Address — embedded Google Map with details
- Footer with Newsletter — links and subscription form

### Technology Stack
- HTML5 → semantic page structure
- CSS3 → layout, styling, responsive design
- Font Awesome → icons via CDN
- Custom Fonts → Montserrat, Playfair Display

### File Structure
Assignment-11-CSS/ <br />
├── assets/ <br />
│   ├── fonts/ <br />
│   │   ├── Montserrat-Regular.ttf <br />
│   │   └── PlayfairDisplay-Regular.ttf <br />
│   └── imgs/ <br />
│       ├── dishes/ <br />
│       ├── footer/ <br />
│       ├── items/ <br />
│       ├── logos/ <br />
│       ├── order/ <br />
│       ├── pics/ <br />
│       ├── team/ <br />
│       └── testimonial/ <br />
├── index.html # Main HTML file  <br />
├── style.css # Styling and responsive layout <br />
└── README.md # Project documentation

### How to View
Clone the repository

```bash
git clone https://github.com/sheikh-mohammad/frontend-ui-projects/bakery-cake-web.git
cd bakery-cake-web
```

Open index.html in your browser to preview the website.

### Customization
- Replace images in assets/imgs/ with your own visuals
- Update text content in index.html
- Adjust fonts, colors, and layout via style.css

### Contributing
Contributions are welcome!

Fork the repository
Create a new branch (git checkout -b feature-name)
Commit your changes
Open a Pull Request with a clear description
Optional `docs/` deployment layout:
```bash
mkdir -p docs
mv index.html style.css assets docs/
git add . && git commit -m "chore: move site to docs for Pages"
git push
```