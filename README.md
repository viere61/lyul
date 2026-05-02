# Personal Website

Static, minimal portfolio site for GitHub Pages.

## Edit Content

- Update the bio, name, project titles, descriptions, labels, and years in `index.html`.
- Duplicate an `<article class="project">...</article>` block to add more work.
- Replace each `.media-slot` placeholder with an `<img>` tag when you have images ready.

Example:

```html
<figure class="media-slot">
  <img src="assets/images/project-one.jpg" alt="Short description of the image" />
</figure>
```

## Fonts

The site uses `Helvetica Neue` for body text and `Cormorant Garamond` for more personal, editorial moments such as the name, section headings, and project titles. Helvetica Neue is usually available on macOS; Cormorant Garamond should be added as a local webfont or loaded from a static font stylesheet if you want it to appear consistently across all devices.

## Deploy on GitHub Pages

1. Push this folder to a GitHub repository.
2. In GitHub, go to `Settings` -> `Pages`.
3. Set the source to your main branch and root folder.
4. Save. GitHub Pages will serve `index.html` automatically.

No server-side code or build step is required.
