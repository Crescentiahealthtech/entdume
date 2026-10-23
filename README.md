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

Astro generates the static site in dist/. For Cloudflare Pages, use npm run build as the build command and dist as the output directory.

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
