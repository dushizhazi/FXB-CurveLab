# RC3 Test Report — 2026-10-27

## Environment
- Linux container, Chromium headless (`/usr/bin/chromium`), Python Playwright; HTML loaded via `page.set_content` because `file://` navigation was administratively blocked.
- Desktop viewport 1280×900; emulated mobile viewport 390×844 (touch enabled).
- Under test: `index.html` SHA-256 `95cff7f479ac4c3aa84d2087c90709a3ca339a89ad5136a1aaf9d8e3dfccd56f`.
- JavaScript extracted and passed `node --check`.

## Automated browser results

| Case | Result |
|---|---|
| R01 unapplied export | PASS |
| R01 invalid plot export | PASS |
| R02 exponent | PASS |
| R03 sqrt domain | PASS |
| R04-B error switch | PASS |
| R04-A PNG error | PASS |
| R04-B score switch | PASS |
| R04-B coordinate switch | PASS |
| SVG actual DOM export | PASS |
| PNG real download | PASS |
| SVG real download | PASS |
| mobile initial render | PASS |


12/12 PASS. Real PNG and SVG downloads validated by file signatures/content. Screenshots saved for desktop/mobile.

## Additional user acceptance (reported to 03 on 2026-10-27)
- User confirmed physical mobile two-finger gesture operation and actual offline opening tested successfully. This is user-reported acceptance recorded by 03, not an independent T03 or 03 browser run. Device/browser versions and step logs were not provided.
- The RC4 application HTML is byte-identical to RC3, so the existing RC3 browser test evidence remains applicable.

## Not established
- Independent physical Android/iOS two-finger gesture measurements, clipboard permissions, complete fit-model round-trip matrix, storage-denial browser profile, and cross-device visual compatibility. User acceptance of gestures and offline opening is documented above.
- Automated browser ran via injected HTML, not actual file:// launch or deployed GitHub Pages. Separately, user confirmed actual offline opening.
- PNG pixel-level visual comparison against SVG not performed; successful decode and PNG signature verified.

No claim of complete release-gate clearance; independent 03 review remains required.
