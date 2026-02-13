# How to Deploy to Vercel

There are two main ways to deploy your Valentine webpage to Vercel:

## Method 1: GitHub Integration (Recommended - Easiest) 🚀

This method automatically deploys when you push to GitHub.

### Steps:

1. **Go to Vercel**
   - Visit [vercel.com](https://vercel.com)
   - Sign up or log in (you can use your GitHub account)

2. **Import Your Repository**
   - Click "Add New..." → "Project"
   - Click "Import Git Repository"
   - Find and select `PudPawat/Valentine-simple-web`
   - Click "Import"

3. **Configure Project**
   - **Framework Preset**: Select "Other" (since it's a static HTML file)
   - **Root Directory**: Leave as `./` (default)
   - **Build Command**: Leave empty (no build needed for static HTML)
   - **Output Directory**: Leave empty or set to `./`
   - **Install Command**: Leave empty

4. **Deploy**
   - Click "Deploy"
   - Wait 1-2 minutes for deployment
   - Your site will be live at a URL like: `valentine-simple-web.vercel.app`

5. **Automatic Updates**
   - Every time you push to GitHub, Vercel will automatically redeploy!

## Method 2: Vercel CLI (For Command Line) 💻

### Step 1: Install Vercel CLI

```bash
npm install -g vercel
```

Or if you don't have npm:
```bash
# Using Homebrew (Mac)
brew install vercel-cli

# Or download from: https://vercel.com/download
```

### Step 2: Login to Vercel

```bash
vercel login
```

This will open your browser to authenticate.

### Step 3: Deploy

```bash
cd /home/pawatchun/Desktop/Valentine
vercel
```

Follow the prompts:
- **Set up and deploy?** → Yes
- **Which scope?** → Select your account
- **Link to existing project?** → No (first time)
- **What's your project's name?** → `valentine-simple-web` (or press Enter for default)
- **In which directory is your code located?** → `./` (press Enter)

### Step 4: Production Deploy

For production deployment:
```bash
vercel --prod
```

## Custom Domain (Optional) 🌐

After deployment, you can add a custom domain:

1. Go to your project on Vercel dashboard
2. Click "Settings" → "Domains"
3. Add your domain name
4. Follow DNS configuration instructions

## Environment Variables (Not needed for this project)

Since this is a static HTML page, no environment variables are needed.

## Troubleshooting

- **Build errors?** Make sure Framework Preset is set to "Other"
- **404 errors?** Ensure `index.html` is in the root directory
- **Styling not working?** Check that all CSS is in the HTML file (which it is)

## Quick Commands Reference

```bash
# Deploy to preview
vercel

# Deploy to production
vercel --prod

# View deployments
vercel ls

# Remove deployment
vercel remove
```

---

**That's it!** Your Valentine webpage will be live on the internet! 💕
