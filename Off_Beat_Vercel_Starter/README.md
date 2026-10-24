# Off Beat — Vercel-ready editorial website

## Run locally

1. Install Node.js 20 or newer.
2. In this folder run `npm install` then `npm run dev`.
3. Open http://localhost:3000.

## Deploy on Vercel

1. Push this folder to a GitHub repository (or import the folder with Vercel CLI).
2. On vercel.com choose **Add New → Project**, import the repo.
3. Vercel should auto-detect **Next.js**. Keep the default build settings and click **Deploy**.
4. Add a custom domain in Vercel → Project Settings → Domains if needed.

## IMPORTANT: pre-launch work

- This is a **functional front-end prototype**, not a production newsroom. Stories and imagery are illustrative placeholders. Replace them with original, verified reporting and images for which Off Beat has usage rights.
- The sample content currently lives in `lib/stories.ts`; it is NOT connected to a CMS. For editorial publishing, integrate WordPress (REST API or WPGraphQL) or another CMS and implement draft/preview, scheduling, media credits and permissions.
- Add approved privacy/cookie policy, editorial/corrections policy, contact information, real social accounts, analytics consent, proper image alt text, and SEO/sitemap/robots configuration.
- Replace placeholder About and Contact text as appropriate. Review the logo's transparent background and crop for the header.
- Before public launch, complete accessibility, security and performance testing, and mobile QA.

## Project structure

- `app/page.tsx` homepage
- `app/[category]/page.tsx` section pages
- `app/story/[slug]/page.tsx` article template
- `app/search/page.tsx` client-side search across sample stories
- `components/` navigation, story cards, sharing
- `lib/stories.ts` demonstration content
- `public/offbeat-logo.png` supplied official logo
