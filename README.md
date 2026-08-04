# Green Oval Garage — Website

Website for Green Oval Garage, a Land Rover specialist repair shop in Winter Park, FL.

## Files

| File | Purpose |
|---|---|
| `index.html` | The entire website (all 3 pages: Home, Services, Contact) |
| `shop_video.mp4` | Hero + About section background video |
| `favicon.png` | Browser tab icon (also embedded in the HTML) |
| `apple-touch-icon.png` | iPhone home-screen icon (also embedded in the HTML) |

## How it works

- Single-page application — Home / Services / Contact are switched with JavaScript, no page reloads
- Contact form submits to a Google Apps Script that logs each request to a Google Sheet and emails the shop
- Everything except the video is self-contained inside `index.html`

## Making changes

1. Edit `index.html`
2. Commit and push to `main`
3. If Netlify is connected to this repo, it deploys automatically within ~1 minute

## Form backend

The contact form posts to a Google Apps Script Web App. To change where notifications go, edit the `to:` address in the Apps Script (not in this repo) and redeploy it as a new version. The script URL lives in `index.html` — search for `script.google.com` if it ever needs replacing.

## Local preview

Open the folder in VS Code and use the Live Server extension ("Go Live" button). Opening `index.html` directly by double-clicking will block the video from loading.
