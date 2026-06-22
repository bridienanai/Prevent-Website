# Prevent Biometrics — Website Handoff

A marketing-only site (no products / no checkout). Built to brand: navy + Signal Blue, 135° gradients, Inter, gradient stat tiles / cards / badges.

## How to preview
Double-click any `.dc.html` file — it opens directly in a browser. No build step, no server. `support.js` is the small runtime that renders them; keep it next to the HTML files.

## Pages
| File | Purpose |
|---|---|
| `Prevent Biometrics.dc.html` | Home (hero, as-featured-in, why it matters, how it works, validation, blog, newsroom, support, footer) |
| `Careers.dc.html` | Careers page (email-to-apply) |
| `blog-hae.dc.html` | Blog article — head acceleration exposure |
| `blog-fitting.dc.html` | Blog article — fitting the IMM |
| `blog-matchday.dc.html` | Blog article — match-day case study |

## Where the content lives
- **Copy / colors:** edit any visible text or single color directly in the OmniMonkey editor preview.
- **Blog cards + Newsroom list:** in `Prevent Biometrics.dc.html`, inside the `<script data-dc-script>` block — see the `blogPosts` and `pressReleases` arrays (each item is plain text fields + a link).
- **Links (Tweaks):** Portal → `portal.preventbiometrics.com`, Support → `support.preventbiometrics.com` (HubSpot help center). Editable in the Tweaks panel or the `portalUrl` / `helpUrl` props.
- **Images:** `assets/` (product + rugby photography) and `uploads/` (logos + press logos). Blog thumbnails are drag-and-drop slots — drop a new image on a card to replace it.

## Notes
- The four **Newsroom** links go to real, live articles (World Rugby, Cleveland Clinic, RPA, Sportsmith).
- The **Validation** section cites real peer-reviewed studies; the 0.97 / 0.98 CCC and 81.6% PPV figures come from the cited 2025 paper — confirm before publishing.
- Blog articles are **AI-assisted drafts** — review before publishing.

## Putting it in Shopify
1. Create the store; keep it marketing-only (no products, checkout off). Upgrade to **Shopify Plus** later — Settings → Plan — without rebuilding.
2. Pick a flexible theme (Impulse / Prestige, or free Dawn).
3. Rebuild the home page with theme sections (Image banner, Logo list, Multicolumn, Rich text, Blog posts); use **Custom Liquid** sections for the bespoke gradient tiles / validation cards — paste the markup + inline CSS from these files.
4. Content: Pages → Online Store ▸ Pages · Blog & News → Online Store ▸ Blog posts (two blogs: "Blog" and "Newsroom") · Images/PDFs → Content ▸ Files.
5. Navigation: header menu = Why / How / Validation / Blog / Newsroom / Support; Customer Portal + Support are external links.
6. Install the HubSpot app for lead capture; point the Support button at your HubSpot help center.
7. Point `preventbiometrics.com` at Shopify once validated (run in parallel first).
