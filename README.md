# DRIV3N website (privacy, terms, support)

Apple requires a working **Privacy Policy URL** and **Support URL** for App Store Connect. These four static pages are ready to host.

## 1. Fill in the placeholders
Search every .html file for `[` and replace each yellow-highlighted placeholder:
- `[YOUR NAME OR COMPANY]`, `[SUPPORT EMAIL]`, `[DATE]`, `[YEAR]`
- `[APP STORE LINK – add after approval]` in index.html (you can leave it until the app is live)
Then delete `class="ph"` from the tags you filled in (that class is only the yellow highlight).

## 2. Host it free (pick one)
- **GitHub Pages**: create a public repo, upload these files, Settings → Pages → Deploy from branch `main` / root. URL: `https://<username>.github.io/<repo>/privacy.html`
- **Netlify Drop**: drag this folder onto https://app.netlify.com/drop
- **Cloudflare Pages**: create project → Direct Upload → this folder.
Any https host works; a custom domain is optional.

## 3. Put the links in two places
1. **App Store Connect** → your app → App Information → Privacy Policy URL (privacy.html), and the version page → Support URL (support.html). Optionally put terms.html in the description or License Agreement.
2. **The app**: open `GiGTracker/AppLinks.swift` and paste the full `https://` addresses. The Settings → Legal & Support rows only appear once a valid https address is filled in.
