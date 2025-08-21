# GitHub Pages Deployment Guide

This guide will walk you through deploying Chun Lin's portfolio website to GitHub Pages.

## Prerequisites

1. A GitHub account
2. Git installed on your local machine
3. Node.js and npm installed

## Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name your repository `ChunPortfolio`
5. Make it public (required for free GitHub Pages)
6. Don't initialize with README (we already have one)
7. Click "Create repository"

## Step 2: Update Homepage URL

Before deploying, you need to update the homepage URL in `package.json`:

1. Open `package.json`
2. Find the "homepage" field
3. Replace `yourusername` with your actual GitHub username:

```json
{
  "homepage": "https://yourusername.github.io/ChunPortfolio"
}
```

## Step 3: Push Code to GitHub

If you haven't already, push your code to GitHub:

```bash
# Initialize git repository (if not already done)
git init

# Add all files
git add .

# Commit changes
git commit -m "Initial commit: Portfolio website"

# Add remote repository (replace 'yourusername' with your GitHub username)
git remote add origin https://github.com/yourusername/ChunPortfolio.git

# Push to GitHub
git push -u origin main
```

## Step 4: Deploy to GitHub Pages

1. Make sure all dependencies are installed:
```bash
npm install
```

2. Deploy the website:
```bash
npm run deploy
```

This command will:
- Build your React app
- Create a `gh-pages` branch
- Push the built files to that branch

## Step 5: Configure GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to "Pages" section (in the left sidebar)
4. Under "Source", select "Deploy from a branch"
5. Choose "gh-pages" branch
6. Click "Save"

## Step 6: Wait for Deployment

GitHub Pages will take a few minutes to deploy your site. You can check the status in the "Pages" section of your repository settings.

## Step 7: Access Your Website

Once deployed, your portfolio will be available at:
```
https://yourusername.github.io/ChunPortfolio
```

## Troubleshooting

### Common Issues

1. **404 Error**: Make sure you've configured GitHub Pages to use the `gh-pages` branch
2. **Routing Issues**: The app uses HashRouter which should work fine with GitHub Pages
3. **Build Errors**: Check that all dependencies are installed correctly

### Updating Your Site

To update your deployed site:

1. Make your changes locally
2. Commit and push to GitHub:
```bash
git add .
git commit -m "Update portfolio"
git push
```

3. Deploy again:
```bash
npm run deploy
```

### Custom Domain (Optional)

If you want to use a custom domain:

1. Go to your repository Settings > Pages
2. Enter your custom domain in the "Custom domain" field
3. Update the "homepage" field in `package.json` to match your custom domain
4. Add a `CNAME` file in the `public` folder with your domain name
5. Deploy again with `npm run deploy`

## File Structure After Deployment

After deployment, your repository will have:
- `main` branch: Your source code
- `gh-pages` branch: Built files for GitHub Pages

## Security Notes

- The `gh-pages` branch contains built files only
- Never commit sensitive information like API keys
- Use environment variables for any sensitive data

## Performance Tips

- Images are optimized automatically during build
- CSS and JavaScript are minified
- The site uses modern web technologies for optimal performance

---

Your portfolio is now live! 🎉
