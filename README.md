# Reithmeier Agency LLC — Website

A clean, professional **black & white** static website for **Reithmeier Agency LLC**, built to support TCPA / SMS messaging approval for an insurance agency. The structure mirrors a proven compliant layout and includes everything a lead vendor, dialer, or carrier reviewer typically looks for.

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Home — agency overview, approach, solutions, process, CTA (with SMS disclosure) |
| `quote.html` | Request a Quote — SMS consent language + quote-form embed slot |
| `privacy-policy.html` | Privacy Policy with TCPA & SMS consent + "mobile info not shared" language |
| `sms-terms.html` | SMS Terms & Conditions (opt-in, STOP/HELP, frequency, costs) |
| `sms-opt-in.html` | SMS Opt-In & Call-to-Action (CTA + sample messages for carrier review) |
| `help.html` | Help & Support (STOP/HELP, contact) |

Contact email: **Info@reithmeieragency.com**

## ⚠️ Placeholders to replace before going live

1. **Phone number** — currently `000-000-0000` / `tel:+10000000000` throughout (nav, hero, SMS opt-in, footer). Replace with the agency's real SMS-capable number.
2. **Quote form** — `quote.html` has a dashed placeholder panel where the form embed goes. Drop in the Reithmeier Agency form `<iframe>` (e.g. Jotform). The SMS consent checkbox language is already written.
3. **Logo** — `logo.svg` and `favicon.svg` are temporary black "RA" monograms. Replace with the agency's real logo (keep it ~square; PNG/SVG both fine).
4. **Custom domain** — no `CNAME` is set, so the site serves at the default GitHub Pages URL. Add a `CNAME` file with the domain (e.g. `www.reithmeieragency.com`) once DNS is pointed.

## Run locally

```bash
python3 -m http.server 8111
```

Then visit http://localhost:8111

## Hosting (GitHub Pages)

Push to a GitHub repo, then enable Pages: **Settings → Pages → Deploy from branch → `main` / `/root`**. The site is plain static HTML/CSS — no build step.

## Styling

Theme tokens (the black & white palette) live in `:root` at the top of `styles.css`. The accent is near-black (`--accent: #111111`); dark panels are near-black; surfaces are neutral white/gray.
