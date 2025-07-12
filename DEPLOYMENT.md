# Deployment Guide - Giulio Seccia Website

This guide will help you deploy the academic website to Vercel, a fast and reliable hosting platform.

## 📋 Prerequisites

1. **Git** installed on your computer
2. **GitHub account** (free)
3. **Vercel account** (free) - sign up at [vercel.com](https://vercel.com)

## 🚀 Deployment Methods

### Method 1: Direct Vercel Deployment (Recommended)

#### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and create a new repository
2. Name it `giulio-seccia-website` (or your preferred name)
3. Make it **public** or **private** (your choice)
4. **Don't** initialize with README, .gitignore, or license (we already have these)

#### Step 2: Push Your Code to GitHub

```bash
# Initialize git repository (if not already done)
git init

# Add all files
git add .

# Commit the files
git commit -m "Initial commit - Academic website for Giulio Seccia"

# Add your GitHub repository as remote
git remote add origin https://github.com/YOUR-USERNAME/giulio-seccia-website.git

# Push to GitHub
git push -u origin main
```

#### Step 3: Deploy with Vercel

1. **Go to Vercel**: Visit [vercel.com](https://vercel.com) and sign in
2. **Import Project**: Click "New Project" or "Import Git Repository"
3. **Connect GitHub**: Connect your GitHub account if not already connected
4. **Select Repository**: Choose your `giulio-seccia-website` repository
5. **Configure Project**:
   - **Framework Preset**: Select "Other" (since it's a static HTML site)
   - **Root Directory**: Leave as `./` (root)
   - **Build Command**: Leave empty (no build needed)
   - **Output Directory**: Leave empty (will serve from root)
6. **Deploy**: Click "Deploy"

#### Step 4: Access Your Website

- Vercel will provide a URL like: `https://giulio-seccia-website.vercel.app`
- Your website is now live! 🎉

### Method 2: Vercel CLI Deployment

If you prefer using the command line:

#### Step 1: Install Vercel CLI

```bash
npm install -g vercel
```

#### Step 2: Login to Vercel

```bash
vercel login
```

#### Step 3: Deploy

```bash
# From your project directory
vercel

# Follow the prompts:
# ? Set up and deploy "~/giulio-seccia"? [Y/n] y
# ? Which scope should contain your project? [Your account]
# ? Link to existing project? [y/N] n
# ? What's your project's name? giulio-seccia-website
# ? In which directory is your code located? ./
```

#### Step 4: Deploy to Production

```bash
vercel --prod
```

## 🔧 Configuration Details

### Files Created for Deployment

1. **`.gitignore`** - Excludes WEBSITE folder and unnecessary files
2. **`vercel.json`** - Vercel configuration with optimizations
3. **`package.json`** - Project metadata and scripts

### Key Features Enabled

- ✅ **Clean URLs** - `/about` instead of `/about.html`
- ✅ **Security Headers** - XSS protection, content type sniffing prevention
- ✅ **Asset Caching** - Optimized caching for CSS, JS, images, and PDFs
- ✅ **Fast Loading** - Vercel's global CDN

## 🌐 Custom Domain (Optional)

To use a custom domain like `giulioseccia.com`:

1. **Purchase Domain**: Buy from any domain registrar
2. **Add to Vercel**: 
   - Go to your project settings in Vercel
   - Click "Domains"
   - Add your custom domain
   - Update DNS settings as instructed

## 📊 Project Structure

```
giulio-seccia-website/
├── index.html              # Home page
├── published_papers.html   # Publications
├── work_in_progress.html   # Work in progress
├── teaching.html           # Teaching info
├── styles.css              # Main stylesheet
├── CV-Seccia.pdf          # Curriculum Vitae
├── photo_website.jpg      # Profile photo
├── papers/                # Research papers
│   ├── bankruptcy.pdf
│   ├── jet-2000.pdf
│   └── tradec_clean240514.pdf
├── vercel.json            # Vercel configuration
├── package.json           # Project metadata
├── .gitignore             # Git ignore rules
└── README.md              # Project documentation
```

## 🔄 Updating Your Website

### For GitHub + Vercel Integration:

1. Make changes to your files
2. Commit and push to GitHub:
   ```bash
   git add .
   git commit -m "Update website content"
   git push
   ```
3. Vercel will automatically redeploy your site! 🚀

### For CLI Deployment:

```bash
# Make your changes, then:
vercel --prod
```

## 🛠️ Development Server

To test locally before deployment:

```bash
# Start local server
python3 -m http.server 8000

# Or use npm script
npm run dev
```

Visit `http://localhost:8000` to preview your site.

## 📈 Performance Features

- **Global CDN**: Fast loading worldwide
- **Automatic HTTPS**: Secure connections
- **Optimized Images**: Automatic image optimization
- **Caching**: Smart caching for better performance

## 🆘 Troubleshooting

### Common Issues:

1. **404 Errors**: Check file paths and ensure all files are committed
2. **Styling Issues**: Verify CSS file paths and font loading
3. **PDF Not Loading**: Ensure PDF files are in the correct directory

### Getting Help:

- **Vercel Docs**: [vercel.com/docs](https://vercel.com/docs)
- **GitHub Issues**: Create an issue in your repository
- **Vercel Support**: Contact through their dashboard

## 🎯 Next Steps

1. **Deploy the website** following the steps above
2. **Test all pages** and links
3. **Share the URL** with colleagues
4. **Set up custom domain** (optional)
5. **Add analytics** (Google Analytics, etc.)

Your academic website is now ready for the world! 🌍

---

*Happy deploying! 🚀* 