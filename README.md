# ControlMe AI — iPhone PWA

This is a phone-first, installable web app for recovery support, mood check-ins, an urge-reset timer, habit tracking, and data export.

## Important scope
- It is a Progressive Web App (PWA), not a native iOS `.ipa`.
- It can be installed from Safari on an iPhone after it is hosted over HTTPS.
- The “coach” is built-in supportive logic, not a live generative AI service. No API key or account is needed.
- Entries are stored in browser local storage on the device. They are not synced to a server. Clearing Safari website data may erase them; use Export periodically.
- It does not block websites. iOS Screen Time / Family Controls blocking requires a native app and Apple's required entitlements.

## Deploy using only your iPhone (GitHub Pages)
1. In Safari, sign in or create a GitHub account.
2. Create a new public repository, e.g. `controlme-ai`.
3. Upload all files in this project (index.html, manifest.json, sw.js, icon-192.png, icon-512.png). GitHub mobile website may offer **Add file → Upload files**.
4. In the repository, open **Settings → Pages**.
5. Under build/deployment, select **Deploy from a branch**, choose `main` and `/ (root)`, then Save.
6. Wait for the Pages URL to appear. Open that HTTPS URL in Safari on your iPhone.
7. Tap Share → **Add to Home Screen** → enable **Open as Web App** if shown → Add.
8. Launch ControlMe from the new Home Screen icon.

## Local testing
A PWA service worker needs HTTPS or localhost. For a simple preview, open `index.html` in a browser; tracking features work, but installation/offline caching may not.

## Privacy
Do not enter identifying or highly sensitive information. Local browser storage is not a substitute for secure medical-record storage. Exported JSON files are unencrypted; store them carefully.

## Support note
The app is a self-help tool, not therapy or emergency care. If pornography feels uncontrollable and impacts work or relationships, consider a licensed mental-health professional.
