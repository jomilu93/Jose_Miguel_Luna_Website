# Jose Miguel L: personal website

A one-page "bento" layout: a full-width intro (photo, name, description), a row of product cards (Catch App, Adulting, Moonshine of the Seas), a row of research cards (Azetta AI, SLAY), and contact cards. Clicking a project card opens a panel with more detail. Links like `/#adulting` open that panel directly.

It's one file (`index.html`) with no build step. The only external dependency is Google Fonts (Inter, Inter Tight). Dark mode follows the system setting.

## Preview locally

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

## Still to fill in

Search `index.html` for `✏️`:

- [ ] **Screenshots and links**: each project's panel (the `<dialog>` elements at the bottom) has commented-out `<img class="shot">` and link lines. Put images in `images/` and uncomment them.

Project colors are the `--catch`, `--adulting`, `--moonshine`, `--azetta` and `--slay` tokens at the top of the `<style>` block.

## Deploy

- **GitHub Pages**: Settings → Pages → *Deploy from a branch* → `main` and `/ (root)`. The site is published at https://jomilu93.github.io/Jose_Miguel_Luna_Website/ and updates within a minute or two of each push to `main`. `.nojekyll` tells Pages to serve the files as-is.
- **Vercel / Netlify / Cloudflare Pages**: import the repo, with no build command and the root as the output directory.
