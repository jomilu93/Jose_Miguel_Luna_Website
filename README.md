# Jose Miguel Luna: personal website

A single-page portfolio: hero, **Now building** (Catch), **Selected work** (Adulting, Azetta AI, Moonshine of the Seas, SIVICO), About and Contact.

It's one self-contained file (`index.html`) with no build step and no dependencies apart from Google Fonts. It supports light and dark mode (it follows the system setting and has a toggle), works on phones, and respects reduced-motion settings.

## Preview locally

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

Or just double-click `index.html`.

## Still to fill in

Every spot is marked with a `✏️ EDIT` comment in `index.html`:

- [ ] **Email**: replace both `hello@yourdomain.com` links (contact section and the Catch early-access button).
- [ ] **LinkedIn**: put your profile URL in the contact section.
- [ ] **Project links**: each project card has a commented-out "Visit →" link. Uncomment it and add the URL.
- [ ] **About copy**: the About section is a first draft built from the themes in your projects. Rewrite it in your own voice.
- [ ] Optional: the hero says "Hola, I'm …". Change it if that isn't your vibe.

Project colors are set in the `:root` tokens at the top of the `<style>` block (`--adulting`, `--azetta`, `--moonshine`, `--sivico`, `--catch`). The dark theme has its own set below them.

## Deploy

The site lives at the repo root, so any static host works as-is:

- **GitHub Pages**: Settings → Pages → *Deploy from a branch* → pick the branch and `/ (root)`. It goes live at `https://jomilu93.github.io/jose_miguel_luna_website/`, or at a custom domain if you add one.
- **Vercel / Netlify / Cloudflare Pages**: import the repo, leave the build command empty, and set the output directory to the root.
