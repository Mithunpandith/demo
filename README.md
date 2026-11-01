# Polished Detailing — Website Preview

Public demo: https://polished-detailing-sydney-preview.fairelk8193.chatgpt.site

This is a responsive design prototype for Polished Detailing, Sydney. It is not a WordPress theme or an Elementor import file. The existing WordPress website, hosting, DNS, blog, booking system, Stripe account and tracking have not been changed.

## Option 1: Just upload index.html and README.md

The separate `index.html` download is fully self-contained: all seven pages, styling, JavaScript and images are included. No assets folder, installation, build or internet connection is needed to preview it. Open the file in a browser, or upload it to GitHub.

1. Create a GitHub repository.
2. Choose **Add file → Upload files**.
3. Upload `index.html` and this `README.md` to the repository root.
4. Commit the files.
5. For GitHub Pages hosting, open **Settings → Pages** and select **Deploy from a branch → main → / (root)**, then save.
6. Open the Pages URL shown by GitHub once deployment finishes.

Navigation in this portable version uses hash URLs such as `#/car-detailing/`. That keeps every page working offline and under a GitHub repository subdirectory. It is a preview format, not the final SEO URL structure.

## Option 2: Upload the complete website ZIP

Extract `polished-detailing-github.zip` on your computer, then upload its **contents** to the repository root. Do not upload the ZIP alone if you want GitHub Pages to display the site. This version includes real page folders, `style.css`, `app.js`, `service-config.json`, and all WebP images. It supports repository subpaths without needing to edit the domain.

Do not replace its index.html with the standalone download unless you intentionally want the self-contained version.

## Included pages

| Page | Full-folder URL | Standalone navigation |
| --- | --- | --- |
| Home | `/` | `#/` |
| Car Detailing | `/car-detailing/` | `#/car-detailing/` |
| Ceramic Coating | `/ceramic-coating/` | `#/ceramic-coating/` |
| Contact Us | `/contact-us/` | `#/contact-us/` |
| FAQs | `/faqs/` | `#/faqs/` |
| Blog | `/blog/` | `#/blog/` |
| Booking Terms | `/booking-terms/` | `#/booking-terms/` |

The logo returns to Home; there is no separate Home menu item. All 11 blog article links preserve the original website URLs.

## Working preview interactions

- Responsive mobile navigation and fixed booking/call buttons.
- Interior, Exterior and Complete package selector by vehicle size.
- Ceramic prices by vehicle size, with an extensible protection-length model.
- Booking service selection, preferred date/time, suburb, review, back and close.
- Final booking links open the corresponding existing live booking pages.
- Before/after slider, searchable grouped FAQs and blog filtering.
- Contact quote form validates and prepares an email draft or copied request.

The prototype itself **does not charge deposits, reserve appointments, send confirmation emails or submit quote details to a server**. A user must complete any actual booking on the existing business website, or send the prepared email themselves.

## Content awaiting business approval

- Final detailing prices for medium/large vehicles.
- Final ceramic coating prices and future 7-year/10-year protection options.
- Verified Google review feed and review count. No individual testimonials were invented.
- Approved Booking Terms & Conditions wording.
- A verified ceramic coating before-and-after project.

The 5.0 rating and current advertised starting prices were taken from the existing business website. All imagery was reused from that website. Newly written page copy is draft copy for review.

## WordPress production handover

Implement the approved design on a staging copy first, preferably with a lightweight block theme or carefully scoped Elementor templates. Retain FluentBooking initially and test Stripe deposits, confirmation emails, timezone, terms links and Google Ads conversions before launch.

The existing detected GTM container is `GTM-WKN45QKL`; keep the WPCode installation as the single production container. The demo does not load tracking scripts. Preserve the live blog posts and their URLs, inventory the legacy URLs, and configure tested 301 redirects on the actual host. Known merges: `/services/` and `/specials-offers/` → `/car-detailing/`.

The demo deliberately remains **noindex** to avoid competing with the business's existing website. Public viewing does not imply search indexing. Canonicals reference the intended production domain. Change these only when the approved redesign is launched on the real business domain.

Before launch, test actual thank-you pages as noindex, payment and email behavior, review authenticity, crawlability, broken links, accessibility and mobile/desktop PageSpeed. No unmeasured PageSpeed scores are claimed.

## Editing the full-folder version

- Page text and markup: each page's `index.html`.
- Shared styles: `style.css`.
- Interactions: `app.js`.
- Approved pricing and future coating options: `service-config.json`.
- Images: `assets/`.

For local testing, serve the extracted directory with any static web server. Directly opening the multi-file version may restrict JSON fetching; the standalone version avoids that issue.
