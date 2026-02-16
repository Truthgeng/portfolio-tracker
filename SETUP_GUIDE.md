# GitHub Setup Guide

Follow these steps to upload your portfolio tracker to GitHub.

## Option 1: Using GitHub Web Interface (Easiest)

### Step 1: Create a New Repository
1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon in the top right → **New repository**
3. Name it: `portfolio-tracker` (or your preferred name)
4. Add description: "Investment portfolio tracker with web app and Excel spreadsheet"
5. Choose **Public** or **Private**
6. ✅ Check "Add a README file"
7. Click **Create repository**

### Step 2: Upload Your Files
1. In your new repository, click **Add file** → **Upload files**
2. Drag and drop these files:
   - `portfolio_tracker.html`
   - `portfolio_tracker.xlsx`
   - `README.md` (replace the default one)
   - `.gitignore`
3. Add commit message: "Initial commit - Portfolio tracker"
4. Click **Commit changes**

### Step 3: Enable GitHub Pages (for Web App)
1. Go to **Settings** → **Pages** (in left sidebar)
2. Under "Source", select **main** branch
3. Click **Save**
4. Wait 1-2 minutes, then visit: `https://yourusername.github.io/portfolio-tracker/portfolio_tracker.html`

---

## Option 2: Using Git Command Line

### Prerequisites
- Git installed ([download here](https://git-scm.com/downloads))
- GitHub account

### Step 1: Create Repository on GitHub
1. Go to [github.com](https://github.com) → **New repository**
2. Name it `portfolio-tracker`
3. **Don't** initialize with README (we'll push our own)
4. Click **Create repository**

### Step 2: Upload from Command Line
Open your terminal/command prompt in the folder containing your files:

```bash
# Initialize git repository
git init

# Add all files
git add portfolio_tracker.html portfolio_tracker.xlsx README.md .gitignore

# Create first commit
git commit -m "Initial commit - Portfolio tracker"

# Connect to GitHub (replace YOUR_USERNAME and YOUR_REPO)
git remote add origin https://github.com/YOUR_USERNAME/portfolio-tracker.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages
Follow Option 1, Step 3 above.

---

## Option 3: Using GitHub Desktop (GUI)

### Prerequisites
- [GitHub Desktop](https://desktop.github.com/) installed

### Steps
1. Open GitHub Desktop
2. **File** → **New Repository**
   - Name: `portfolio-tracker`
   - Local path: Choose where your files are located
3. Copy your portfolio files into that folder
4. In GitHub Desktop, you'll see the files listed
5. Add commit message: "Initial commit"
6. Click **Commit to main**
7. Click **Publish repository**
8. Choose public/private and click **Publish**
9. Enable GitHub Pages (see Option 1, Step 3)

---

## What Each File Does

- **portfolio_tracker.html** - The interactive web application
- **portfolio_tracker.xlsx** - The Excel spreadsheet tracker
- **README.md** - Project documentation (shows on GitHub homepage)
- **.gitignore** - Tells Git which files to ignore

---

## Accessing Your Web App

Once GitHub Pages is enabled, your web app will be live at:
```
https://YOUR_USERNAME.github.io/portfolio-tracker/portfolio_tracker.html
```

Share this URL with anyone, and they can use your tracker!

---

## Tips

- **Keep your data private**: The web app stores data only in your browser (not on GitHub)
- **Excel file is a template**: Download and customize it for your personal use
- **Update anytime**: Just upload new files to GitHub to update your project
- **Custom domain**: In GitHub Pages settings, you can add your own domain name

---

## Need Help?

- [GitHub Docs](https://docs.github.com/en/get-started)
- [Git Basics Tutorial](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)
- [GitHub Pages Guide](https://docs.github.com/en/pages)
