# Frost OS

A browser-based OS desktop with two proxy engines: **Scramjet** and **Ultraviolet**
(switch in the browser bar). Press **Ctrl+K** anywhere to open an app or any link.

## Run locally
    npm install
    npm start        # prints the address, e.g. http://localhost:8080

## Put it on GitHub, then host it
1. Create a GitHub repo and push this whole folder (node_modules is ignored).
2. Go to render.com, New > Web Service, pick your repo. It reads render.yaml
   (build: `npm install`, start: `npm start`). Free tier is fine.
3. Open the URL Render gives you. Done. (Replit can also import a GitHub repo.)

GitHub Pages / jsDelivr can't host this: the proxy needs the Node server
(Wisp websocket) and service-worker files, not just one HTML page.
The whole OS interface itself is one file: public/index.html.

## Credits & license
Built on Scramjet and Ultraviolet (Mercury Workshop / Titanium Network) and the
patterns in their AGPL-3.0 demo apps. If you make your site public, AGPL-3.0
asks you to make your source available too.
