# Yemen FX — Next.js (App Router) + Tailwind
Ready to deploy to **Vercel**.

## Features
- USD/YER by region: **Sana'a (Old Notes)** & **Aden (New Notes)**
- SAR/YER derived from USD→SAR
- Converter between Sana'a ↔ Aden (via USD pivot)
- Auto-refresh every 5 minutes
- Optional `/api/proxy` route to bypass CORS, with 5-min cache

## Quick Start (Local)
```bash
npm install
npm run dev
```
Open http://localhost:3000

## Deploy to Vercel
1. Create a new Vercel project and import this folder/repo.
2. (Optional) Add Environment Variable: `NEXT_PUBLIC_PROXY=1` to use the built-in `/api/proxy` for CORS.
3. Deploy.

## Notes
- Data sources:
  - ACAPS YETI (USD/YER per region)
  - exchangerate.host (USD→SAR)
- If the ACAPS endpoint blocks browser requests via CORS, enable the proxy by setting `NEXT_PUBLIC_PROXY=1`.
