# Personal App Showcase Website

A simple, responsive static website to showcase iOS apps. Starts with Walk Mate — Daily Route Generator.

## Structure

- `index.html`: Home page listing apps
- `apps/walkmate.html`: Detail page for Walk Mate
- `styles.css`: Shared styles
- `assets/app-icons/walkmate.png`: App icon copied from Xcode assets

## Deployment (GitHub Pages)

There are two common options. Pick one.

### Option A: Use `website/` folder on `main` branch
1. Commit and push the `website/` folder to your repository
2. Go to GitHub → Settings → Pages
3. Under "Source", choose `Deploy from a branch`
4. Select `Branch: main` and `Folder: /website`
5. Save; after a minute your site will be live at `https://<username>.github.io/<repo>/`

### Option B: Use a dedicated `gh-pages` branch
1. Create branch `gh-pages` with only the `website/` content
2. In Settings → Pages, select `Branch: gh-pages` and `Folder: / (root)`

## Local Preview

You can open `website/index.html` directly in a browser, or run a quick local server:

```bash
cd website
python3 -m http.server 8080
# Then open http://localhost:8080
```

## Add More Apps

1. Copy or export the app icon to `assets/app-icons/<appname>.png`
2. Create a new detail page under `apps/` (e.g., `myapp.html`)
3. Add a new card in `index.html` linking to the new detail page

## Custom Domain

If you use a custom domain, add a `CNAME` file to `website/` containing your domain, and configure DNS per GitHub Pages docs.
