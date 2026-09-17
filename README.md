# AbSure Biosciences Website

Static responsive website starter for AbSure Biosciences.

## Run locally
Double-click `index.html`, or use VS Code Live Server.

Recommended:
1. Open this folder in VS Code.
2. Install the Live Server extension.
3. Right-click `index.html`.
4. Choose **Open with Live Server**.

## Before production
- Replace placeholder product records in `js/products.js` with the real catalogue.
- Replace placeholder contact details with verified company details.
- Connect `contact.html` to your email/form backend.
- Add approved AbSure logo/product images to `assets/`.
- Add privacy policy, terms and regulatory/company information.
- Test all links and forms.

## Deployment
This is a static site and can be deployed to Firebase Hosting, Netlify, Vercel, GitHub Pages, or standard cPanel hosting.

For Firebase Hosting:
1. Install Node.js LTS.
2. In PowerShell, open this folder.
3. Run `npm install -g firebase-tools`
4. Run `firebase login`
5. Run `firebase init hosting`
6. Choose/create your Firebase project.
7. Set the public directory to `.` (the current folder).
8. Configure as a single-page app: No.
9. Do not overwrite `index.html`.
10. Run `firebase deploy`

For an existing domain such as absurebiosciences.com, update the DNS records in your domain/DNS provider according to the hosting provider's instructions.

## Added product page
`product-niv-g.html` is the supplied AbSure Nipah Virus Glycoprotein (NiV-G) page, integrated into the catalogue.

Place the approved product assets in:
`assets/images/`
- `absure-logo.png`
- `make-in-india.png`
- `product-vial.png`
- `fig1-sds-wb.png`
- `fig2-native-sec.png`
- `fig3-stability.png`
- `fig4-elisa.png`

Place the real CoA at:
`documents/NiV-G-CoA.pdf`

The page currently shows clear placeholders when image files have not yet been added.


## Catalogue status
The catalogue has been converted to a real-product-first structure. The current catalogue record is the supplied Nipah Virus Glycoprotein (NiV-G ectodomain) product page. Do not add unverified product specifications; add new products only from approved AbSure product data.


## Current placeholder assets
- `assets/images/absure-logo-placeholder.svg` — replace with the approved AbSure logo.
- `assets/images/make-in-india-placeholder.svg` — replace with the approved Make in India artwork.
- `assets/images/product-vial-placeholder.svg` and `figure-placeholder.svg` — replace with approved NiV-G product/characterization images.
- `documents/ABS-RP-NIVG-001-DUMMY-CoA.pdf` and `ABS-RP-NIVG-001-DUMMY-Datasheet.pdf` are website-testing documents only and must be replaced before public release.
- The catalogue contains one real NiV-G record and two clearly labelled dummy records ready to be replaced one by one.

## Logo placement
For the real AbSure logo to appear throughout the site, place your approved logo image at:
`assets/images/absure-logo.png`
PNG with a transparent background is recommended. The site will automatically fall back to `absure-logo-placeholder.svg` if the PNG is missing.


## Product-by-product organization
Each product has an independent page at `products/<CATALOGUE-CODE>/index.html`. Product-specific images and documents belong under `assets/products/<CATALOGUE-CODE>/`. Branding lives under `assets/branding/`.

Current catalogue: one real NiV-G product plus four clearly marked placeholder library products from the supplied reference image.


## v6 image rules
- Company and Make in India logos: SVG in `assets/branding/`.
- All product photography and scientific figures: PNG in `assets/products/<CATALOGUE-CODE>/images/`.
- Replace the PNG placeholders with your actual files using the same filenames.
- NiV-G currently expects `product.png`, `fig1.png`, `fig2.png`, `fig3.png`, `fig4.png`.
