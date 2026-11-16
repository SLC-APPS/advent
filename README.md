# Advent 2026 — GitHub Pages installation

This package is ready to upload. No Node.js, build command, database or ChatGPT sign-in is required by the app.

1. Unzip this archive on your computer.
2. Create a GitHub repository for this Advent app, for example advent-2026.
3. Upload the extracted files and the fonts folder into the repository root. index.html must be at the root, alongside app.js and sw.js. Upload the contents, not the ZIP file itself.
4. In the repository open Settings → Pages.
5. Under Build and deployment choose Deploy from a branch, then main and / (root), and Save.
6. Wait for GitHub Pages to finish deployment. Open the website URL shown in Pages settings, normally https://YOUR-USERNAME.github.io/advent-2026/.
7. On your phone, open that HTTPS website. After the offline-ready message appears, all 26 days can be read offline. Use the browser's Add to Home Screen or Install option to install the PWA.

If your file picker hides .nojekyll, it can be added separately in GitHub with Add file → Create new file. Its contents can be empty. This is a plain static site; no Jekyll build is needed.

The app uses relative paths and supports a GitHub Pages repository subdirectory. Do not add the SEMPER development folder or a CNAME file from another project.

Features: Traditional/Simplified Chinese, Mandarin/Cantonese device text to speech, reading preferences, progress, and offline reading. Device speech requires a compatible browser and the chosen voice. Offline speech requires an installed voice. Progress stays in the browser on that device and website origin; it will not transfer from the private Sites preview.

For later app updates, increment VERSION in sw.js whenever cached application files change, then upload the changed files. Returning visitors can use the update prompt.

GitHub documentation:
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

Text attribution is retained under About → Sources and permissions. Font licensing is included in FONT-LICENSE.txt.
