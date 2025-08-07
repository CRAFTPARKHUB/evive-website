# EVIVE Website Deployment

This folder contains your EVIVE architectural design website ready for deployment to Netlify.

## Files Included

- `index.html` - Main website file (Czech version)
- `netlify.toml` - Netlify configuration file
- `framerusercontent.com/` - All assets, images, modules, and content
- `app.framerstatic.com/` - Framer static app files
- `ga.jspm.io/` - Third-party JavaScript modules
- `_DataURI/` - Data URI files

## Deployment Instructions

### Option 1: Drag & Drop Deployment (Easiest)
1. Go to [netlify.com](https://netlify.com) and sign up/login
2. Click "Add new site" → "Deploy manually"
3. Drag and drop the entire `netlify-deploy` folder to the deployment area
4. Your site will be deployed with a random URL (you can customize it later)

### Option 2: Git Repository Deployment
1. Create a new repository on GitHub
2. Upload the contents of the `netlify-deploy` folder to your repository
3. On Netlify, click "Add new site" → "Import an existing project"
4. Connect your GitHub account and select the repository
5. Deploy settings:
   - Build command: `echo 'Static site - no build required'`
   - Publish directory: `.` (root)

### Option 3: Netlify CLI
1. Install Netlify CLI: `npm install -g netlify-cli`
2. Run `netlify login` to authenticate
3. In this directory, run: `netlify deploy --prod --dir=.`

## Custom Domain
After deployment, you can add your custom domain in the Netlify dashboard under "Domain settings".

## Features Configured
- ✅ "Made in Framer" badge removed
- ✅ Proper caching headers for assets
- ✅ Security headers
- ✅ URL redirects for Czech version
- ✅ 404 handling
- ✅ Optimized for performance

## Note
This website was originally built with Framer and has been optimized for deployment on Netlify while maintaining all functionality and removing the Framer branding.
