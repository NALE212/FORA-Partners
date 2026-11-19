# FORA Partners website

One-page website in English, German and Hungarian (navy, warm white and champagne gold). Plain HTML, no build step.

## Files
- `index.html` – the home page (all sections and the contact form)
- `imprint.html`, `privacy.html` – the legal pages, in all three languages
- `i18n.js` – the German and Hungarian texts and the language switch
- `assets/` – the layout, styles and small scripts the pages use
- `fonts/` – Hanken Grotesk (text) and Plus Jakarta Sans (logo), served from the site itself (no Google connection)
- `favicon-32.png`, `apple-touch-icon.png` – browser and phone icons
- `share.jpg` – the preview picture shown when the link is shared (LinkedIn, WhatsApp)
- `logo/` – logo PNG and SVG files (light background, dark background, icon only)

## Publish with GitHub Pages
1. Create a new repository on GitHub (for example `fora-partners`), or open the existing one.
2. Upload everything from this folder (Add file → Upload files). Open the `fora-partners` folder on your computer, select ALL items inside it (Ctrl+A / Cmd+A), and drag them onto the GitHub upload page together, so the `assets`, `fonts` and `logo` folders go up with their contents. GitHub only keeps folders that are dragged in this way; the "choose your files" button cannot upload folders. Then check that the repository shows an `assets` folder next to `index.html`. When replacing the old site, delete the old `share-image.png`.
3. Go to Settings → Pages, set Source to "Deploy from a branch", branch `main`, folder `/ (root)`, and save.
4. After a minute the site is live at `https://<your-username>.github.io/fora-partners/`.
5. Own domain: in Settings → Pages → Custom domain enter `forapartners.eu`, then add the DNS records GitHub shows at your domain provider (four A records for `forapartners.eu` and a CNAME for `www` pointing to `<your-username>.github.io`). Tick "Enforce HTTPS" once it is available.

## Contact form
Requests are sent by Web3Forms to the email address the access key was created for.
The key is in `index.html` (the hidden `access_key` field in the form). Web3Forms keys are meant to be public.

## Later changes
If you get a VAT number (UID) or register in the Firmenbuch, add it to `imprint.html` (all three language blocks).
To change a text, edit it in `index.html` and its German and Hungarian lines in `i18n.js`.
