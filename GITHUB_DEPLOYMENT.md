# Deploying to GitHub Pages

This document provides step-by-step instructions for deploying the Virtual Concert Finder Chatbot to GitHub Pages.

## Prerequisites

1. Create a GitHub account if you don't have one already: [Join GitHub](https://github.com/join)
2. Install Git on your computer if not already installed: [Download Git](https://git-scm.com/downloads)

## Step 1: Create a GitHub Repository

1. Log in to GitHub
2. Click on the "+" icon in the top right corner and select "New repository"
3. Name your repository (e.g., "virtual-concert-chatbot")
4. Choose "Public" visibility
5. Leave "Initialize this repository with a README" unchecked (we already have one)
6. Click "Create repository"

## Step 2: Connect Your Local Repository to GitHub

After creating the repository, GitHub will show you commands to push an existing repository. Run these commands in your terminal:

```bash
git remote add origin https://github.com/yourusername/virtual-concert-chatbot.git
git branch -M main
git push -u origin main
```

Replace `yourusername` with your actual GitHub username.

## Step 3: Enable GitHub Pages

1. Go to your GitHub repository
2. Click on "Settings" (tab on the top right)
3. Scroll down to "GitHub Pages" section
4. Under "Source", select "main" branch
5. Click "Save"
6. Wait a few minutes for your site to deploy
7. GitHub will show you the URL where your site is published (typically `https://yourusername.github.io/virtual-concert-chatbot/`)

## Step 4: Verify Your Deployment

1. Visit the URL provided by GitHub Pages
2. Confirm that your chatbot is working correctly
3. Test the main features to ensure they're functioning with the fallback data

## Additional Customization

1. Update the GitHub link in `index.html` to point to your actual repository
2. Consider adding a custom domain if you want a more professional URL
3. Update the Open Graph meta tags in `index.html` to use an actual image from your project

## Troubleshooting

If your site doesn't deploy:
- Check that all files are properly committed and pushed to GitHub
- Ensure GitHub Pages is enabled for the main branch
- Look for any error messages in the GitHub Pages section of your repository settings

If the chatbot doesn't work properly:
- Check the browser console for errors
- Verify that all paths in the HTML file are correct (they should be relative)
- Make sure the fallback data is working correctly 