# Hoyst POC

A two-page POC: the curated collection lands first, and the Aspire package detail opens from inside it.

## Local preview

Open `index.html` in a browser. (Some browsers block local font/script loads — if anything looks off, serve the folder instead: `python3 -m http.server` then visit `http://localhost:8000`.)

## Publish on GitHub Pages

1. Create a new repository on GitHub named **hoyst-poc** (public).
2. Upload everything in this folder to the repo root:
   - `index.html`
   - `The Aspire - Package Detail.html`
   - `assets/` (folder)
   - `image-slot.js`
   - `.image-slots.state.json` ← **important, holds the dropped images**

   ⚠️ Files starting with a dot are hidden by default on macOS / Linux Finder.
   In Finder press `⌘ + Shift + .` to reveal them before dragging, or use a tool
   that shows hidden files. If you forget this one, the page loads but every
   image placeholder will be empty.
3. In the repo, go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**.
5. Pick **Branch: main**, **Folder: / (root)**, click **Save**.
6. Wait ~1 minute. The site goes live at:

   ```
   https://<your-github-username>.github.io/hoyst-poc/
   ```

That URL is permanent and shareable with anyone.

## Structure

```
hoyst-poc/
├── index.html                          ← Hoyst Curated Collection (entry)
├── The Aspire - Package Detail.html    ← linked from inside the collection
├── image-slot.js
└── assets/
    ├── hoyst-logo.png
    ├── hoyst-logo-trim.png
    ├── hero-exterior.png
    ├── hero-exterior-2.png
    └── fonts/
```

The back-link inside the Aspire page returns to `index.html`.
