Homework App PWA - Storage Only Version

What changed:
- Adding homework no longer downloads index.html.
- Homework is saved inside the installed PWA/browser storage.
- Use Export backup / Import backup for moving homework between devices or making a backup.

How to test:
1. Serve this folder from a local web server or upload it to hosting.
2. Open the site in Chrome/Edge/Android browser.
3. Install using "Add to Home Screen".
4. Add homework and confirm no index.html download happens.

Important:
Service workers do not work reliably by opening index.html directly from file://.
Use a server such as:
  python -m http.server 8080
Then open:
  http://localhost:8080
