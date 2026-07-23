# Publishing to GitHub & GitHub Pages

Follow these steps to publish your cheatsheet on GitHub and access it from anywhere (including mobile):

## Step 1: Create a GitHub Repository

1. Go to [github.com](https://github.com) and log in
2. Click **New repository** (or use the `+` menu)
3. Repository name: `devops-interview-cheatsheet` (or your preferred name)
4. Description: "DevOps/SRE Interview Cheatsheet - Azure, AWS, Kubernetes, Terraform"
5. Choose **Public** (so you can access it from mobile via GitHub Pages)
6. **Do NOT** initialize with README (we already have one)
7. Click **Create repository**

## Step 2: Push to GitHub (Using Git Command Line)

### Option A: If you have Git installed

Open terminal/PowerShell and navigate to the folder:

```bash
cd "C:\Users\DELL\Downloads\New folder (2)"

# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: DevOps/SRE interview cheatsheet"

# Add remote (replace 'yourusername' with your GitHub username)
git remote add origin https://github.com/yourusername/devops-interview-cheatsheet.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Option B: Upload via GitHub Web Interface

1. Go to your new repository on GitHub
2. Click **Add file** → **Upload files**
3. Drag and drop these files:
   - `interview-cheatsheet-v2_1.html`
   - `README.md`
   - `.gitignore`
4. Click **Commit changes**

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (gear icon)
3. Scroll to **Pages** section (left sidebar)
4. Under "Source", select **Deploy from a branch**
5. Select branch: **main** and folder: **/ (root)**
6. Click **Save**

After a few seconds, you'll see:
> "Your site is live at: https://yourusername.github.io/devops-interview-cheatsheet"

## Step 4: Access on Mobile

### Option A: GitHub Pages (Easiest)
- Go to: `https://yourusername.github.io/devops-interview-cheatsheet`
- Bookmark it in your mobile browser
- Works offline too (after first load)

### Option B: Direct GitHub File
- Go to: `https://github.com/yourusername/devops-interview-cheatsheet`
- Click on `interview-cheatsheet-v2_1.html`
- Click **Raw** button in GitHub preview
- Or click the download icon to download and open locally

### Option C: Mobile GitHub App
- Download GitHub mobile app
- Access your repository
- View the HTML file directly

## Mobile Testing Checklist

After publishing, test on mobile:

- [ ] Sidebar menu appears as hamburger (☰)
- [ ] Search works (press `/` key)
- [ ] Subject buttons work
- [ ] Details sections expand/collapse
- [ ] Tables are readable and scrollable
- [ ] No horizontal scrolling needed
- [ ] Tap-friendly buttons and links
- [ ] Fast loading and smooth scrolling

## Browser Compatibility

Works in:
- ✅ Chrome/Edge (Desktop & Mobile)
- ✅ Firefox (Desktop & Mobile)
- ✅ Safari (Desktop & Mobile)
- ✅ All modern mobile browsers

## Tips for Mobile Access

1. **Bookmark it** in your browser's home screen for quick access
2. **Search efficiently** — Press `/` and type to find topics instantly
3. **Offline access** — GitHub Pages caches it, works offline after first load
4. **Share the link** — Send `https://yourusername.github.io/devops-interview-cheatsheet` to your study group

## Updating the Cheatsheet

To add more content:

```bash
cd "C:\Users\DELL\Downloads\New folder (2)"

# Edit the HTML file in your editor

# Commit changes
git add interview-cheatsheet-v2_1.html
git commit -m "Add: New topic XYZ"
git push origin main
```

Changes appear on GitHub Pages within ~1 minute.

## Troubleshooting

### Pages not showing up?
- Wait 2-3 minutes after enabling Pages
- Check Settings → Pages → Source is set correctly
- Repository must be public

### File not updating on mobile?
- Hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)
- Clear browser cache
- Wait 5 minutes for GitHub Pages CDN to sync

### Can't push to GitHub?
- Check you have git installed: `git --version`
- Verify remote: `git remote -v`
- For authentication, use personal access token instead of password (GitHub no longer allows password auth)

## GitHub Personal Access Token (if needed)

If git push fails with authentication:

1. Go to [github.com/settings/tokens](https://github.com/settings/tokens)
2. Click **Generate new token (classic)**
3. Scopes: Select `repo` (full control of private repositories)
4. Click **Generate token**
5. Copy the token
6. Use it as password when pushing

## Next Steps

- Star the repository ⭐ (if helpful)
- Share with your team
- Add more topics based on your interview experiences
- Contribute improvements via pull requests

---

**Questions?** Check the README.md for more info.
