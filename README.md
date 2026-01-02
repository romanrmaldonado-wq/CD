# CD Performance Tracker - PWA Setup Guide

## 📦 Files to Upload

You need to upload these **3 files** to make the PWA work:

1. **cd-performance-tracker.html** - Main app file
2. **manifest.json** - PWA configuration
3. **sw.js** - Service worker for offline functionality

---

## 🚀 GitHub Pages Setup (Step-by-Step)

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **"+"** button (top right) → **"New repository"**
3. Name it: `cd-tracker` (or any name you want)
4. Make it **Public**
5. Click **"Create repository"**

### Step 2: Upload Files

**Option A: Using GitHub Web Interface (Easiest)**

1. On your new repository page, click **"uploading an existing file"** or **"Add file" → "Upload files"**
2. Drag and drop all 3 files:
   - cd-performance-tracker.html
   - manifest.json
   - sw.js
3. Scroll down and click **"Commit changes"**

**Option B: Using Git Command Line**

```bash
# Clone your new repository
git clone https://github.com/YOUR-USERNAME/cd-tracker.git
cd cd-tracker

# Copy the 3 files into this folder
# Then:
git add .
git commit -m "Add CD Performance Tracker PWA"
git push
```

### Step 3: Enable GitHub Pages

1. In your repository, click **"Settings"** (top menu)
2. Scroll down to **"Pages"** in the left sidebar
3. Under "Source":
   - Select **"Deploy from a branch"**
   - Choose **"main"** branch
   - Keep folder as **"/ (root)"**
4. Click **"Save"**
5. Wait 1-2 minutes for deployment

### Step 4: Get Your URL

Your app will be live at:
```
https://YOUR-USERNAME.github.io/cd-tracker/cd-performance-tracker.html
```

For example, if your username is `romanpower`:
```
https://romanpower.github.io/cd-tracker/cd-performance-tracker.html
```

---

## 📱 Install on iPhone

Once your GitHub Pages site is live:

1. **Open Safari** on your iPhone (must be Safari, not Chrome)
2. Go to your GitHub Pages URL
3. Tap the **Share button** (square with arrow pointing up)
4. Scroll down and tap **"Add to Home Screen"**
5. Name it "CD Stats" or whatever you prefer
6. Tap **"Add"**

### ✅ Done! 

The app icon will appear on your home screen with the 📊 emoji. It will:
- Open in full screen (no browser bars)
- Work offline after first load
- Save all your data locally on your device

---

## 🔄 Updating the App

To update your app later:

1. Go to your GitHub repository
2. Click on the file you want to edit (e.g., `cd-performance-tracker.html`)
3. Click the pencil icon **"Edit this file"**
4. Make your changes
5. Scroll down and click **"Commit changes"**
6. Wait 1-2 minutes for GitHub Pages to update

**On your iPhone:**
- Just refresh the app (swipe down) to get the latest version
- Or delete and re-add to home screen if there are major changes

---

## ⚙️ Optional: Custom Domain

If you want a custom URL like `cdtracker.yourname.com`:

1. Buy a domain (from Namecheap, Google Domains, etc.)
2. In your repo Settings → Pages
3. Add your custom domain
4. Follow GitHub's DNS configuration instructions

---

## 🆘 Troubleshooting

**App not loading on iPhone?**
- Make sure you're using Safari, not Chrome
- Check that all 3 files are uploaded
- Try clearing Safari cache: Settings → Safari → Clear History and Website Data

**Updates not showing?**
- Wait 2-3 minutes after pushing to GitHub
- Hard refresh in Safari: Hold the refresh button
- Check GitHub Actions tab to see if deployment finished

**PWA not installing?**
- Ensure HTTPS is enabled (GitHub Pages does this automatically)
- All 3 files must be in the same directory
- Try opening in Safari's private mode first

---

## 📊 Features

- **Month-by-month tracking** with dropdown selector
- **Daily updates** with +/- buttons for Estimates and Appointments
- **Baseline editing** - Set and edit 2025 baseline data for any month
- **Full year view** - See all 12 months at a glance
- **Automatic saving** - All data saves locally to your device
- **Offline support** - Works without internet after first load
- **Year-over-year comparison** - Track your growth vs 2025

---

## 💾 Your Data

All data is stored locally on your iPhone using localStorage. This means:
- ✅ Your data never leaves your device
- ✅ Works completely offline
- ✅ Fast and private
- ⚠️ If you delete the app, you'll lose the data
- ⚠️ Data doesn't sync between devices

To backup your data, you can export it from Safari's Developer Console, but normal usage shouldn't require this.

---

Need help? Issues with setup? Let me know! 🚀
