# Barcelona Itinerary

A single-page, tab-based trip itinerary for Barcelona (Jun 30 – Jul 4, 2026).

## Deploy to Vercel

### Option A — Vercel website (easiest, no install needed)
1. Go to https://vercel.com and sign in (GitHub, GitLab, or email).
2. Click **Add New → Project**.
3. Choose **"Deploy without Git"** / drag-and-drop, then drag this whole folder
   (`barcelona-vercel/`, containing `index.html` and `vercel.json`) onto the page.
4. Click **Deploy**. Vercel will give you a live URL in under a minute,
   e.g. `https://barcelona-itinerary.vercel.app`.

### Option B — Vercel CLI
```bash
npm install -g vercel
cd barcelona-vercel
vercel
```
Follow the prompts (log in if needed, accept the defaults). It will print a live URL.
Run `vercel --prod` to push it to your permanent production URL instead of a preview link.

### Option C — GitHub + Vercel (best if you want to keep editing it later)
1. Create a new GitHub repo and push this folder to it.
2. In Vercel, click **Add New → Project**, then **Import** that GitHub repo.
3. Leave all settings as default (no framework, no build command needed — it's a static file) and click **Deploy**.
4. Every future push to the repo will auto-redeploy.

## Notes
- This is a single static `index.html` — no build step, no dependencies, no
  framework. Vercel will detect it as a static site automatically.
- `vercel.json` just disables trailing slashes / enables clean URLs; you can
  delete it and it'll still deploy fine.
- To use a custom domain, add it under Project → Settings → Domains once deployed.
