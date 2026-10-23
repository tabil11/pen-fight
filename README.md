# Pen Fight: Bench Edition (কলম যুদ্ধ)

The classic school-bench pen fight game for the browser. Flick your pen and knock the other one off the bench, without falling off yourself.

- **vs Computer** (Easy / Medium / Hard) or **2 Players** on the same phone
- 7 pens: Real Madrid, IEEE, IEEE Photonics Society, IEEE Computer Society, COMPASS, QPAIN, OMLET
- Works on phone and desktop, and runs offline once installed
- **Installable as an app** (PWA) from the website: Android/Chrome/Edge show an "Install app" button, and on iPhone you use Share → Add to Home Screen

## How to play
1. Touch your pen, drag back like a slingshot, and let go.
2. Flick near the end of the pen to spin it, or the middle to push it straight.
3. Knock the other pen off the bench. If your own pen falls, you lose the round.
4. The first player to win 3 rounds wins the match.

## Put it online with GitHub Pages
1. Create a new **public** repository on GitHub, for example `pen-fight`.
2. Upload every file in this folder: `index.html`, `manifest.webmanifest`, `sw.js` and the `icons/` folder.
   (Use "Add file → Upload files" on GitHub, or run `git push`.)
3. In the repository, open **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, then pick `main` and `/ (root)`, and save.
4. After a minute the game is live at `https://<your-username>.github.io/pen-fight/`.
5. Open that link on a phone. In Chrome, tap **Install app** (or ⋮ → Install app). On iPhone, open it in Safari and tap Share → **Add to Home Screen**.

## Updating
After you change a file, open `sw.js` and change `VERSION` (for example `penfight-v2`). This makes installed copies pick up the new version.

## Run locally
Open `index.html` directly in a browser. To test install and offline mode you need a local server instead:
```
python -m http.server 8000
```
Then open http://localhost:8000.
