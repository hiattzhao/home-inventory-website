# Home Inventory Manager Website

Static website for downloading Home Inventory Manager application.

## Structure

```
home-inventory-website/
├── index.html          # Main download page
├── style.css           # Stylesheet
├── downloads/          # Distribution files
│   ├── home-inventory-app_1.0.0-1_all.deb (Linux)
│   ├── Home_Inventory_Manager.AppImage (Linux - Universal)
│   └── Home Inventory Manager.exe (Windows)
└── README.md           # This file
```

## Local Development

Serve the website locally:

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx http-server

# Using PHP
php -S localhost:8000
```

Then open http://localhost:8000 in your browser.

## Deployment

This is a static website that can be deployed to:

- GitHub Pages
- Netlify
- Vercel
- Any static hosting service

### GitHub Pages Deployment

1. Push to a GitHub repository
2. Go to Settings → Pages
3. Select the branch to deploy (usually `main`)
4. Your site will be available at `https://yourusername.github.io/home-inventory-website/`

## Adding Download Files

Place the distribution files in the `downloads/` directory:

```bash
# Copy Linux package
cp ../home-inventory-app_1.0.0-1_all.deb downloads/

# Copy Linux AppImage
cp ../home-inventory-app/dist/Home_Inventory_Manager.AppImage downloads/

# Copy Windows installer (when available)
cp "Home Inventory Manager.exe" downloads/
```

## Customization

- Update links in `index.html` if your GitHub repository URL is different
- Add screenshots by replacing the placeholder sections
- Modify styling in `style.css` to match your brand
- Update version numbers when releasing new versions

## Features

- ✅ Responsive design (mobile-friendly)
- ✅ Download buttons for Linux and Windows
- ✅ Installation instructions
- ✅ Feature showcase
- ✅ FAQ section
- ✅ Screenshot placeholders
- ✅ System requirements
- ✅ Clean, modern design
