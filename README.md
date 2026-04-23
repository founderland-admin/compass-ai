# Compass AI — Investor Readiness

A single-page site for Compass AI.

## Deploying to GitHub Pages

You don't need the command line — everything can be done on github.com.

### 1. Create a new repository
1. Go to https://github.com/new
2. Name it something like `compass-ai` (this will be part of your live URL).
3. Set it to **Public** (GitHub Pages requires Public on free accounts).
4. Check **"Add a README file"** is UNchecked (we already have one).
5. Click **Create repository**.

### 2. Upload the files
1. On the empty repo page, click **"uploading an existing file"** (the link is in the quick-setup box).
2. Drag both `index.html` and `README.md` into the upload area.
3. Scroll down and click **Commit changes**.

### 3. Turn on GitHub Pages
1. In your repo, click **Settings** (top nav).
2. In the left sidebar, click **Pages**.
3. Under **Source**, select **Deploy from a branch**.
4. Under **Branch**, pick `main` and `/ (root)`, then click **Save**.
5. Wait 30–60 seconds. Refresh the Pages settings page — you'll see a URL like:
   `https://<your-username>.github.io/compass-ai/`

That's your live site.

## Editing the page

### Option A — Edit directly on GitHub (easiest)
1. Open `index.html` in your repo.
2. Click the pencil icon (✏️) in the top-right of the file view.
3. Make your edits.
4. Scroll down, write a short commit message (e.g., "Update headline"), and click **Commit changes**.
5. Your live site will update in ~30 seconds.

### Option B — Edit locally
1. Clone the repo: `git clone https://github.com/<your-username>/compass-ai.git`
2. Open `index.html` in any editor (VS Code is great and free).
3. Commit and push your changes back up:
   ```
   git add index.html
   git commit -m "Update headline"
   git push
   ```

## Notes

- **Custom font:** The original HTML references a local font file `uploads/Hanson-Bold.ttf` for the display headings. Since that file wasn't included, the browser will quietly fall back to Helvetica Neue (the CSS already handles this). If you want to restore the custom display font, upload `Hanson-Bold.ttf` to your repo and update the CSS path on line 12 of `index.html` from `url('uploads/Hanson-Bold.ttf')` to `url('Hanson-Bold.ttf')`.
- **Custom domain:** If you want a custom URL (e.g., `compass.yourdomain.com`), you can add it under Settings → Pages → Custom domain after your site is live.
