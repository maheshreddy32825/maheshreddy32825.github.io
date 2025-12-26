# Dynamic GitHub Pinned Repos Setup

## ✅ Implementation Complete

Your portfolio now **dynamically fetches your pinned repos** from GitHub and displays them on the projects page.

---

## 🔐 Configuration Required

### **Local Development**
A `.env.local` file has been created with:
```
GITHUB_TOKEN=your_token_here
GITHUB_USERNAME=maheshreddy32825
```

### **Vercel Production Setup**

You need to add environment variables to Vercel:

**Steps:**
1. Go to: https://vercel.com/dashboard
2. Select project: `maheshreddy32825.github.io`
3. Click **Settings** → **Environment Variables**
4. Add two variables:

   **Variable 1 - GITHUB_TOKEN:**
   - Name: `GITHUB_TOKEN`
   - Value: `[Your GitHub Personal Access Token]`
   - Environments: All (Production, Preview, Development)

   **Variable 2 - GITHUB_USERNAME:**
   - Name: `GITHUB_USERNAME`
   - Value: `maheshreddy32825`
   - Environments: All

5. Click **Redeploy** to rebuild with new variables

---

## 📊 What Gets Displayed

For each pinned repo:
- 📦 Repository name
- 📝 Description
- 🌐 Primary language
- ⭐ Star count
- 🔗 Direct GitHub link

---

## 🔄 How It Works

1. **Build time:** Portfolio fetches your 4-6 pinned repos from GitHub
2. **Auto-sync:** When you pin/unpin repos, next build gets the latest
3. **Fallback:** If API fails, shows static projects instead

---

## ✨ Features

- ✅ Real-time sync with GitHub
- ✅ Supports up to 6 pinned repos
- ✅ Shows language, stars, descriptions
- ✅ Direct links to repos
- ✅ Graceful fallback on API errors
- ✅ Secure token handling
