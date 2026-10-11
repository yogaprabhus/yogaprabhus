# Yogaprabhu S - Professional Portfolio

A responsive, framework-free portfolio website built with semantic HTML5, CSS3, and vanilla JavaScript.

## Files

- `index.html` - page content, SEO metadata, Open Graph data, and Person JSON-LD
- `styles.css` - responsive visual design and reduced-motion/accessibility styles
- `script.js` - accessible mobile navigation and dynamic footer year
- `assets/Yogaprabhu_S_Resume.pdf` - downloadable resume linked from the site
- `robots.txt` and `sitemap.xml` - starter files; update the domain before deployment

## Local preview

### Option A: Python
Run from this directory:

```bash
python -m http.server 8000
```

Open http://localhost:8000 in your browser.

### Option B: VS Code
Open the folder in VS Code and use a local static-server extension, or use the Python command above. Opening `index.html` directly also works for most features, but a local server is closer to production behavior.

## Personalize before publishing

1. Replace every `https://YOUR-DOMAIN.example/` occurrence in `index.html`, `robots.txt`, and `sitemap.xml` with the final HTTPS URL, including trailing slash conventions.
2. Confirm all achievement figures, role dates, course titles, and project descriptions are current.
3. The site intentionally has no portrait because no professional photo was provided. If desired, add one under `assets/`, use an optimized WebP or AVIF, set explicit width/height, and provide accurate descriptive alt text. Do not use a generated or stock person photo as if it were you.
4. Replace `assets/Yogaprabhu_S_Resume.pdf` with the latest reviewed PDF using the same filename, or update the download link in `index.html` if the file name changes.
5. Confirm permission to publish any employer-related descriptions. Do not publish confidential borrower data, internal templates, proprietary code, or non-public client information.
6. The IMA profile entry was visible in public indexing, but its exact program/qualification title was not confirmed. It is deliberately not represented as a completed qualification.

## Deploy using static hosting

Choose a static host such as GitHub Pages, Netlify, or Cloudflare Pages. Upload/push the entire folder while preserving the `assets` directory. No backend or build process is required. Configure the site to serve `index.html` at the root and force HTTPS. Confirm that the deployed site loads `styles.css`, `script.js`, the resume PDF, `robots.txt`, and `sitemap.xml` over the final domain.

## Custom domain checklist

- Register or use a domain you control.
- Add the domain in your hosting provider's site settings.
- Create the required DNS records exactly as given by the host (commonly A/AAAA or CNAME records).
- Wait for DNS/SSL provisioning and confirm the site loads at HTTPS without certificate warnings.
- Choose one canonical host (`https://example.com/` or `https://www.example.com/`) and redirect the other to it.
- Update the canonical URL, `og:url`, JSON-LD `url`, `robots.txt`, and `sitemap.xml` to the chosen domain.
- Test the resume download and LinkedIn/email links on desktop and mobile.

## Google Search Console checklist

1. Add the deployed domain as a Domain property in Google Search Console (DNS verification is generally the most complete option) or use a URL-prefix property.
2. Complete the verification steps shown by Google; do not commit verification secrets or private tokens to a public repository.
3. Submit `https://YOUR-FINAL-DOMAIN/sitemap.xml` in the Sitemaps report after replacing the placeholder domain.
4. Use URL Inspection for the homepage and request indexing when available.
5. Check the Page indexing and HTTPS reports periodically, and correct canonical/domain mismatches.
6. Keep the site useful and current. Google decides whether and when to crawl, index, and rank the page; this setup cannot guarantee indexing or rankings.

## Before go-live

- [ ] Domain placeholders replaced everywhere
- [ ] Resume PDF reviewed and downloads successfully
- [ ] LinkedIn profile and project links open the correct public pages
- [ ] Email link opens a mail client
- [ ] Current designation, dates, award names, and certification issue date reconfirmed
- [ ] No unpublished borrower/client information or confidential company material
- [ ] Confirm IMA program title/status before adding it
- [ ] Test keyboard navigation, skip link, mobile navigation, reduced-motion setting, and visible focus styles
- [ ] Test at narrow mobile, tablet, and desktop widths
- [ ] Inspect metadata, canonical, JSON-LD, `robots.txt`, and `sitemap.xml` after deployment
- [ ] Submit sitemap and inspect the page in Google Search Console
