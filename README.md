# MAST 2.0 — GitHub Pages Website

A lightweight, responsive static website for MAST / Tim Conley. No Wix branding, no paid hosting, and no build tools.

## Preview on your computer

Double-click `index.html`. For the best preview, use a small local server:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish with GitHub Pages

1. Sign in at GitHub and create a **public** repository.
2. Open the repository and choose **Add file → Upload files**.
3. Drag the **contents of this folder** into GitHub. Do not upload the ZIP itself.
4. Click **Commit changes**.
5. Open **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select **main** and **/(root)**, then click **Save**.
8. Wait 1–3 minutes. GitHub will show the website address.

## Connect mastmusic.net

The included `CNAME` file already contains `mastmusic.net`.

At your domain provider, add these DNS records:

| Type | Name | Value |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | YOUR-GITHUB-USERNAME.github.io |

Then return to **GitHub → Settings → Pages**, confirm `mastmusic.net` as the custom domain, and enable **Enforce HTTPS** when available.

## Required final edit: contact form

1. Create a free form at Formspree.
2. Copy its form ID.
3. Open `contact.html`.
4. Replace `YOUR_FORM_ID` with your actual ID.

## Change text, links or images

- Main pages are the `.html` files in the project root.
- Global design is in `assets/css/style.css`.
- Site behavior is in `assets/js/main.js`.
- Images are in `assets/images/`.
- Replace an image while keeping its filename to update it without touching the HTML.

## Important

The site uses Google Fonts. It will still work if Google Fonts are unavailable, but typography will fall back to Arial/sans-serif.
