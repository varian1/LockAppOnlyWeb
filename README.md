# TapLock website (privacy policy + app-ads.txt)

Static files for the developer website. Not part of the app build.

| File | Purpose |
|---|---|
| `privacy.html` | Privacy policy. Its URL goes into AdMob (GDPR message), Google Play (App content → Privacy policy) and `EXPO_PUBLIC_PRIVACY_POLICY_URL`. |
| `app-ads.txt` | Authorizes Google to sell ads in the app. Must be at the **root** of the domain set as "Website" in the Play Store listing. Already contains this app's AdMob publisher ID. |
| `index.html`, `style.css` | Landing page and shared styles. |

## Before uploading

The developer name and contact email are filled in. If the app's final name changes from `TapLock`, update it in `privacy.html` and `index.html`. Keep the developer name the same as on Google Play.

## Hosting on GitHub Pages

`app-ads.txt` must be at the domain root, so use a **user site** (`<username>.github.io`), not a project page (`<username>.github.io/<repo>/`).

1. On GitHub, create a **public** repository named exactly `<username>.github.io`.
2. Upload the four files from this folder (Add file → Upload files), then commit.
3. Settings → Pages: Source = "Deploy from a branch", Branch = `main`, folder `/ (root)`.
4. After a minute, check:
   - `https://<username>.github.io/privacy.html`
   - `https://<username>.github.io/app-ads.txt`
5. Use `https://<username>.github.io` as the **Website** in the Play Console store listing, and the `privacy.html` URL as the privacy policy everywhere.
