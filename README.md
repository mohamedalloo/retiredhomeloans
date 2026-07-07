# RetiredHomeLoans

Flagship landing site for retiredhomeloans.com — retiree purchase lead generation, an AdaptLend service. Sibling site to RetiredRefi (same architecture, purchase-focused content, pine-green identity).

Static site: `index.html` + `styles.css` + `script.js`. No build step.

## Lead storage

Form inserts into the shared AdaptLend Supabase `leads` table (insert-only RLS, publishable key in `script.js`). Attribution: `matched_product` suffix `— RetiredHomeLoans`.

## Deploy

Same GitHub Pages pattern as adaptlend/retiredrefi: push to GitHub, enable Pages from `main` root (CNAME in place), then Namecheap DNS (4 GitHub A records + www CNAME) and Enforce HTTPS.

## Compliance notes

- Brand of the AdaptLend service (Honest Casa LLC, NMLS #1566096, DRE #02022356); footer discloses and links AdaptLend Terms/Privacy. Confirm DBA requirements with counsel before spending on traffic.
- No welcome email wired; success screen mentions email — wire a branded sender or soften the copy before heavy traffic.
- Calculator and examples are labeled illustrative — keep the "not a quote or commitment" footer language.
