# 🚀 Deploy EVIVE Website to GitHub

Your EVIVE website is ready for GitHub deployment! Follow these simple steps:

## 📋 Prerequisites
- GitHub account (sign up at [github.com](https://github.com) if you don't have one)
- Git is already set up in this folder ✅

## 🎯 Step-by-Step GitHub Deployment

### Step 1: Create GitHub Repository
1. Go to [github.com](https://github.com) and sign in
2. Click the **"+"** button in the top-right corner
3. Select **"New repository"**
4. Repository settings:
   - **Repository name**: `evive-website` (or your preferred name)
   - **Description**: "EVIVE - Modern Architectural Design Website"
   - **Visibility**: Choose Public or Private
   - **DO NOT** initialize with README, .gitignore, or license (we already have these)
5. Click **"Create repository"**

### Step 2: Connect and Push to GitHub
After creating the repository, GitHub will show you commands. Use these commands in Terminal:

```bash
# Add your GitHub repository as remote origin
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git

# Rename the main branch to 'main' (modern standard)
git branch -M main

# Push your website to GitHub
git push -u origin main
```

**Replace `YOUR_USERNAME` and `YOUR_REPOSITORY_NAME` with your actual GitHub username and repository name.**

### Example:
If your GitHub username is `johndoe` and repository name is `evive-website`:
```bash
git remote add origin https://github.com/johndoe/evive-website.git
git branch -M main
git push -u origin main
```

## 🌐 Deploy to Netlify from GitHub

Once your code is on GitHub, you can easily deploy to Netlify:

### Option 1: Netlify Dashboard (Recommended)
1. Go to [netlify.com](https://netlify.com) and sign up/login
2. Click **"Add new site"** → **"Import an existing project"**
3. Choose **"Deploy with GitHub"**
4. Authorize Netlify to access your GitHub account
5. Select your repository (`evive-website`)
6. Deploy settings (pre-configured in `netlify.toml`):
   - **Branch to deploy**: `main`
   - **Build command**: `echo 'Static site - no build required'`
   - **Publish directory**: `.` (root)
7. Click **"Deploy site"**
8. Your site will be live in minutes with a custom Netlify URL!

### Option 2: Netlify CLI
```bash
# Install Netlify CLI (if not already installed)
npm install -g netlify-cli

# Login to Netlify
netlify login

# Link to existing site or create new
netlify init

# Deploy
netlify deploy --prod
```

## 🎨 What's Included in Your Deployment

✅ **Complete EVIVE website** with all functionality  
✅ **"Made in Framer" badge removed**  
✅ **Optimized for performance** with proper caching  
✅ **Security headers** configured  
✅ **Mobile-responsive design**  
✅ **Czech language support**  
✅ **All images and assets** properly organized  
✅ **SEO optimized** with meta tags  

## 🔧 Future Updates

To update your website:
1. Make changes to files in this folder
2. Commit changes:
   ```bash
   git add .
   git commit -m "Update website content"
   git push origin main
   ```
3. Netlify will automatically redeploy your site!

## 🎯 Custom Domain Setup

After deployment on Netlify:
1. Go to your site's Netlify dashboard
2. Click **"Domain settings"**
3. Click **"Add custom domain"**
4. Enter your domain name
5. Follow the DNS configuration instructions

## 📞 Support

If you encounter any issues:
- Check the [Netlify documentation](https://docs.netlify.com/)
- Visit [GitHub Help](https://help.github.com/)
- All configuration is already optimized in this repository

---

**Your website structure:**
- 📄 `index.html` - Main website file
- ⚙️ `netlify.toml` - Deployment configuration
- 🖼️ `framerusercontent.com/` - All assets and images
- 🔧 `app.framerstatic.com/` - JavaScript modules
- 📝 `.gitignore` - Git exclusions
- 📖 `README.md` - Project documentation

**Ready to deploy! 🚀**
