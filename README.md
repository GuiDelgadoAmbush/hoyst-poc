# Hoyst POC

A curated real estate collection experience — two pages built for sharing with clients.

## Pages

- **[Hoyst Curated Collection](index.html)** — The entry point. Three hand-picked residential packages presented by an advisor.
- **[The Aspire – Package Detail](The%20Aspire%20-%20Package%20Detail.html)** — Deep-dive on a single property with investment projections and editorial storytelling.

## Viewing locally

Open `index.html` in a browser. If fonts or images don't load, serve the folder instead:

```
python3 -m http.server
```

Then visit `http://localhost:8000`.

## Structure

```
├── index.html                          ← Curated Collection (entry)
├── The Aspire - Package Detail.html    ← linked from the collection
├── image-slot.js
├── .image-slots.state.json             ← holds property images (don't delete)
└── assets/
    ├── hoyst-logo.png
    ├── hoyst-logo-trim.png
    ├── hero-exterior.png
    └── hero-exterior-2.png
```
