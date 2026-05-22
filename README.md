# testfblink

Website to be used for testing the editing of Facebook links for Composer.

## Setup for Facebook link previews

Facebook reads **Open Graph** tags in `index.html`. Before posting a link, replace `YOUR-VERIFIED-DOMAIN.com` in these meta tags with the **exact hostname** you verified in Facebook Business settings:

- `og:url` — the public URL of this page (e.g. `https://www.example.com/`)
- `og:image` and `twitter:image` — absolute URL to `images/squarelucky.png` on the same host

The image must be served over **HTTPS** and be publicly reachable (no auth).

After deploying, use the [Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/) to scrape the URL and refresh the cached preview.
