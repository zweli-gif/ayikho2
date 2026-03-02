# Deploy to GitHub Pages (fix for 'Coming soon' screen)

You are seeing **Ayikho 2 — Coming soon...** because GitHub Pages is serving an old placeholder `index.html`.

This folder contains the working app in **two places**:
- `/index.html` (root)
- `/docs/index.html` (docs)

So it will work whether your Pages setting uses **/(root)** or **/docs**.

## Steps
1) Open your repo **ayikho2** on GitHub.
2) Upload **all files/folders** from this zip into the repo (root).
   - Important: `index.html` must be at the repo root (top level).
3) Commit changes.
4) Go to **Settings → Pages**:
   - Source: Deploy from a branch
   - Branch: `main`
   - Folder: choose **/(root)** (recommended)
   - If you prefer `/docs`, choose `/docs` (also works with this zip)
5) Wait for the Pages build (Actions tab), then hard refresh:
   - Mac: Cmd + Shift + R

## Quick check
When you open https://<username>.github.io/ayikho2/ you should see:
- Ayikho top bar
- Start / Modules / Data nav
