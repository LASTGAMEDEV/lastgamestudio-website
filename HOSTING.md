# HOSTING GUIDE — GitHub Pages (FREE)

## Step 1: Create the Repo
1. Go to https://github.com/new
2. Name it: `lastgamestudio-website` (or anything)
3. Make it **Public**
4. Click **Create repository**

## Step 2: Upload the File
**Option A — GitHub Web (easiest):**
1. In your new repo, click **"Add file" → "Upload files"**
2. Drag `index.html` from `lastgamestudio-site/`
3. Commit message: "Initial website launch"
4. Click **Commit changes**

**Option B — Git CLI:**
```bash
cd lastgamestudio-site
git init
git add index.html
git commit -m "Initial website launch"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/lastgamestudio-website.git
git push -u origin main
```

## Step 3: Enable GitHub Pages
1. In your repo, go to **Settings** tab
2. Click **Pages** in left sidebar
3. Under "Source", select **Deploy from a branch**
4. Select **main** branch, folder **/(root)**
5. Click **Save**
6. Wait 1-2 minutes
7. Your site will be live at: `https://YOUR_USERNAME.github.io/lastgamestudio-website`

## Step 4: Custom Domain (optional)
1. In Settings → Pages, under "Custom domain"
2. Enter: `lastgamestudio.com` (or www.lastgamestudio.com)
3. Click Save
4. Add DNS records at your domain registrar:
   - A record → `185.199.108.153`
   - A record → `185.199.109.153`
   - A record → `185.199.110.153`
   - A record → `185.199.111.153`
   - (Or CNAME → `YOUR_USERNAME.github.io`)
5. GitHub will auto-generate SSL certificate (HTTPS)

## DONE! 🎉
Your website is now live on the internet!

## To Update Later:
Just edit `index.html` in the repo — changes go live in ~1 minute.
