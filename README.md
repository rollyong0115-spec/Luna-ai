# Luna AI V2.1 — Mobile Data Edition

Upload **all five app files** to the root of your existing GitHub repository and replace old versions: `index.html`, `manifest.webmanifest`, `sw.js`, `icon-192.png`, `icon-512.png`. Keep your GitHub Pages branch on main / root.

## Test on Android
1. Open Luna in **Chrome**, refresh after deployment, and open Settings.
2. Set **Local model: Qwen 0.5B** and **Download storage: IndexedDB**. Save.
3. Tap **Download & Start Local AI**. Keep the browser in the foreground, preferably charging; mobile data works.
4. Wait until **Local ready** before chatting.
5. If an error appears, tap Retry. Try the 360M option as a diagnostic.

Note: switching from Cache API to IndexedDB does **not** migrate downloaded shards; files may redownload. Partially fetched shards may require starting over, and Android may close background browser tabs. The downloaded model is cached by the browser and is not an APK. Google Gemini API key is optional and intended only for private testing; do not publish it.
