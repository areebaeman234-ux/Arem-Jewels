# Arem Jewels — Site

Static 4-page site: `index.html` (Home), `shop.html`, `about.html`, `contact.html`, sharing one `style.css`.

## Dropping in real images

Every placeholder is a gold-dashed box with a label. To swap one in:

1. Add your image file to `assets/images/` (folder already created).
2. Find the matching HTML comment above the placeholder `<div class="media-frame ...">` — it names the suggested filename.
3. Replace the whole `<div class="media-frame ...">...</div>` block with:
   ```html
   <img src="assets/images/your-file.jpg" alt="Describe the image">
   ```
   Keep the `alt` text — it's what screen readers announce.

Suggested filenames (from your image curation notes):

| Placeholder | Suggested filename |
|---|---|
| Hero texture (Home) | `hero-paper-grain.jpg` |
| Featured: Layered Necklace | `featured-layered-necklace.jpg` |
| Featured: Asymmetric Pendant | `featured-asymmetric-pendant.jpg` |
| Featured: Hammered Ring | `featured-hammered-ring.jpg` |
| Collection: Heritage Gold | `collection-heritage-gold.jpg` |
| Collection: Silver Stories | `collection-silver-stories.jpg` |
| Collection: Custom Pieces | `collection-custom-pieces.jpg` |
| Process icon: Design | `icon-design.svg` |
| Process icon: Craft | `icon-craft.svg` |
| Process icon: Finish | `icon-finish.svg` |
| About: founder portrait (real photo) | `founder-portrait.jpg` |
| Contact: location map | replace with an embedded map iframe, or a screenshot |

## Deploying to GitHub Pages

If this replaces your current placeholder repo (`Arem-Jewels`):

1. Copy these files into your repo, overwriting the placeholder `index.html`.
2. Commit and push to the branch GitHub Pages is serving from (usually `main`).
3. Live in a minute or two at your existing URL: https://areebaeman234-ux.github.io/Arem-Jewels/

## Activating the contact form

The form on `contact.html` is static — it won't send anything yet. Easiest free fix once you're ready:

1. Sign up at [Formspree](https://formspree.io) (free tier).
2. Replace `action="#"` in `contact.html`'s `<form>` tag with the endpoint Formspree gives you.
3. Delete the `.form-note` paragraph.

No other code changes needed — still 100% static, still free, still hosted on GitHub Pages.
