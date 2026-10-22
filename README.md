# exif inspector

Drop in a photo, see everything it quietly knows about you: camera, lens, settings, exact date — and GPS coordinates, if they're in there.

**Live demo:** https://mjanthony819.github.io/exif-inspector/

## what it does

- drag & drop (or click to choose) any JPEG / TIFF / HEIC / PNG / WebP
- summary card: camera, lens, exposure, aperture, ISO, focal length, date taken, software
- GPS coordinates with a one-click OpenStreetMap link when present
- full raw tag table (every EXIF tag, sorted)
- **download a stripped copy** — re-encodes the image through a canvas, which drops all metadata (the privacy fix)
- 100% client-side: the file is read in your browser and never uploaded anywhere
- light/dark theme

## why it matters

Every phone photo embeds EXIF metadata by default — including precise GPS. Posting an untouched photo can leak where you live. Social platforms strip it; direct messages often don't.

## stack

Single `index.html` — vanilla JS + [exifr](https://github.com/MikeKovarik/exifr) from CDN. No build step. Hosted on GitHub Pages.

## run locally

Open `index.html` in a browser (needs internet once, for the exifr CDN).

---

Built with AI assistance (design and direction by [@mjanthony819](https://github.com/mjanthony819)).
