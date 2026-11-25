# Jose Miguel Luna: personal website

A minimal, single-page site: a short intro, a list of projects (Catch, Adulting, Azetta AI, Moonshine of the Seas, SIVICO) where each row expands for detail, and contact links.

It's one file (`index.html`) with no build step. The only external dependency is the Inter font from Google Fonts. Dark mode follows the system setting.

## Preview locally

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

## Still to fill in

Search `index.html` for `✏️`:

- [ ] **Email**: replace `hello@yourdomain.com` (contact list and Catch's "Get early access").
- [ ] **LinkedIn** URL.
- [ ] **Title** under your name (currently "Builder").
- [ ] **Photo**: put it in `images/` and uncomment the `<img class="avatar">` line in the header.
- [ ] **Screenshots and links**: each project has commented-out `<img>` and link lines inside its expanded section. Put images in `images/` and uncomment them.

## Deploy

- **GitHub Pages**: Settings → Pages → *Deploy from a branch* → pick the branch and `/ (root)`.
- **Vercel / Netlify / Cloudflare Pages**: import the repo, with no build command and the root as the output directory.
