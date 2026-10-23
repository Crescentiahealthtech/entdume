# Ponnaiah ENT & IVF Super Speciality Hospital

An ENT-first, responsive public website built with Astro. The experience is intentionally calm and clinical: warm neutrals, deep teal, accessible interaction patterns, clear service discovery and prominent appointment contact options. Fertility and IVF is presented as a secondary pathway so it can have a dedicated experience of its own.

## Run locally

Requirements: Node.js 20 LTS (or a compatible supported Node.js release) and npm.

~~~bash
npm install
npm run dev
~~~

## Production build

~~~bash
npm run build
npm run preview
~~~

Astro generates the static site in dist/. For Cloudflare Pages, the build command is npm run build and the output directory is dist.

## Automatic Cloudflare Pages deployment

The GitHub Actions workflow builds and deploys the site when a commit lands on main. Pull requests and pushes to other branches run the build check only. To enable production deployment, configure these values in the repository's GitHub settings under **Settings → Secrets and variables → Actions**:

**Repository secrets**
- CLOUDFLARE_API_TOKEN — an API token scoped to the correct Cloudflare account, with Account / Cloudflare Pages / Edit permission.
- CLOUDFLARE_ACCOUNT_ID — the Cloudflare account ID that owns the Pages project.

**Repository variable**
- CLOUDFLARE_PAGES_PROJECT_NAME — the exact Pages project name from Cloudflare Workers & Pages. This is the project name, not the custom domain.

The Cloudflare Pages project's configured production branch must be main. After saving the secret and variable, open **Actions → Build and deploy** and run the workflow against main once, or push/merge a new commit to main. A successful build without these deployment settings will not publish to the live site.

If Cloudflare Pages Git integration is already configured for this repository, confirm that it points to this repository and main as the production branch. If you choose this GitHub Actions workflow as the deployment source, consider disabling Cloudflare's automatic production-branch deployment after verifying the Actions-based deployment to avoid two competing production deploys.

## What's included

- Responsive homepage, desktop navigation and native mobile navigation.
- ENT service discovery, patient preparation guidance, visit details and FAQs.
- Tap-to-call appointment CTAs and Google Maps directions.
- Centralised contact details in src/data/clinic.ts.
- Page metadata, Open Graph tags, canonical URL and Hospital JSON-LD.
- Keyboard focus styling, skip link and reduced-motion support.
- No invented outcome statistics, patient testimonials, accreditations or clinical success rates.

## Before production

- Confirm the displayed hospital brand name, telephone numbers, address and listed hours with the hospital.
- Replace the stock hero image with approved hospital/clinician photography and ensure appropriate image rights.
- Confirm which services are currently offered and adapt the service descriptions accordingly.
- The appointment CTA calls reception; it is not an online booking system. Connect a verified booking workflow separately if needed.
- Ensure emergency information, privacy notice and any required legal or clinical notices are reviewed by the hospital.
- The listed hours and contact details are based on publicly available hospital contact information and should be confirmed before launch.

## Important

Website content is general information and does not replace an individual clinical assessment. Do not use the website to delay urgent or emergency care.
