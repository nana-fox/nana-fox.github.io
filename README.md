# NanaFlow website

Public product, privacy, and support pages for NanaFlow.

- Product: `https://nana-fox.github.io/`
- Privacy: `https://nana-fox.github.io/privacy/`
- Support: `https://nana-fox.github.io/support/`

The website is a static build in `dist/`. To preview locally:

```sh
python3 -m http.server 4280 --directory dist
```

Pushing `main` publishes `dist/` through GitHub Pages.

## Release copy — 2026-11-01

The download buttons link to the existing free Mac App Store version 1.0. Version 1.0.1 (4) is in App Review and is not described as downloadable yet. English and Simplified Chinese home/support pages state this separately. Support copy does not advertise a history-list or backup/import interface that the store app does not expose.

After Apple releases 1.0.1 and its official download is verified, update `#release-status` in both home pages and `#updates` in both support pages. Keep the existing Pages workflow; do not rebuild the site in another framework. Privacy/data-collection terms are unchanged by this copy correction.
