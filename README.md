# KYttinii.github.io

Kayoung Lee's portfolio. AI Product Developer, Freediver, Writer.
Built with the 다이빙캣 design system. Plain HTML/CSS, no build step.

- `index.html` — the portfolio
- `photography/` — underwater photo gallery (structure inspired by rampatra/photography)
- `assets/img/` — photos ©free.young.510

## Adding a photo to the gallery

1. Upload the full-size photo (long edge ~1400px) to `photography/images/fulls/`
   and a small version (long edge ~640px) to `photography/images/thumbs/`.
2. Add one entry to `photography/photos.json`:

```json
{
  "full": "images/fulls/my-photo.jpg",
  "thumb": "images/thumbs/my-photo.jpg",
  "title": "Short title",
  "alt": "What is in the photo, for screen readers"
}
```

Camera settings (model, ƒ-stop, shutter, ISO) appear automatically if the JPEG still has its EXIF data.
If it doesn't, add them by hand: `"settings": ["OM-1", "ƒ/8", "1/250s", "ISO 400"]`.
