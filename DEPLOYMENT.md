# BMI Calculator - Deployment Guide

This BMI Calculator is a static web application that can be deployed to various platforms. Choose the deployment method that best suits your needs.

## 🚀 Quick Deploy Options

### 1. Netlify (Recommended for beginners)

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/yourusername/bmi-calculator)

**Manual Deployment:**
1. Visit [netlify.com](https://netlify.com)
2. Sign up/Login with GitHub
3. Click "New site from Git"
4. Connect your GitHub repository
5. Deploy settings:
   - Build command: (leave empty)
   - Publish directory: `.` (root)
6. Click "Deploy site"

### 2. Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yourusername/bmi-calculator)

**Manual Deployment:**
1. Visit [vercel.com](https://vercel.com)
2. Sign up/Login with GitHub
3. Click "New Project"
4. Import your GitHub repository
5. Click "Deploy"

### 3. GitHub Pages

**Automatic Deployment (using GitHub Actions):**
1. Push your code to GitHub
2. Go to your repository settings
3. Navigate to "Pages" section
4. Select "GitHub Actions" as source
5. The workflow will automatically deploy on every push to main/master

**Manual Deployment:**
1. Go to your repository settings
2. Navigate to "Pages" section
3. Select "Deploy from a branch"
4. Choose `main` branch and `/ (root)` folder
5. Click "Save"

### 4. Firebase Hosting

1. Install Firebase CLI: `npm install -g firebase-tools`
2. Login: `firebase login`
3. Initialize: `firebase init hosting`
   - Select existing project or create new
   - Set public directory to `.` (current directory)
   - Configure as single-page app: No
   - Set up automatic builds: No
4. Deploy: `firebase deploy`

### 5. Surge.sh

1. Install Surge: `npm install -g surge`
2. Run: `surge`
3. Follow the prompts to deploy

### 6. Local Development

**Using Python (if Python is installed):**
```bash
python3 -m http.server 8000
```
Then visit: http://localhost:8000

**Using Node.js:**
```bash
npx serve .
```
Then visit: http://localhost:3000

**Using PHP (if PHP is installed):**
```bash
php -S localhost:8000
```
Then visit: http://localhost:8000

## 📁 Project Structure

```
bmi-calculator/
├── index.html          # Main HTML file
├── bmiCalculator.js    # JavaScript functionality
├── calculator.css      # Styling
├── bg.jpg             # Background image
├── package.json       # Project metadata
├── netlify.toml       # Netlify configuration
├── vercel.json        # Vercel configuration
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Actions workflow
```

## 🔧 Configuration Files

- **netlify.toml**: Configuration for Netlify deployment
- **vercel.json**: Configuration for Vercel deployment
- **.github/workflows/deploy.yml**: GitHub Actions workflow for automatic deployment
- **package.json**: Project metadata and scripts

## 🌐 Custom Domain

After deploying to any platform, you can configure a custom domain:

1. **Netlify**: Go to Site settings → Domain management
2. **Vercel**: Go to Project settings → Domains
3. **GitHub Pages**: Go to Repository settings → Pages → Custom domain

## 📱 Features

- Responsive BMI calculator
- Real-time BMI calculation
- Color-coded BMI categories
- Clean, modern interface
- Mobile-friendly design

## 🛠️ Troubleshooting

**Common Issues:**
- Ensure all files are in the root directory
- Check that file paths are correct (case-sensitive on some platforms)
- Verify that the repository is public (for free tiers)

**File Not Found Errors:**
- Make sure `index.html` is in the root directory
- Check that CSS and JS files are properly linked

## 📞 Support

If you encounter any issues during deployment, check the platform-specific documentation:
- [Netlify Docs](https://docs.netlify.com/)
- [Vercel Docs](https://vercel.com/docs)
- [GitHub Pages Docs](https://docs.github.com/en/pages)
- [Firebase Hosting Docs](https://firebase.google.com/docs/hosting)