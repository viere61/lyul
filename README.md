# Personal Website

Static, minimal portfolio site for GitHub Pages.

## Edit Content

- Update the bio, name, project titles, descriptions, labels, and years in `index.html`.
- Duplicate an `<article class="project">...</article>` block in `index.html` to add more work to the homepage index.
- Give each project title a link to a static detail page, such as `art/lake.html` or `interactions/project-title-one.html`.
- Use the homepage `.media-slot` as an optional preview image, not the full portfolio presentation.

Example:

```html
<figure class="media-slot">
  <img src="assets/images/project-one.jpg" alt="Short description of the image" />
</figure>
```

## Add Project Pages

Artwork pages live in `art/`. Interaction project pages live in `interactions/`.

To add a new artwork:

1. Duplicate one of the existing files in `art/`.
2. Rename it, for example `new-artwork-title.html`.
3. Update the page title, heading, label, year, description, and image placeholders.
4. Link to it from the matching project title in `index.html`.

## Flexible Image Layouts

Detail pages include reusable gallery classes for different image needs:

- `image-full`: a wide landscape image or hero documentation image.
- `image-narrow`: a centered portrait image that does not stretch too wide.
- `image-pair`: two related images side by side on desktop and stacked on mobile.
- `image-stack`: a vertical sequence of images with generous spacing.

Replace a placeholder like this:

```html
<figure class="gallery-item image-narrow">
  <img src="../assets/images/lake-detail.jpg" alt="Describe the artwork clearly" />
  <figcaption>Optional caption, dimensions, material, or context.</figcaption>
</figure>
```

Put image files in `assets/images/`. From pages inside `art/` or `interactions/`, image paths should usually start with `../assets/images/`.

## Fonts

The site uses `Helvetica Neue` for body text and `Cormorant Garamond` for more personal, editorial moments such as the name, section headings, and project titles. Helvetica Neue is usually available on macOS; Cormorant Garamond should be added as a local webfont or loaded from a static font stylesheet if you want it to appear consistently across all devices.

## Deploy on GitHub Pages

1. Push this folder to a GitHub repository.
2. In GitHub, go to `Settings` -> `Pages`.
3. Set the source to your main branch and root folder.
4. Save. GitHub Pages will serve `index.html` automatically.

No server-side code or build step is required.
