# samejima.art

An ambient collage site celebrating Samejima Mamimi. The page is a single static document (`index.html`) that loads a curated data file and arranges each piece of art into a playful grid with filtering, tag search, and a lightweight modal viewer.

> **Note:** The sample artwork entries ship with placeholder image URLs so that the layout renders without redistributing copyrighted work. Swap the URLs with links to your own hosted fanart or scans.

## Getting started

```bash
# from repo root
npx serve .
# …or use any static server you like
```

Then open the printed URL (usually `http://localhost:3000`) to browse the collage.

## Curating the gallery

All gallery metadata lives in `assets/data/artworks.js`. Each entry looks like this:

```js
{
  id: "vespa-dawn",          // unique slug
  title: "Vespa Dawn",
  artist: "kana *",
  type: "fanart",            // or "official"
  favorite: true,            // toggles the Favorites filter
  imageUrl: "https://…",     // link to hosted image
  alt: "Accessible description for screen readers",
  sourceLabel: "Pixiv drop",
  sourceUrl: "https://…",    // where the art lives
  tags: ["vespa", "pink"]    // used for filtering and the tag cloud
}
```

Add as many entries as you like—the grid is responsive and auto-fills. When you add new tags, they appear in the tag cloud automatically.

## Customizing the vibe

- Colors, typography, and layout live in `assets/css/main.css`.
- Grid behavior is defined under the `.collage-grid` and `.collage-card` rules.
- Interaction logic (filters, modal, search) is controlled in `assets/js/gallery.js`.

Because everything is static, you can deploy the site to any static host (GitHub Pages, Netlify Drop, Vercel, Cloudflare Pages, etc.) without build tooling. Just ensure the data file has valid URLs for the art you want to spotlight.*** End Patch} to=functions.apply_patch ***!
