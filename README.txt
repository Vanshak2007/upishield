UPISHIELD - HOW TO INSTALL (Android + Windows)

1. HOST THE FOLDER OVER HTTPS (required for camera and install)
   Easiest free options: Netlify Drop (app.netlify.com/drop), GitHub Pages, or Cloudflare Pages.
   Upload all files in this folder. You get an https:// link.
   (For testing on one PC only, http://localhost also works, e.g. "python -m http.server 8000".)

2. ANDROID
   Open the link in Chrome > menu > "Install app" (or the Install button in the app).
   For a real .apk/.aab: go to pwabuilder.com, paste your link, choose Android.

3. WINDOWS
   Open the link in Edge or Chrome > address bar install icon > Install.
   For an .msix package: pwabuilder.com > Windows.

4. REAL ANALYSIS
   - Works without any key: pixel forensics + OCR (Tesseract, needs internet on first use).
   - Best results: Settings > paste your Anthropic API key (console.anthropic.com).
     Claude then reads the receipt and checks it visually.
   - The key is stored on that device only. For an app you give to other people, do not
     ship your own key: put a small backend proxy in front of the API instead.
