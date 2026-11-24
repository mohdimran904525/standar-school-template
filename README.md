# Kindergarten school template · React
An independent React + Vite recreation of the KidsCool reference homepage. The landing page retains the reference section order, typography settings, layout rules and local artwork. It does not require WordPress, Elementor, or a WordPress database.

## Run on your machine
Use Node.js 20.19+ or 22.12+.
```sh
npm ci
npm run dev
```
`npm run build` generates `dist/`. `npm run preview` serves the built output locally.

## Rebrand
- Edit `src/brand.js` for the school name, phone, email, logos, theme CSS variables and shared image overrides. The initial number and email are the reference's demo text with no call or mail action. Use the correct Justdial listing when one is available.
- Add your original photos to `public/assets/media/`. Use `brand.images` to replace a picture in multiple sections, or overwrite its file after keeping a backup. The same local path is reused wherever that picture appears.
- To set a palette, fill in `brand.palette` using variables such as `--wdtPrimaryColor`, `--wdtSecondaryColor`, and `--wdtTertiaryColor`. Inspect `public/assets/reference.css` for the reference's Elementor color variables too. The starter leaves them unchanged.
- Edit the named HTML section fragments in `src/reference/` for headings and body copy. `src/main.jsx` uses React to assemble header, homepage, footer and dialogs. Carousel and reveal behavior is in `src/carousel.js`; homepage interaction wiring is in `src/site-interactions.js`.
- Newsletter forms are local demos. Shop, LMS, other WordPress inner pages and any CMS, checkout or email service are not implemented in this homepage starter. Some original links are retained as references. Video loads the third-party player only when opened.
- The artwork is packaged locally. Google Fonts CSS is requested for the reference typefaces and the page has a system-font fallback. `asset-sources.json` records the original artwork locations. Replace reference branding and use graphics you have rights to when preparing a client deployment.

Reference: https://wdtkidscool.wpenginepowered.com/
