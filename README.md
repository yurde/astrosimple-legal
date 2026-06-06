# Astrosimple marketing site

Static site for `https://astrosimple.app`. Hosted on Cloudflare Pages.

## Pages

- `/` — landing
- `/privacy/` — privacy policy
- `/terms/` — terms of service
- `/support/` — support page

## Source of truth

Legal copy lives in `docs/privacy-policy.md` and `docs/terms-of-service.md`. The HTML in `site/privacy/index.html` and `site/terms/index.html` is rendered by hand from those files. **When you change a markdown file, regenerate the matching HTML.**

## Deploy

Cloudflare Pages → connect repo → root directory `site/` → no build command → output directory `site` (or empty if root is set). See `docs/cloudflare-deploy-instructions.md`.

## Local preview

```sh
npx serve site
```
