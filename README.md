# Digital Crack Gauge

Measure concrete crack widths from a photograph, from close up to 200 m away. No ladder, no contact with the surface. Physics only, no AI.

**Open the tool:** https://volkov596.github.io/digitalcrackgauge/ (access code required, see [Access](#access))

## What it does

Load a photo, set its scale, draw a short line across the crack and read the width in millimetres.

- **Approach A** scales against a crack of known width photographed with the same camera: the most accurate route.
- **Approach B** needs no reference.
- **A2 and B2** correct for surface colour: paint, coloured or dark concrete.
- **Expected accuracy** is shown with every estimate, and the tool warns when a photo lacks the detail for a reliable reading.
- **Along crack** (Pro): trace a crack once and get its width along the whole length (10–50 sections; mean, median, minimum, maximum, 95th percentile and a chart).
- Several lines per photo, a measurement log with CSV export, and annotated images for reports.
- JPEG, PNG and 16-bit PNG and TIFF photos up to 52 MP.
- Built-in user guide (the **?** button).

## How it works

Lens blur spreads a crack's darkness over neighbouring pixels: the crack looks wider and fainter the further away you are, but the total contrast it creates stays about the same. Digital Crack Gauge measures that contrast along your line and many parallel lines beside it, then turns it into a width. This is why it can measure cracks narrower than a single pixel, and why it needs no training data.

## Accuracy

The key number is how many pixels wide the crack is in the photo.

| Crack in the photo | Typical accuracy, Approach B |
|---|---|
| 2 px or more | ±10% |
| 1–2 px | ±20% |
| 0.5–1 px | ±30%, may read high |
| under 0.5 px | indicative only |

With a reference (Approach A), lab errors averaged about 0.03 mm on 0.1–0.4 mm lines. On site, repeat measurements of the same spot with different cameras and distances typically agreed within about 10% on bare concrete. Full results are in the paper.

## Access

- **Lite**: the full measuring workflow (photo, scale, line, all four results, several lines, log).
- **Pro**: adds Along crack, scaling from distance with camera profiles, fitting the estimate to your own camera, graph-based refinement and averaging options.

Access codes are issued by the author. Access is currently limited to Australia and New Zealand.

## Privacy

- Photos stay on your device. Only the readings along your line are sent to the analysis service, and they are not stored.
- Anonymous usage counts (date, country, access channel) are kept. No photos, readings or personal details.
- The log, profiles and settings are stored in your browser only.

## Requirements

A current desktop or mobile browser and an internet connection.

## Paper

*Accurate Measurement of Structural Cracks at Long Range Using Consumer Cameras (Physics only, no AI).* E. Volkov. Preprint, DOI to follow. Presented at the NZ Bridge & Geotechnical Conference 2026, Auckland.

## Licence and terms

© 2026 Egor Volkov. All rights reserved. Patent pending.

This repository hosts the app; it is not open source. No licence is granted to copy, modify, redistribute, host or reverse engineer the software or the analysis service. Use of the app is subject to the [Terms of Use](TERMS.md).

## Contact

Pro access, licensing and other enquiries: use the email button in the app, or [LinkedIn](https://www.linkedin.com/in/egorv).
