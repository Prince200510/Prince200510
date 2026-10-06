# Validation report

Checked 2026-10-06 using local headless Chromium 133. No changes were pushed to GitHub.

| Check | Result |
| --- | --- |
| SVG XML | All five animated SVGs parse successfully; local IDs are unique and namespaced. |
| Forbidden content | No JavaScript, foreignObject, externally referenced fonts, images or stylesheets in SVGs. |
| Fonts | Two embedded base64 WOFF2 fonts in every SVG; browser font-loading checks passed. Both licenses included. |
| External asset requests | Zero HTTP/HTTPS requests during graphic and local preview rendering. |
| Timeline | Each animated SVG rendered at 0, 2, 5, 9 and 13 seconds using paused CSS and SVG timelines. |
| Image embedding | Each SVG also rendered as a visible HTML img at nominal 0, 2, 5, 9 and 13 seconds. |
| Static fallback | Animation elements removed and CSS animation disabled; all five rendered with readable final/base content. |
| Reduced motion | Standalone media-query checks show zero CSS animations and hidden moving SMIL decoration. README and preview additionally use picture/source to select animation-free static files, confirmed through currentSrc. |
| Transparency | PNG inspection confirms transparent outer corner pixels on all five graphics; opaque navy content panels are intentional. No portraits or raster masks are used. |
| Text bounds | Browser text bounds stay within the SVG canvas after entrances. Manually inspected for interior card overflow, overlap and glyph problems. |
| Layout | Reviewed full-size graphics, desktop image embedding and a 375px mobile preview; no horizontal page overflow. Fine print scales down on narrow screens, as it does for fixed-layout README graphics. |
| README | All five primary image paths end in ?v=1. Static source paths also end in ?v=1. Projects table and normal clickable social links included. |

At 0 seconds the name and badge are intentionally entering. The static copies immediately show all final content. The carousel changes every 4 seconds and the roles every 4 seconds. Badge entrance settles, followed by a ±1.7° pendulum loop. Licensed Simple Icons marks are paired with explicit technology labels.

## Links

- GitHub profile: HTTP 200.
- CrownDB, CrownKit and Cpp repositories: HTTP 200.
- Instagram: HTTP 200; returned page title matches the supplied username.
- LinkedIn: timed out during automated checking. The exact user-supplied URL is retained; availability was not independently confirmed.
- Email: syntax checked; no email sent and delivery not tested.

This is local browser verification, not a live test of GitHub's image proxy or every GitHub client. The package contains no contribution service, live stats badge or guessed counts. Social cards themselves are not links when embedded as images; the README places real links beneath them.
