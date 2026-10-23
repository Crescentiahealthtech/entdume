# Ponnaiah ENT & IVF Super Speciality Hospital — Astro flagship

## Run locally
Requirements: Node.js 20 LTS or a compatible Node.js release and npm.

```bash
npm install
npm run dev
```

## Production build
```bash
npm run build
npm run preview
```

The static production output is generated in `dist/`. Deploy that directory to a static host (Cloudflare Pages, Netlify, or any static web server). For Cloudflare Pages, use build command `npm run build` and output directory `dist`.

## Before publishing
- Verify the hospital's actual phone number and WhatsApp number in `src/data/clinicalData.ts`. The values in the supplied source may be placeholders.
- Verify every doctor credential, procedure, outcome metric, success rate, accreditation, and laboratory specification with the hospital. Do not publish unverified clinical or success-rate claims.
- The acoustic tone demo is educational only; it is not calibrated audiometry and must not be represented as a diagnostic test. Keep volume low and stop if uncomfortable.
- Configure a real consultation/booking backend before treating the consultation UI as a live booking system.

## Included
Astro configuration, Tailwind configuration, global styles, structured clinical data, 3D hero sculpture, acoustic tone studio, 3D clinical node viewer, consultation drawer, base layout, navigation, and homepage.
