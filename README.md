# my-portfolio

Personal portfolio of Ezechukwu Miracle (Mi-Tech), live at <https://mi-tech.pages.dev/>.

It is one static page, `index.html`, with plain HTML, CSS and a little vanilla JavaScript. There is no build step: open the file in a browser, or serve the folder with any static server (for example `python3 -m http.server`).

## Layout

- `index.html`: the whole site. Styles are in the `<style>` block in the head; scripts sit at the end of the body.
- `assets/projects/<project>/`: screenshots, in two sizes per screen. `<screen>.webp` (up to 1200px tall) is shown in the screenshot viewer, and `<screen>-600.webp` (600px tall) is shown on the project card. Banners use `banner.webp` plus a smaller `banner-<width>.webp`.
- `assets/photos/`: photos of me, each with a smaller copy (`-400`, `-600` or `-800`) for small screens.
- `assets/og-image.jpg`: the 1200×630 preview that shows when the link is shared.
- `ezechukwu_miracle_cv.docx`: the resume behind the "My Resume" buttons.

## Adding a project

1. Export the screens as WebP into `assets/projects/<project>/`, in both sizes above.
2. Copy an existing `<article class="project">` in `index.html` and update the text, the three card images, and the hidden `gallery-src` list (one link per screen, with its width, height and a caption that doubles as alt text).
3. Set `--accent` on the article to the app's main colour; it tints the card behind the screens.

If the site's address changes, update the canonical, Open Graph and JSON-LD URLs in the `<head>`.
