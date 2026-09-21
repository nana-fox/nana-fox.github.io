# NanaFlow website design QA

## Evidence

- Source visual truth: `/Users/nio/.codex/generated_images/01a042c7-add0-7cf1-ae77-2f1964e65f6f/exec-e1279b2b-0a7d-444e-9b39-35fe9ceafdd7.png`
- Browser implementation: `/Users/nio/project/nanafox/nanaflow-site/implementation-final-1145x1200.jpg`
- Mobile implementation: `/Users/nio/project/nanafox/nanaflow-site/implementation-mobile.jpg`
- Full-view comparison: `/Users/nio/project/nanafox/nanaflow-site/qa-comparison.jpg`
- Focused product comparison: `/Users/nio/project/nanafox/nanaflow-site/qa-focused-comparison.jpg`
- Route and state: `/`, Simplified Chinese, light appearance, page top, no hover or focus state

## Viewport and normalization

- Source pixels: 1145 × 1374.
- Implementation pixels: 1145 × 1200, captured from the in-app browser at a 1145 × 1200 CSS viewport with device pixel ratio 1.
- Mobile pixels and CSS viewport: 390 × 844 at device pixel ratio 1.
- The full comparison places both artifacts in equal-width, top-aligned columns. The source is scaled to fit its full height; the implementation uses the equal-width browser capture. The focused comparison enlarges the shared product-window and menu-bar region at the same horizontal scale.

## Findings

- Fonts and typography: passed. The implementation uses the macOS system family and PingFang fallback, with the same centered display hierarchy, restrained body weight, tight headline tracking, and readable navigation scale as the source.
- Spacing and layout rhythm: passed. Header, centered hero copy, pill CTA, GitHub link, product stage, and three-column feature strip preserve the source's order and visual rhythm. The responsive 390 px view has no horizontal overflow.
- Colors and visual tokens: passed. Deep green, warm white, muted gray, subtle mint, hairline borders, and soft elevation are consistent with the source.
- Image quality and asset fidelity: passed. The hero atmosphere is a dedicated raster asset. The NanaFlow app icon, timer window, and menu-bar strip are real product assets. Feature icons are vendored Tabler SVG image assets rather than CSS or handcrafted drawings.
- Copy and content: passed. The Chinese and English homepages retain the selected short value proposition and only the three agreed core capabilities.
- Navigation and behavior: passed. The feature anchor scrolls to `#features`; privacy, support, language, and GitHub destinations resolve to the intended URLs. No browser console warnings or errors were observed.

## Intentional differences

- The product window keeps NanaFlow's real native screenshot aspect ratio instead of stretching to the slightly taller generated mock.
- The menu-bar callout uses NanaFlow's real blue macOS menu-bar capture rather than the mock's neutral approximation. This is more accurate to the shipping product; the stronger blue is retained as a P3 polish difference.

## Comparison history

1. Initial browser comparison found one P2 mismatch: the three feature illustrations in the selected visual had been replaced by numeric labels.
2. Replaced the labels with vendored Tabler `browser`, `menu-2`, and `chart-bar` SVG image assets, recolored to the NanaFlow green token.
3. Re-captured the 1145 × 1200 implementation and repeated both full-view and focused comparisons. The icons are present and no actionable P0, P1, or P2 mismatch remains.

## Follow-up polish

- P3: replace the menu-bar callout when a neutral-background native capture is produced; do not recolor the current real screenshot in code.

final result: passed
