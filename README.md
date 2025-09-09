# Reg - Static Website Template

A simplified HTML template deployed to GitHub Pages with automated CI/CD.

## Overview

This repository contains a static website template that has been simplified to remove animations and JavaScript while maintaining clean, professional design. The site is automatically deployed to GitHub Pages using GitHub Actions.

## Features

- 📱 Responsive design that works on all devices
- 🎨 Clean, modern styling with CSS gradients and shadows
- ⚡ Fast loading - no JavaScript dependencies
- 🚀 Automated deployment to GitHub Pages
- ♿ Accessible design with proper focus states
- 🎯 SEO-friendly structure

## Project Structure

```
reg/
├── index.html          # Main HTML file
├── styles.css          # CSS styling
├── .github/
│   └── workflows/
│       └── deploy.yml  # GitHub Actions workflow
├── .gitignore         # Git ignore file
└── README.md          # This file
```

## Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/head-org-il/reg.git
   cd reg
   ```

2. Open `index.html` in your browser or serve it with a local server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   ```

3. Visit `http://localhost:8000` to view the site

## Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to the `main` branch. The deployment process:

1. GitHub Actions workflow is triggered on push to `main`
2. Static files are built and prepared
3. Site is deployed to GitHub Pages
4. Available at: `https://head-org-il.github.io/reg/`

## Customization

### Replacing with Canva Template Content

To replace the placeholder content with your actual Canva template:

1. Export your Canva design as HTML
2. Copy the HTML content and replace the content in `index.html`
3. Copy any CSS and modify `styles.css` to remove animations and JavaScript
4. Remove any `<script>` tags and animation-related CSS
5. Test locally and push to deploy

### Modifying Styles

- Edit `styles.css` to customize colors, fonts, and layout
- The current design uses:
  - Color scheme: Purple/pink gradients (`#667eea`, `#764ba2`, `#f093fb`, `#f5576c`)
  - Font: Arial (can be changed to any web-safe font)
  - Responsive breakpoint: 768px for mobile

### Adding Content

- Add new sections to `index.html`
- Update navigation links in the header
- Modify the hero section, about, services, and contact sections as needed

## Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers

## Performance

- No JavaScript = faster loading
- Optimized CSS with efficient selectors
- Responsive images ready (add your images to an `images/` folder)
- Minimal HTTP requests

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Make your changes
4. Test locally
5. Commit and push: `git commit -m "Description" && git push`
6. Create a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).