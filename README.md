# FXB CurveLab v2.1.0

Standalone offline HTML for formula plotting and sketch-to-equation fitting. Open `index.html` in a browser. Chinese and English interfaces; light and dark themes. Export SVG and PNG.

## Syntax

`x`, `pi`, `e`, `+ - * / ^`, parentheses, `sin`, `cos`, `tan`, `sqrt`, `abs`, `exp`, `ln`, `log`, decimal and scientific notation (e.g. `1e-7`). Explicit multiplication required.

## Limitations

Sketch fitting is approximate and non-unique; polynomial, sine and shifted reciprocal/hyperbola models are supported. Not a general symbolic equation solver; `y=f(x)` cannot represent arbitrary implicit curves. Domain restrictions and asymptotes may leave visible gaps.

## Compatibility and privacy

No network calls or backend. Runs in modern browsers supporting Canvas, SVG, Pointer Events and ResizeObserver. Chromium desktop/mobile-emulation checks passed, including SVG/PNG downloads. The user confirmed physical mobile two-finger gestures and actual offline opening. Device/browser versions were not recorded; cross-device compatibility remains limited to the tested scope. Theme/language preferences are saved locally when storage is permitted.

## License and assets

Code: MIT, see LICENSE. See SOURCES.md for logo provenance and trademark distinction.
