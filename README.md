# From Code to UX — Interview-Ready

An interactive, single-page course for developers transitioning into UI/UX roles. Covers 8 modules of theory, quizzes, exercises, and interview prep, with progress saved locally in the browser.

## Deploy to GitHub Pages (free, ~5 minutes)

1. **Create a new repo** on GitHub (e.g. `ux-for-coders`). Don't initialize with a README (you already have one).

2. **Push this project** — from your terminal, inside this folder:
   ```bash
   git add .
   git commit -m "Initial course build"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/ux-for-coders.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to your repo → **Settings** → **Pages** (left sidebar)
   - Under "Build and deployment" → Source: **Deploy from a branch**
   - Branch: **main**, folder: **/ (root)**
   - Click **Save**

4. **Your course is live** in 1-2 minutes at:
   ```
   https://YOUR_USERNAME.github.io/ux-for-coders/
   ```

## Updating content later
Edit `index.html` directly (all module content lives in the `modules` array near the top of the `<script>` tag), then:
```bash
git add .
git commit -m "Update module content"
git push
```
GitHub Pages redeploys automatically within a minute or two.

## Notes
- Progress is saved via browser `localStorage` — it's per-device/per-browser, not synced across devices. Fine for personal use; if you want cross-device tracking or multiple learners, you'd need a backend (e.g. small database + auth), which is a bigger build.
- No build step, no dependencies — it's a single static HTML file, so it also works by just double-clicking `index.html` locally.
