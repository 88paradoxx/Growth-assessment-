# Clinical Growth Assessor

A single-page pediatric growth assessment tool (WHO 2006 & IAP 2015 percentile modeling) with an interactive canvas-based growth chart. Pure static HTML/CSS/JS — no build step, no backend, no dependencies to install.

## Run locally

Just open `index.html` in a browser, or serve it:

```bash
npx serve .
```

## Deploy to Vercel

**Option A — CLI**
```bash
npm i -g vercel
vercel
```

**Option B — Dashboard**
1. Push this folder to a GitHub repo.
2. Go to [vercel.com/new](https://vercel.com/new) and import the repo.
3. Framework preset: **Other** (static site). No build command, no output directory needed — Vercel will serve `index.html` from the root automatically.
4. Deploy.

## Deploy to GitHub Pages

**Option A — Automatic (included workflow)**
1. Push this folder to a GitHub repo.
2. Go to **Settings → Pages → Build and deployment → Source**, select **GitHub Actions**.
3. Push to `main` — the included workflow (`.github/workflows/deploy-pages.yml`) builds and deploys automatically.

**Option B — Manual, no workflow**
1. Push this folder to a GitHub repo.
2. Go to **Settings → Pages → Build and deployment → Source**, select **Deploy from a branch**.
3. Choose branch `main`, folder `/ (root)`, save.
4. Your site will be live at `https://<username>.github.io/<repo-name>/`.

## Files

- `index.html` — the app itself
- `vercel.json` — headers/routing config for Vercel
- `package.json` — metadata + optional local dev script
- `.github/workflows/deploy-pages.yml` — GitHub Pages auto-deploy
