# snowpack-hop-site

Landing, support and privacy pages for **Snowpack Hop**, a one-tap platformer for iPhone: Tuck the fox runs on his
own, and every snow critter he stomps packs into a block he can climb.

Live: https://nguyenvanlamm.github.io/snowpack-hop-site/ · [support](https://nguyenvanlamm.github.io/snowpack-hop-site/support.html) · [privacy](https://nguyenvanlamm.github.io/snowpack-hop-site/privacy.html)

Plain static HTML and CSS, no build step and no JavaScript. GitHub Pages serves the `main` branch root directly
(no GitHub Actions). Fredoka and Nunito are self-hosted (SIL OFL 1.1, licences in `assets/fonts/`), so the site makes
no third-party requests. Screenshots and the icon come from the game repo (`screenshots/`, `assets/icon/`).

The privacy page must match what the app does (no account, no analytics, progress and purchases stored on the device).
Update it together with the app.

Search and AI files: `sitemap.xml`, `robots.txt`, `llms.txt` and `llms-full.txt` at the root, and JSON-LD plus Open
Graph tags in each page's `<head>`. Crawlers read only https://nguyenvanlamm.github.io/robots.txt, so that root file
must also carry this site's `Sitemap:` line. `assets/img/og.png` (1200x630) is the share card, composed from the app
icon and the game screenshot. When the game reaches the App Store, add the store link, update "Coming soon" in the
pages, `llms.txt`, `llms-full.txt` and the JSON-LD, and keep `llms-full.txt` in step with any page text change.

Preview locally: `python3 -m http.server 8000` and open http://127.0.0.1:8000/.
