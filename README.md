# Verhaegh & Zn. Homepage

Static homepage for [verhaeghzn.nl](https://verhaeghzn.nl), deployable via GitHub Pages.

## Local preview

```bash
python3 -m http.server 8080
```

Open [http://localhost:8080](http://localhost:8080).

## GitHub Pages deployment

1. Push this repository to GitHub (e.g. `verhaeghzn/vzn-homepage` or the org repo).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
4. Select branch `main` (or `master`) and folder **`/ (root)`**.
5. Save. GitHub will publish the site within a few minutes.

The `CNAME` file configures the custom domain `verhaeghzn.nl`. In your DNS provider, add:

| Type  | Name | Value                    |
|-------|------|--------------------------|
| A     | @    | 185.199.108.153          |
| A     | @    | 185.199.109.153          |
| A     | @    | 185.199.110.153          |
| A     | @    | 185.199.111.153          |
| CNAME | www  | `<username>.github.io`   |

(Or use the four A records GitHub shows in your repo's Pages settings.)

## Structure

```
index.html          Main page
css/styles.css      Styles
js/main.js          Navigation & small enhancements
assets/favicon.svg  Favicon
CNAME               Custom domain
.nojekyll           Skip Jekyll processing
```

## License

© Verhaegh & Zn. All rights reserved.
