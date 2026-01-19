# GitHub Pages Deployment Guide for NilPay

Follow these steps to deploy your landing page on GitHub Pages (it's free!):

## Step 1: Install Git
If you haven't already, download and install Git from: https://git-scm.com/download/win
- Run the installer
- Use default settings
- Restart your terminal/VS Code after installation

## Step 2: Create a GitHub Account
1. Go to https://github.com
2. Click "Sign up"
3. Create your account (free)

## Step 3: Create a New Repository
1. Log into GitHub
2. Click the **+** icon (top right) → "New repository"
3. Repository name: **nilpay** (or your preferred name)
4. Description: "NilPay - One Wallet. Every Network."
5. Choose **Public** (required for free GitHub Pages)
6. Click "Create repository"

## Step 4: Push Your Code to GitHub

Open Terminal/PowerShell in VS Code (Ctrl + `) or open it separately and run these commands:

```powershell
cd "c:\Users\Admin\Desktop\NilPay"

# Configure git with your GitHub credentials (one-time setup)
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

# Initialize repository
git init

# Add all files
git add .

# Create initial commit
git commit -m "Initial commit: NilPay landing page"

# Add remote (replace YOUR_USERNAME with your actual GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/nilpay.git

# Push to GitHub (you'll be prompted to login)
git branch -M main
git push -u origin main
```

## Step 5: Enable GitHub Pages

1. Go to your repository on GitHub: https://github.com/YOUR_USERNAME/nilpay
2. Click **Settings** (top menu)
3. Scroll down to **Pages** (left sidebar)
4. Under "Source", select **Deploy from a branch**
5. Select branch: **main**
6. Select folder: **/ (root)**
7. Click **Save**

Wait 1-2 minutes, then refresh the page. GitHub will show you a message like:
> "Your site is published at https://YOUR_USERNAME.github.io/nilpay"

## Step 6: Your Site is Live! 🎉

Visit: `https://YOUR_USERNAME.github.io/nilpay`

That's it! Your landing page is now live on the internet.

## Future Updates

Whenever you make changes to your files, run:

```powershell
cd "c:\Users\Admin\Desktop\NilPay"

git add .
git commit -m "Update: describe your changes here"
git push
```

GitHub Pages will automatically update your live site within a few minutes.

## Optional: Custom Domain

If you own a domain, you can point it to your GitHub Pages site:
1. In Settings → Pages, add your custom domain
2. Update your domain DNS settings (instructions vary by registrar)

## Troubleshooting

**"fatal: not a git repository"**
- Make sure you're in the correct directory: `cd "c:\Users\Admin\Desktop\NilPay"`

**"git not recognized"**
- Git isn't installed. Download it from https://git-scm.com/download/win and restart your terminal

**Changes not showing after push**
- Wait 2-3 minutes for GitHub to redeploy
- Clear your browser cache (Ctrl + Shift + Delete)
- Check the Actions tab in your GitHub repo to see deployment status

Need help? Just ask!
