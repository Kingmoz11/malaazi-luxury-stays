# Malaazi Luxury Stays

A responsive, multi-page static website for Malaazi, a premium hospitality and lifestyle brand curating stays and experiences on Kenya's Coast.

## Pages

- Home (`index.html`)
- Collection (`collection.html`)
- Signature Experiences (`signature.html`)
- Executive Gatherings (`executive-gatherings.html`)
- Discover (`discover.html`)
- About (`about.html`)
- Contact (`contact.html`)

## Run locally

Because this is a static site, no build step is required. Open `index.html` in a browser, or use a local server:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## cPanel deployment

1. Log in to cPanel.
2. Open **File Manager** and select the domain's document root, usually `public_html`.
3. Upload the project files and folders, preserving the structure:
   - `index.html`
   - `collection.html`, `signature.html`, `executive-gatherings.html`, `discover.html`, `about.html`, `contact.html`
   - `css/`
   - `js/`
4. If uploading a ZIP, use **Extract** inside `public_html`, then move the contents out of any extra wrapper folder.
5. Confirm that `public_html/index.html` exists directly in the document root.
6. Visit your domain. Enable an SSL certificate in **SSL/TLS Status** or **Let's Encrypt** if your host provides it.

## Customization

- Replace the Unsplash URLs with licensed Malaazi photography in the HTML files.
- Update email addresses, phone numbers and social links in the footer/contact page.
- The contact form currently validates in the browser and displays a confirmation. To receive real messages, connect it to your host's PHP mail handler or a form service.

## Important

The image URLs are remote demo assets. For production, download properly licensed images into an `images/` directory and update the `src` and background URLs.
