# Hosting the privacy policy (GitHub Pages, free)

1. In `index.html`, replace every `[SUPPORT EMAIL]` and `[DATE]`.
2. On github.com, create a **public** repo, e.g. `upward-app`.
3. Upload `index.html` (plus `app-ads.txt` once you have your AdMob publisher id:
   `google.com, pub-XXXXXXXXXXXXXXXX, DIRECT, f08c47fec0942fa0`).
4. Repo **Settings → Pages → Source: Deploy from a branch → `main` / root → Save**.
5. After about a minute the page is live at `https://<your-username>.github.io/upward-app/`.

Use that URL for `privacyPolicyUrl` in `src/config/brand.js`, for the Play Console
privacy policy field, and as the website in the store listing.

> `app-ads.txt` only works at the **root** of a domain. A project page like
> `…github.io/upward-app/` doesn't count, so name the repo
> `<your-username>.github.io` instead. The site then lives at
> `https://<your-username>.github.io/`, which works for both files.

Keep this page in sync with `docs/PRIVACY_POLICY.md` when data practices change.
