# snowpack-hop-site

Landing, support and privacy pages for **Snowpack Hop**, a one-tap platformer for iPhone: Tuck the fox runs on his
own, and every snow critter he stomps packs into a block he can climb.

Live: https://nguyenvanlamm.github.io/snowpack-hop-site/ · [support](https://nguyenvanlamm.github.io/snowpack-hop-site/support.html) · [privacy](https://nguyenvanlamm.github.io/snowpack-hop-site/privacy.html)

Plain static HTML and CSS, no build step and no JavaScript. GitHub Pages serves the `main` branch root directly
(no GitHub Actions). Fredoka and Nunito are self-hosted (SIL OFL 1.1, licences in `assets/fonts/`), so the site makes
no third-party requests. Screenshots and the icon come from the game repo (`screenshots/`, `assets/icon/`).

The privacy page must match what the app does (no account, no analytics, progress and purchases stored on the device).
Update it together with the app.

Preview locally: `python3 -m http.server 8000` and open http://127.0.0.1:8000/.
