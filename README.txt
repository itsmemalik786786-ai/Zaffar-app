ZAFFAR Android/PWA package

Files:
- index.html: your original app with PWA manifest + service worker registration added
- manifest.webmanifest: install metadata and app icons
- sw.js: caches the local app shell for repeat visits
- icons/: 192px and 512px launcher icons

IMPORTANT:
1. Upload the contents of this folder to an HTTPS host (for example, a GitHub Pages site).
2. Open the hosted URL in Chrome on Android and test it.
3. For an Android APK, use https://www.pwabuilder.com with the hosted HTTPS URL and choose the Android package option.
4. Keep the signing key and credentials safe if you generate a signed package.

Limitations in the current HTML:
- Tailwind CSS and Google Fonts are loaded from external CDNs, so the first load and some styling still need internet.
- Notification settings currently use browser Notification APIs and an in-page timer; they are not guaranteed to fire when the app is closed or the phone has killed the page.
- The mentor responses are local scripted responses, not a connected live AI model.
- User progress is stored in browser localStorage. Test backup/export before switching browsers or reinstalling.

This package is a prepared PWA source project, NOT an APK. PWABuilder requires a publicly hosted HTTPS URL before Android packaging.
