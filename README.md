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
