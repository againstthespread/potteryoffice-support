# PotteryOffice Support Website

Static, dependency-free GitHub Pages site for PotteryOffice support and privacy information.

## Before publishing

Replace `SUPPORT_EMAIL_TO_REPLACE` in `index.html` and `privacy.html` with the real support email address. Update both the visible address and its `mailto:` link. Do not publish while the placeholder remains.

The privacy policy currently reflects the reviewed iOS app source, package configuration, and privacy manifest as of November 16, 2026. Recheck it and the App Store Connect privacy answers against the final release build and any last-minute dependency or service changes.

## Preview locally

From this directory, run:

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000/>. The pages use relative links and work beneath the GitHub Pages project path.

## Publish with GitHub Pages

1. Replace the support email placeholder, then push the existing local commit to the remote main branch:

   ```sh
   git push -u origin main
   ```

2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main`, and choose `/(root)` as the folder. Save.
4. Wait for GitHub Pages to finish publishing, then check both URLs:
   - Support: <https://againstthespread.github.io/potteryoffice-support/>
   - Privacy: <https://againstthespread.github.io/potteryoffice-support/privacy.html>
5. Replace the app's Settings links only if the repository or Pages path changes. The current iOS Settings links already point to these URLs.

No build step, JavaScript, analytics, advertisements, tracking code, CDNs, or hosted fonts are used. Do not push or enable publishing until the support email placeholder is replaced and the final privacy statements are confirmed.
