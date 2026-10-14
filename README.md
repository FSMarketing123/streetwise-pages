# StreetWise landing pages

The collateral libraries embedded on https://streetwise.franklinst.com/, published with GitHub Pages.

| Page | Live URL (paste into the Wix HTML block → Website Address) | Packages |
|---|---|---|
| Capital Markets | https://fsmarketing123.github.io/streetwise-pages/capital-markets/ | `capital-markets/items.json` |
| Leasing | https://fsmarketing123.github.io/streetwise-pages/leasing/ | `leasing/items.json` |
| Management Services | https://fsmarketing123.github.io/streetwise-pages/management/ | `management/items.json` |
| Insurance Services | https://fsmarketing123.github.io/streetwise-pages/insurance/ | `insurance/items.json` |

## Adding packages

Add one line per package to that page's `items.json` and push. The live site picks it up within a few minutes — nothing changes in Wix.

```json
{"t": "Title", "s": "Brochures & Decks", "type": "Brochure", "prop": "Retail", "mkt": "Tampa, FL", "url": "https://publuu.com/flip-book/1098962/<id>", "img": "https://47gp61txie.execute-api.us-east-2.amazonaws.com/share/1098962/<id>", "des": "Designer Name"}
```

- `s` must match one of the page's section names (see `SECTIONS` in that page's `index.html`). Leasing has no `s`; it groups by `type` and also uses `tier` (1–3).
- `url` / `img` use the Publuu flipbook id. Leave `url` empty to show an "Awaiting file" placeholder.
- Optional: `"star": true` marks a package as featured.
