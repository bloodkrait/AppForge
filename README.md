# AppForge

Your personal AI-powered app idea generator. Runs entirely in the browser — no server, no build step.

---

## First-time setup (do this once)

### Step 1 — Get your Anthropic API key

1. Go to [console.anthropic.com](https://console.anthropic.com)
2. Sign in (or create a free account)
3. Click **API Keys** in the left sidebar
4. Click **Create Key**, give it a name like "AppForge"
5. Copy the key — it starts with `sk-ant-...`

> ⚠️ You'll need to add a payment method and add credits ($5 is plenty to start). Each idea generation costs roughly $0.01–0.03.

---

### Step 2 — Add your API key to the app

1. Open `index.html` in any text editor (Notepad on Windows, TextEdit on Mac)
2. Find this line near the top:
   ```
   window.ANTHROPIC_API_KEY = "YOUR_API_KEY_HERE";
   ```
3. Replace `YOUR_API_KEY_HERE` with your actual key:
   ```
   window.ANTHROPIC_API_KEY = "sk-ant-api03-...your key here...";
   ```
4. Save the file

---

### Step 3 — Put it on GitHub

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** button → **New repository**
3. Name it `app-forge` (or anything you like)
4. Set it to **Public**
5. Click **Create repository**
6. On the next screen, click **uploading an existing file**
7. Drag and drop `index.html` and `README.md` into the upload area
8. Click **Commit changes**

---

### Step 4 — Turn on GitHub Pages (makes it a real URL)

1. In your repo, click **Settings** (top tab)
2. Scroll down to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Under **Branch**, select `main` and click **Save**
5. Wait 1–2 minutes, then your app is live at:
   ```
   https://YOUR-GITHUB-USERNAME.github.io/app-forge/
   ```

Bookmark that URL on your phone. Done.

---

## Updating the app

When Claude gives you a new version of the app:

1. Open your repo on GitHub
2. Click on `index.html`
3. Click the **pencil icon** (Edit)
4. Select all the text and replace it with the new code
5. Click **Commit changes**

Your live URL updates automatically within a minute or two.

---

## Your data

- All saved ideas and project data are stored in your browser's localStorage
- They persist between sessions on the same device/browser
- They do NOT sync between devices (phone vs computer)
- Clearing your browser data will erase them — use the "Export Brief" button to save important ideas as files

---

## Keeping your API key safe

- Your key is in the HTML file — **keep the repo Public** is fine since GitHub Pages requires it, but be aware the key is visible in the source code
- If you ever share your screen or the file, others could see the key
- You can set spending limits at [console.anthropic.com](https://console.anthropic.com) under **Limits** so there's no surprise bill
- If the key ever gets compromised, just delete it and create a new one

---

## Files

| File | What it is |
|------|------------|
| `index.html` | The entire app — this is the only file you need |
| `README.md` | This guide |
| `app-forge-v3.jsx` | Claude project file — upload this to your Claude Project so Claude remembers the codebase |
