# Luna AI V2 — GitHub Pages

Upload the following files into the root of your `Luna-ai` GitHub repository:
- index.html
- manifest.webmanifest
- sw.js
- icon-192.png
- icon-512.png

Keep your existing GitHub Pages deployment from the `main` branch and root. Wait for deployment, then open https://rollyong0115-spec.github.io/Luna-ai/ and refresh.

Open in recent Chrome on Android. Tap **Check WebGPU**, then **Download & Start Local AI**. This can take several minutes and a substantial download; use Wi-Fi and keep Luna in the foreground. First choice is a Qwen 1.5B preset if present in WebLLM; otherwise it chooses a Llama 1B or SmolLM fallback. Open settings to select a lighter model, or select Gemini mode and enter your own API key.

Local mode does not send chat messages to an inference API, although model files and JavaScript are downloaded from third-party hosts. Hybrid mode sends chat content to Gemini only when local inference fails and you have configured a key. The browser may use online speech recognition even when local AI is running. Key storage in localStorage is only for personal testing, not secure public deployment. A real APK requires a separate Android build; Chrome install is a PWA, not an APK.

WebLLM: https://github.com/mlc-ai/web-llm
