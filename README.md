# Pavani A — Portfolio

A single-page static site (no build step). Deploy directly on Vercel.

## Deploy on Vercel — Option A: CLI (fastest)

```bash
npm i -g vercel
cd portfolio
vercel
```

Follow the prompts (log in, confirm project name). It deploys instantly and gives you a live URL.
Run `vercel --prod` afterward to push it to your permanent production URL.

## Deploy on Vercel — Option B: GitHub (recommended long-term)

1. Create a new GitHub repo, e.g. `portfolio`.
2. Push these files to it:
   ```bash
   git init
   git add .
   git commit -m "portfolio site"
   git branch -M main
   git remote add origin https://github.com/Pavani-A/portfolio.git
   git push -u origin main
   ```
3. Go to [vercel.com](https://vercel.com), sign in with GitHub, click **Add New → Project**, and import the `portfolio` repo.
4. Leave all settings as default (no framework, no build command needed — it's static HTML) and click **Deploy**.
5. Every future push to `main` auto-deploys.

## Custom domain

In the Vercel dashboard: Project → Settings → Domains → add your domain (or use the free `*.vercel.app` subdomain it gives you by default).

## Files

- `index.html` — the whole site (HTML, CSS, and JS inline, no dependencies to install)
- `vercel.json` — minor config (clean URLs)
