# FORA Partners website

One-page website in English, German and Hungarian. Plain HTML, no build step.

## Files
- `index.html` – the whole site (text, design, language switch, contact form, legal pages)
- `favicon-32.png`, `apple-touch-icon.png` – browser and phone icons
- `share-image.png` – the preview picture shown when the link is shared (LinkedIn, WhatsApp)
- `fonts/` – the Plus Jakarta Sans font, served from the site itself (no Google connection)
- `logo/` – logo PNG and SVG files (light background, dark background, icon only)

## Publish with GitHub Pages
1. Create a new repository on GitHub (for example `fora-partners`).
2. Upload all files from this folder (Add file → Upload files), including `.nojekyll`.
3. Go to Settings → Pages, set Source to "Deploy from a branch", branch `main`, folder `/ (root)`, and save.
4. After a minute the site is live at `https://<your-username>.github.io/fora-partners/`.
5. Own domain: in Settings → Pages → Custom domain enter `forapartners.eu`, then add the DNS records GitHub shows at your domain provider (four A records for `forapartners.eu` and a CNAME for `www` pointing to `<your-username>.github.io`). Tick "Enforce HTTPS" once it is available.

## Contact form
Requests are sent by Web3Forms to the email address the access key was created for.
The key is in `index.html` (`const WEB3FORMS_KEY`). Web3Forms keys are meant to be public.

## Later changes
If you get a VAT number (UID) or register in the Firmenbuch, add it to the Imprint in `index.html` (all three languages).
