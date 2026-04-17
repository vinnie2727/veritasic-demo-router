# veritasic-demo-router

Tiny Vercel project that owns **demo.veritasic.com** and proxies subpaths to other Vercel apps.

## Routes

| URL | Proxies to |
|---|---|
| `/equipment-risk-tower/...` | `https://REPLACE-WITH-YOUR-APP.vercel.app/equipment-risk-tower/...` |

## Setup

1. Edit `vercel.json` — replace `REPLACE-WITH-YOUR-APP.vercel.app` with the production `*.vercel.app` URL of the **equipment-risk-tower** project (Vercel → that project → Settings → Domains).
2. Push this folder to a GitHub repo.
3. Import the repo into Vercel as a new project (framework: **Other**, no build command).
4. Vercel → this project → **Settings → Domains** → add **demo.veritasic.com**.
5. Make sure DNS for `demo.veritasic.com` points to Vercel only (CNAME `cname.vercel-dns.com.`).
