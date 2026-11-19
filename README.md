# SS COSMETIC – static e-commerce site (no backend, no database)

Open `index.html` (or upload the folder to any static host: Netlify, GitHub Pages, Hostinger…).

## 1. Set your WhatsApp number & UPI ID  → `js/config.js`
    const STORE_WHATSAPP_NUMBER = "919876543210";   // country code + number, digits only
    const STORE_UPI_ID = "yourname@okbank";
Also edit store phone, email, address, delivery fee and free-delivery limit there.

## 2. Add / edit / remove products  → `js/products.js`
Copy any line inside `PRODUCTS`, change the values. Leave `image: ""` for auto artwork, or put your photo in
`assets/products/` and use `image: "assets/products/my-photo.jpg"` (extra gallery photos: `images: [...]`).
No limit on products. Discount % is calculated automatically.

## 3. Add a category
Add a line to `CATEGORIES` in `js/products.js`, then use its `slug` in products' `category`.

## Notes
- Edit testimonials in `index.html` (demo text) and policy pages (`privacy-policy.html`, `terms.html`, `shipping-policy.html`, `return-policy.html`) to match your business.
- After hosting, replace YOUR-DOMAIN.com in `robots.txt` and `sitemap.xml`.
- UPI payment is verified manually by you; orders are never auto-marked as paid.
