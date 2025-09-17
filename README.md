# Havala Hanson - Academic Website

A professional website for storing and displaying published reports, curriculum vitae, and academic documents with photos and detailed content.

## Overview

This repository contains a clean, responsive website designed for academics and researchers to showcase their work. The site includes:

- **Homepage**: Professional landing page with featured documents
- **Documents**: Organized repository of research papers and reports
- **CV**: Complete curriculum vitae with downloadable PDF option
- **About**: Personal background and research interests

## Features

- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Document Organization**: Easy-to-navigate structure for academic papers
- **Photo Integration**: Support for images, charts, and visualizations in documents
- **Professional Styling**: Clean, academic-appropriate design
- **SEO Friendly**: Proper HTML structure and meta tags
- **Fast Loading**: Optimized static HTML/CSS with minimal dependencies

## Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Havala-Hanson/havalawebsite.git
   cd havalawebsite
   ```

2. **Open in VS Code:**
   ```bash
   code .
   ```

3. **Preview locally:**
   - Install the "Live Server" extension in VS Code
   - Right-click on `index.html` and select "Open with Live Server"
   - Or simply open `index.html` in your web browser

4. **Customize content:**
   - Replace placeholder content with your actual information
   - Add your documents to the `documents/` folder
   - Update images in the `images/` folder
   - Modify styling in `css/styles.css` if desired

## File Structure

```
├── index.html              # Homepage
├── documents.html          # Document listing
├── cv.html                 # Curriculum vitae
├── about.html              # About page
├── css/
│   └── styles.css          # Main stylesheet
├── images/                 # Photos and graphics
├── documents/              # Individual document pages
├── BUILD.md                # Detailed build instructions
└── README.md               # This file
```

## Adding New Documents

1. Create a new HTML file in the `documents/` folder
2. Use existing documents as templates
3. Add images to the `images/` folder
4. Update `documents.html` to include the new document
5. Test and commit your changes

## Deployment

### GitHub Pages (Recommended)
1. Go to repository Settings > Pages
2. Select "Deploy from a branch" and choose "main"
3. Your site will be available at `https://havala-hanson.github.io/havalawebsite/`

### Other Options
- **Netlify**: Connect your GitHub repo for automatic deployments
- **Traditional hosting**: Upload files via FTP to any web host

## Customization

The website is designed to be easily customizable:

- **Colors**: Modify the CSS color variables
- **Fonts**: Change font families in the CSS
- **Layout**: Adjust grid layouts and spacing
- **Content**: Replace all placeholder text and images

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Contributing

This is a personal academic website. If you find bugs or have suggestions for improvements, please open an issue.

## Documentation

For detailed build and deployment instructions, see [BUILD.md](BUILD.md).

---

**Built with:** HTML5, CSS3, and modern web standards
**Designed for:** Academics, researchers, and professionals
