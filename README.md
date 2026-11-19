# ARTFLOW — bilingual storefront

A responsive static website built around the supplied ARTFLOW artwork library and brand brief.

## Open locally

Because the product catalogue is loaded from `products.json`, run the project through a local web server rather than opening `index.html` directly:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000` from this folder.

## Publish

Upload the complete contents of this folder to GitHub Pages, Netlify, or another static hosting provider. Keep the `assets/` folder and `products.json` beside `index.html`.

## Activate WhatsApp ordering

Open `config.js` and set your WhatsApp Business number, including country code, with digits only. For Morocco, use the `212` country prefix and omit `+`, spaces, and dashes:

```js
window.ARTFLOW_CONFIG = {
  whatsappNumber: '212XXXXXXXXX',
  currency: 'DH'
};
```

The number is intentionally blank because it was not provided in the brief. Product orders, custom requests, and artwork-composition requests are wired to WhatsApp once this is set.

## Included features

- French / Arabic language switch with RTL layout
- Hero and homepage content based on the supplied emotional brand direction
- 6 official categories and 4 editorial collections
- Best-seller cards in the requested 4:6 portrait ratio on the homepage
- Full catalogue with category filters, search, and sorting
- Favorites saved in the visitor's browser
- Artwork pairing shortlist (up to 3 works)
- Product detail modal with the three supplied sizes and prices
- WhatsApp order and custom-request flows
- Optimized WebP versions of the supplied artwork images

## Notes

- Artwork titles are derived from the supplied filenames. Generic filenames such as `Artboard` receive a simple category-based title.
- The three supplied prices are shown as size options: 60 × 40 cm — 230 DH; 80 × 60 cm — 280 DH; 85 × 110 cm — 342 DH.
- No delivery, guarantee, material, or customer-review claims have been invented.
