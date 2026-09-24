# Stoked Distributors

Static site for Stoked Distributors, exclusive statewide distributor of Capital Call Vintners wines.

## Structure
- `index.html` — all page content
- `styles.css` — all styling (design tokens at top of file)
- `script.js` — mobile nav toggle + footer year
- `assets/images/` — logo, warehouse photos, wine case photo, Dendra Lee headshot
- `assets/docs/` — placeholder trade documents (see below)

## Placeholder content to replace before launch
- **Trade documents:** `assets/docs/current-price-list.txt`, `wholesale-order-form.txt`, `product-catalog.txt` are text placeholders. Replace each with the real PDF (same base filename, `.pdf` extension) and update the three `href` values in the "Trade documents" section of `index.html` to match.
- **Jared Stokes photo:** the Team section currently shows a placeholder tile for Jared. Add his photo to `assets/images/` and swap the placeholder `<div class="team-card__photo team-card__photo--placeholder">` block for an `<img>` tag (see Dendra's card for the pattern).
- **Warehouse photos and wine case photo:** currently stock/placeholder images. Swap in real photos of the Cumming, IA facility when available, keeping the same filenames or updating the `src` attributes.
- **Retail pallets photo** (`assets/images/retail-pallets.jpg`) is not currently used on the page; it was supplied as a placeholder but didn't fit the brand (visible pricing signage, unrelated products).

## Deploying to GitHub Pages
1. Create a new GitHub repository and push this folder's contents to the `main` branch.
2. In the repo settings, go to **Pages** and set the source to the `main` branch, root folder.
3. GitHub will publish the site at `https://<username>.github.io/<repo-name>/`.
4. For a custom domain, add a `CNAME` file to the repo root with the domain name, and point the domain's DNS at GitHub Pages per GitHub's custom domain docs.

No build step is required; this is a plain HTML/CSS/JS site.
