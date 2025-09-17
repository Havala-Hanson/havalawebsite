# Building and Deploying from VS Code

This document provides instructions for building and deploying the Havala website from VS Code.

## Prerequisites

- VS Code installed on your computer
- Git configured and connected to GitHub
- Basic understanding of HTML/CSS
- Web browser for testing

## Development Workflow

### 1. Clone and Setup

```bash
# Clone the repository
git clone https://github.com/Havala-Hanson/havalawebsite.git
cd havalawebsite

# Open in VS Code
code .
```

### 2. Local Development

The website is built with static HTML/CSS files and can be developed locally without any build tools.

**To preview your changes:**

1. Open `index.html` in your web browser, or
2. Use VS Code's "Live Server" extension for auto-refresh during development:
   - Install the "Live Server" extension in VS Code
   - Right-click on `index.html` and select "Open with Live Server"
   - Your browser will open the site and auto-refresh when you make changes

### 3. Adding New Documents

To add a new document to the website:

1. **Create the document HTML file:**
   - Navigate to the `documents/` folder
   - Create a new HTML file (e.g., `my-new-document.html`)
   - Use the existing documents as templates
   - Include proper navigation and styling

2. **Add images (if needed):**
   - Place images in the `images/` folder
   - Use JPG, PNG, or SVG formats
   - Optimize images for web (recommend < 1MB file size)

3. **Update the documents listing:**
   - Edit `documents.html`
   - Add a new `document-item` div with your document information
   - Include title, description, publication date, and link

4. **Test your changes:**
   - Preview the document page
   - Check that navigation works properly
   - Verify images load correctly

### 4. Customizing Content

**Update personal information:**
- Edit `cv.html` with your actual CV information
- Update `about.html` with your bio and research interests
- Replace placeholder images in `images/` folder with actual photos

**Modify styling:**
- Edit `css/styles.css` to change colors, fonts, or layout
- The CSS is organized in sections for easy customization
- Test changes across different screen sizes

### 5. Git Workflow from VS Code

**Making changes:**
1. Edit files in VS Code
2. Save your changes (Ctrl+S / Cmd+S)
3. Use VS Code's Source Control panel (Ctrl+Shift+G / Cmd+Shift+G)
4. Stage changes by clicking the "+" next to files
5. Write a commit message and commit (Ctrl+Enter / Cmd+Enter)
6. Push to GitHub using the sync button

**Alternative command line workflow:**
```bash
# Stage all changes
git add .

# Commit with message
git commit -m "Add new research document"

# Push to GitHub
git push origin main
```

## Deployment Options

### Option 1: GitHub Pages (Recommended)

1. Go to your repository on GitHub
2. Navigate to Settings > Pages
3. Select "Deploy from a branch"
4. Choose "main" branch and "/ (root)" folder
5. Save - your site will be available at `https://havala-hanson.github.io/havalawebsite/`

### Option 2: Netlify

1. Create account at netlify.com
2. Connect your GitHub repository
3. Deploy with default settings
4. Get custom domain at `your-site-name.netlify.app`

### Option 3: Traditional Web Hosting

1. Download all files from your repository
2. Upload via FTP to your web hosting provider
3. Ensure `index.html` is in the root directory

## File Structure

```
havalawebsite/
├── index.html              # Main homepage
├── documents.html          # Document listing page
├── cv.html                 # CV page
├── about.html              # About page
├── css/
│   └── styles.css          # Main stylesheet
├── images/                 # Image files
│   ├── placeholder-*.jpg   # Placeholder images (replace these)
│   └── profile-photo.jpg   # Your profile photo
├── documents/              # Individual document pages
│   ├── sample-report.html
│   └── sample-publication.html
├── README.md               # Project documentation
├── LICENSE                 # MIT License
└── .gitignore             # Git ignore rules
```

## Tips for VS Code Development

**Useful Extensions:**
- Live Server: Auto-refresh browser during development
- HTML CSS Support: Enhanced HTML/CSS editing
- Prettier: Code formatting
- GitLens: Enhanced Git integration

**Keyboard Shortcuts:**
- `Ctrl/Cmd + Shift + P`: Command palette
- `Ctrl/Cmd + \``: Toggle terminal
- `Ctrl/Cmd + B`: Toggle sidebar
- `F12`: Go to definition (for CSS classes)

## Troubleshooting

**Images not loading:**
- Check file paths are correct (use relative paths)
- Ensure image files are in the `images/` folder
- Verify file extensions match (case-sensitive on some servers)

**CSS not applying:**
- Check the CSS file path in HTML `<link>` tags
- Clear browser cache (Ctrl+F5 / Cmd+Shift+R)
- Verify CSS syntax is correct

**Links not working:**
- Use relative paths (e.g., `documents.html`, not `/documents.html`)
- Check file names match exactly (case-sensitive)

## Adding Interactive Features

While this is a static website, you can enhance it with:

**Simple JavaScript additions:**
- Contact forms (using Formspree or Netlify Forms)
- Search functionality for documents
- Dynamic content loading

**Third-party integrations:**
- Google Analytics for tracking
- Disqus for comments
- Social media sharing buttons

## Maintenance

**Regular updates:**
- Add new documents as they're published
- Update CV with new positions/achievements
- Refresh images and content periodically
- Check all links are working

**Performance optimization:**
- Compress images before uploading
- Minify CSS for production (optional)
- Monitor page load speeds