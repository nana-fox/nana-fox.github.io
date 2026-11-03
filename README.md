# NanaFlow website

Public product, privacy, and support pages for NanaFlow.

- Product: `https://nana-fox.github.io/`
- Privacy: `https://nana-fox.github.io/privacy/`
- Support: `https://nana-fox.github.io/support/`

The website is a static build in `dist/`. To preview locally:

```sh
python3 -m http.server 4280 --bind 127.0.0.1 --directory dist
```

Pushing `main` publishes `dist/` through GitHub Pages.

## Release copy — checked 2026-11-02

The official CN and US listings now show free version 1.0.1, and App Store Connect shows exact build 1.0.1 (4) ready for distribution. English and Simplified Chinese home/support pages reflect this publication. An official Store download of 1.0.1 (4) was verified on 2026-11-03 (Store receipt and Apple signing). Support copy does not advertise a history-list or backup/import interface that the store app does not expose.

For future releases, update `#release-status` in both home pages and `#updates` in both support pages from actual Apple publication evidence; track an actual Store download separately and never substitute listing visibility for that check. Keep the existing Pages workflow; do not rebuild the site in another framework. On November 2, the privacy pages clarified that the store UI has no backup/restore entry point; the original policy date and data-collection scope remain unchanged.

## Copy maintenance

Home pages lead with the timer, menu-bar controls and local statistics, then the official download link, macOS requirement and account-free use. Support pages cover reachable controls, release-channel differences and specific unresolved behavior without guaranteeing a sound fix. Keep English and Chinese content equivalent; keep pending-version improvements labeled with their version.

The App Store copy lives in `nana-fox/NanaFlow` under `AppStore/metadata.*.md`; its maintenance handoff is `Plans/project-maintenance.md`. Do not copy Beta-only features or inaccessible backup/history UI into the store website. Since the 2026-11-03 redesign the home pages draw the app UI in HTML/CSS with sample data (labelled as an illustration) instead of using screenshots; keep the drawn menus, labels and sound names in sync with the app's real strings. `assets/og-zh.png` / `og-en.png` are the 1200×630 share images rendered from the same scene.

Only `dist/` is deployed. Local preview servers, private release receipts, keys and user data never belong in this repository. Keep previews bound to loopback and stop the server after checking the pages.
