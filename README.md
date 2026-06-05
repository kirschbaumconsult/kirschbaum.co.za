# kirschbaum.co.za

Static one-page site for Kirschbaum Software Consulting, served via GitHub Pages.

- `index.html` — the page
- `styles.css` / `tokens.css` — brand styles and design tokens
- `assets/` — favicon and app icons
- `CNAME` — custom apex domain (`kirschbaum.co.za`)

## Deploy

Pushing to `main` publishes automatically via GitHub Pages.

### DNS (apex via Route 53)

Point the apex `kirschbaum.co.za` at GitHub Pages with A/AAAA records:

```
A     185.199.108.153
A     185.199.109.153
A     185.199.110.153
A     185.199.111.153
AAAA  2606:50c0:8000::153
AAAA  2606:50c0:8001::153
AAAA  2606:50c0:8002::153
AAAA  2606:50c0:8003::153
```

Then enable **Enforce HTTPS** in the repo's Pages settings.
