# website

outportsoftware.ca: the Outport Software site, served by GitHub Pages from `main`.

- `/` company page. `/yesteryear/`, `/flashpage/` and `/toweridle/` each hold an app's help page
  (`index.html`), `privacy.html` and `terms.html`. Store listings and the apps link to these URLs,
  so never move them, and change legal wording only on purpose.
- `/jobcloseout/` is an unlinked demand test page. It still uses the old `/style.css`, which is
  kept only for it.
- Plain HTML and one stylesheet, `assets/site.css`. No build step, no JavaScript, no cookies, no
  analytics, no third-party requests. Fonts are self-hosted in `assets/fonts/` (all SIL OFL; the
  licences sit beside them): Bricolage Grotesque for headings, Atkinson Hyperlegible Next for
  text, Oxanium for the Tower Idle name.
- Light and dark themes follow `prefers-color-scheme`. The colour tokens are at the top of
  `assets/site.css` and match the design system in `app-factory/packages/core`.
- `logo.svg` is the company mark (saltbox house over a harbour). The harbour scene on the home
  page is inline SVG coloured by the same tokens.
- Each new app gets its own folder with `index.html`, `privacy.html` and `terms.html`, a card on
  the home page, a footer column and entries in `sitemap.xml`.
- `.preview/` holds local screenshots and is not tracked.
