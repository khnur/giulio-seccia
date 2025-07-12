# Giulio Seccia - Personal Academic Website

A modern, responsive personal website for Professor Giulio Seccia, Chair of the Department of Economics at Nazarbayev University.

## 🚀 Quick Start

1. **Clone or download** this repository
2. **Open `index.html`** in your web browser
3. **For deployment**, see [DEPLOYMENT.md](./DEPLOYMENT.md) for detailed instructions

## 🌐 Live Demo

Deploy your own version to Vercel in minutes! See the [deployment guide](./DEPLOYMENT.md) for step-by-step instructions.

## Features

- **Modern Design**: Clean, professional layout with responsive design
- **Cross-browser Compatibility**: Works perfectly in Chrome, Firefox, Safari, and Edge
- **Photo Placement**: Profile photo positioned next to contact information as requested
- **Proper Typography**: Fixed italic formatting for journal names in publications
- **Mobile-friendly**: Fully responsive design that works on all devices
- **Fast Loading**: Optimized CSS and images for quick page loads
- **Deployment Ready**: Configured for easy deployment to Vercel

## Website Structure

```
├── index.html                 # Main homepage
├── published_papers.html      # Published papers listing
├── work_in_progress.html      # Work in progress papers
├── teaching.html              # Teaching information
├── styles.css                 # Main stylesheet
├── CV-Seccia.pdf             # Curriculum Vitae
├── photo_website.jpg         # Profile photo (Chrome-compatible)
├── photo_website.webp        # Profile photo (original format)
├── papers/                   # Research papers folder
│   ├── bankruptcy.pdf
│   ├── jet-2000.pdf
│   └── tradec_clean240514.pdf
├── cmkts.pdf                 # Additional research paper
├── vercel.json               # Vercel deployment configuration
├── package.json              # Project metadata
├── .gitignore                # Git ignore rules
└── DEPLOYMENT.md             # Deployment instructions
```

## Key Improvements Made

1. **Fixed Photo Layout**: Photo now appears next to the address information using CSS Grid
2. **Fixed Italic Formatting**: Corrected broken `<i>` tags in publication titles
3. **Chrome Compatibility**: Converted webp image to jpg format for universal browser support
4. **Modern HTML5**: Upgraded from HTML 4.01 to modern HTML5 structure
5. **Responsive Design**: Added mobile-first responsive design
6. **Professional Navigation**: Sticky navigation bar with active state indicators
7. **Clean Typography**: Used Inter font family for modern, readable text
8. **Improved Accessibility**: Added proper alt tags and semantic HTML structure
9. **Deployment Ready**: Added Vercel configuration for easy deployment

## Browser Support

- Chrome (latest) ✅
- Firefox (latest) ✅
- Safari (latest) ✅
- Edge (latest) ✅
- Mobile browsers ✅

## 🚀 Deployment

This website is ready for deployment to Vercel! See [DEPLOYMENT.md](./DEPLOYMENT.md) for:

- Step-by-step deployment instructions
- GitHub integration setup
- Custom domain configuration
- Performance optimization details

## How to Use

1. **Local Development**: Open `index.html` in any web browser
2. **Local Server**: Run `python3 -m http.server 8000` or `npm run dev`
3. **Production**: Deploy to Vercel following the [deployment guide](./DEPLOYMENT.md)

## Content Updates

To update content:
- Edit the HTML files directly
- Replace PDFs in the respective folders
- Update the photo by replacing `photo_website.jpg`
- Modify `styles.css` for design changes
- Push changes to GitHub for automatic deployment (if using Vercel + GitHub)

## Technical Details

- **CSS Framework**: Custom CSS with modern features (Grid, Flexbox, CSS Variables)
- **Fonts**: Inter font family from Google Fonts
- **Images**: Optimized JPG format for compatibility
- **Performance**: Minimal dependencies, fast loading times
- **SEO**: Proper meta tags and semantic HTML structure
- **Hosting**: Optimized for Vercel deployment with CDN and caching

## 📁 Files Not Included

The original `WEBSITE/` folder is excluded from version control (see `.gitignore`). This contains the source materials that were used to create the modern website.

---

*Last updated: July 2025* 