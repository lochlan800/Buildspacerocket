# GitHub Pages Deployment

## How to Deploy to GitHub Pages

This Space Rocket Builder game is ready to be deployed to GitHub Pages. Follow these steps:

### Option 1: Deploy from Main Branch Root (Recommended)

1. **Merge the feature branch to main:**
   ```bash
   git checkout main
   git merge claude/space-rocket-game-P3PHU
   git push origin main
   ```

2. **Configure GitHub Pages in the repository settings:**
   - Go to your repository on GitHub.com
   - Click **Settings** → **Pages** (on the left sidebar)
   - Under "Source", select **Deploy from a branch**
   - Choose branch: **main**
   - Choose folder: **/ (root)**
   - Click **Save**

3. Your game will be live at: `https://lochlan800.github.io/Buildspacerocket/`

### Option 2: Deploy from docs/ Folder

If you prefer to keep the game in a `docs/` subfolder:

1. Create a `docs/` folder and move files there
2. Follow the same GitHub Pages configuration but select `docs` folder instead of root
3. Game will be at: `https://lochlan800.github.io/Buildspacerocket/`

## Testing Locally

To test the game before deploying:

1. Start a local HTTP server:
   ```bash
   python3 -m http.server 8000
   ```

2. Open your browser to: `http://localhost:8000`

3. Click on `index.html` to play the game

## Live Game Features

Once deployed, the game will:
- ✅ Run completely in the browser (no backend needed)
- ✅ Save high scores to each player's device
- ✅ Work on desktop (arrow keys) and mobile (device tilt)
- ✅ Have smooth animations and responsive design

## Troubleshooting

**Game not loading?**
- Check that index.html is in the correct location
- Clear your browser cache (Ctrl+Shift+Delete)
- Check browser console for errors (F12 → Console tab)

**High scores not saving?**
- Ensure cookies/localStorage are enabled in your browser
- Try a different browser
- Check if you're in private/incognito mode (these don't save data)

---

Enjoy your space rocket game! 🚀
