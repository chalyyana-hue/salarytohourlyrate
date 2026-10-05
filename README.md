# SalaryToHourlyRate.com

Free pay calculators that turn salary into hourly pay, and hourly pay into yearly, monthly and weekly income.

**Live site:** https://salarytohourlyrate.com

## What is on the site

| Page | File |
| --- | --- |
| Salary to hourly calculator (home page) | `index.html` |
| Hourly to salary calculator | `hourly-to-salary-calculator.html` |
| 18 hourly rate pages ($12 to $80 an hour) | `12-dollars-an-hour-is-how-much-a-year.html` and similar |
| About, Privacy, Contact | `about.html`, `privacy.html`, `contact.html` |
| Custom 404 page | `404.html` |
| Old calculator address, redirects to home | `salary-to-hourly-calculator.html` |

Other files: `og-image.png` (social sharing image), `sitemap.xml`, `robots.txt`, `CNAME` (custom domain for GitHub Pages).

## How it is built

- Plain HTML, CSS and a little JavaScript. There is no build step and no framework to install.
- Each page is self-contained. The styles are inside the page, so there are no external stylesheets or scripts.
- The only outside request is the Plus Jakarta Sans font from Google Fonts.
- Calculators run in the visitor's browser. Nothing a visitor types is sent anywhere.
- Light mode is the default. The Dark/Light button saves the choice in the browser.

## Publish with GitHub Pages

1. Put all the files in the root of this repo (`index.html` must be at the top level).
2. Go to **Settings > Pages**. Under Source choose **Deploy from a branch**, then `main` and `/ (root)`.
3. Under **Custom domain**, enter `salarytohourlyrate.com` and save.
4. At the domain registrar, add four **A records** for the root domain (`@`):
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
5. Add a **CNAME** record for `www` that points to your GitHub username followed by `.github.io`.
6. When Pages shows "DNS check successful", tick **Enforce HTTPS**.

A domain can be attached to one repo at a time. Keep the `CNAME` file in the repo root, and do not delete it.

## Launch checklist

- [ ] Site opens at https://salarytohourlyrate.com with HTTPS
- [ ] `www` redirects to the main address
- [ ] Both calculators work on a phone
- [ ] Dark/Light button works
- [ ] A made-up address such as `/test` shows the 404 page
- [ ] Domain property added in Google Search Console
- [ ] `https://salarytohourlyrate.com/sitemap.xml` submitted

## Editing

- **Text and design:** edit the HTML files directly. Keep one `<h1>` per page and a unique `<title>` and meta description.
- **Domain change:** the address appears in canonical links, social tags, structured data, `sitemap.xml` and `robots.txt`. Update all of them together.
- **New hourly rate pages:** the numbers repeat many times on each page, so regenerate rate pages from the template instead of editing them by hand.
- **Contact email:** shown on `contact.html`.

## SEO notes

- Every page has a unique title, meta description, canonical link and social sharing tags.
- The calculator pages have structured data. The rate pages have breadcrumb data.
- New sites usually take months to rank. Watch Search Console for pages that are "Crawled, currently not indexed", and add useful content to those pages.
- Add affiliate links or ads only after the site has steady traffic. Update `privacy.html` when you do.

## Disclaimer

Results are estimates of gross pay before tax. They are for general information only and are not financial, tax or legal advice.
