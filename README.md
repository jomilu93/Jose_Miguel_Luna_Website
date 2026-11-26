# Jose Miguel Luna: personal website

A one-page "bento" layout: an intro card, a big **Now building: Catch App** card, one card each for Adulting, Azetta AI, Moonshine of the Seas and SIVICO, plus contact cards. Clicking a project card opens a panel with more detail. Links like `/#adulting` open that panel directly.

It's one file (`index.html`) with no build step. The only external dependency is Google Fonts (Inter, Inter Tight). Dark mode follows the system setting.

## Preview locally

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

## Still to fill in

Search `index.html` for `✏️`:

- [ ] **Screenshots and links**: each project's panel (the `<dialog>` elements at the bottom) has commented-out `<img class="shot">` and link lines. Put images in `images/` and uncomment them.

Project colors are the `--catch`, `--adulting`, `--azetta`, `--moonshine` and `--sivico` tokens at the top of the `<style>` block.

## Deploy

- **GitHub Pages**: Settings → Pages → *Deploy from a branch* → pick the branch and `/ (root)`.
- **Vercel / Netlify / Cloudflare Pages**: import the repo, with no build command and the root as the output directory.
