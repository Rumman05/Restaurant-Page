# The Daily Grind - Coffee Shop Website

A modern, responsive coffee shop website built with vanilla JavaScript, HTML, and CSS using Webpack for module bundling and development.

## Live Demo

🌐 **[View Live Site](https://rumman05.github.io/Restaurant-Page/)**

## Features

- **Single Page Application (SPA)** - Dynamic tab-based navigation
- **Responsive Design** - Mobile-first approach that works on all devices
- **Modern UI/UX** - Inspired by contemporary coffee shop aesthetics
- **Modular Architecture** - Clean separation of concerns with ES6 modules
- **Interactive Elements** - Hover effects, smooth transitions, and functional CTA buttons

## Project Structure

```
coffee-shop-website/
├── src/
│   ├── images/
│   │   ├── hero-coffee.jpg
│   │   ├── coffee.png
│   │   ├── specialty-drinks.jpg
│   │   ├── cold-drinks.jpg
│   │   └── pastries.jpg
│   ├── about.js
│   ├── homepage.js
│   ├── menu.js
│   ├── script.js
│   ├── styles.css
│   └── template.html
├── dist/
├── node_modules/
├── .gitignore
├── package.json
├── webpack.config.js
└── README.md
```

## Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with Flexbox and Grid
- **JavaScript (ES6+)** - Modular programming with imports/exports
- **Webpack** - Module bundling and development server
- **Georgia Font** - Elegant serif typography

## Color Palette

The website uses a warm, coffee-inspired color scheme:
- **Dark Brown**: `#3d2914` (Headers, primary text)
- **Medium Brown**: `#5d4037` (Secondary text)
- **Gold Accent**: `#8b6914` (Highlights, decorative elements)
- **Tan**: `#d4b896` (Buttons, accents)
- **Cream**: `#f5f0e8` (Background)
- **White**: `#ffffff` (Cards, content areas)

## Pages

### Home Page
- Hero section with call-to-action
- Welcome message
- Featured menu items
- Hours and location information
- Customer testimonial

### Menu Page
- Coffee section
- Specialty drinks
- Cold beverages
- Pastries and snacks
- Each section includes images and detailed descriptions

### About Page
- Company story
- Mission statement
- What makes the shop special
- Location and hours

## Setup and Installation

1. **Clone the repository**
   ```bash
   git clone [your-repo-url]
   cd coffee-shop-website
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Add your images**
   Place your coffee shop images in the `src/images/` directory:
   - `hero-coffee.jpg` - Main hero image
   - `coffee.png` - Coffee section image
   - `specialty-drinks.jpg` - Specialty drinks image
   - `cold-drinks.jpg` - Cold beverages image
   - `pastries.jpg` - Pastries and snacks image

4. **Start development server**
   ```bash
   npx webpack serve
   ```

5. **Open your browser**
   Navigate to `http://localhost:8080`

## Build for Production

```bash
npx webpack
```

This creates optimized files in the `dist/` directory.

## Deployment

The project is configured for GitHub Pages deployment:

1. **Create gh-pages branch** (first time only)
   ```bash
   git branch gh-pages
   ```

2. **Deploy/redeploy**
   ```bash
   git checkout gh-pages && git merge main --no-edit
   npx webpack
   git add dist -f && git commit -m "Deployment commit"
   git subtree push --prefix dist origin gh-pages
   git checkout main
   ```

3. **Configure GitHub Pages**
   - Go to repository Settings
   - Set source branch to `gh-pages`

## Key Features Explained

### Modular JavaScript Architecture
- Each page is a separate module that exports a function
- Clean separation between content creation and event handling
- Reusable components and consistent structure

### Responsive Design
- Mobile-first CSS approach
- Flexible grid layouts that adapt to screen size
- Touch-friendly navigation and interactions

### Dynamic Content Loading
- All content is created dynamically with JavaScript
- No hardcoded HTML content (except navigation)
- Smooth page transitions with content replacement

### Image Optimization
- Webpack handles image processing and optimization
- Proper import statements for reliable asset loading
- Responsive images that scale appropriately

## Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile browsers (iOS Safari, Chrome Mobile)
- Requires ES6 support for modules
