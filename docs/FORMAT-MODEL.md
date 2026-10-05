# Format model (conceptual)

This page explains how Passport Size **thinks about** a passport-photo specification. It does **not** describe source code, class names, or private APIs.

The live, machine-readable copy of shipped formats is:

- [passport-photo-formats.json](https://passportsize.getnorthpath.com/data/passport-photo-formats.json)
- [passport-photo-formats.csv](https://passportsize.getnorthpath.com/data/passport-photo-formats.csv)

License: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Attribution: GetNorthPath Passport Photo. `dateModified`: **2026-09-24**. **62** records, **54** countries.

---

## Why a structured format exists

A “passport photo” is not one size. The product treats each **document** as a record with:

1. An **outer frame** (millimetres, and derived inches / pixels at 300 and 600 DPI)
2. A **head-height window** (chin to crown, hair included)
3. **Appearance rules** the editor can display (background shade, glasses, expression)
4. A **citation** when one exists (`source_name`, `source_url`, `verified_at`)
5. A **head-height basis** (`official` vs ICAO-style general guidance)

Digital pixel and kilobyte windows are documented on dedicated pages (especially [digital-passport-photo](https://passportsize.getnorthpath.com/digital-passport-photo)) and are **not** all present as columns in the public JSON. Treat the JSON as the **print-geometry core**, and the document hubs as the **portal overlay**.

---

## Record fields (public JSON)

Each item in `records` includes:

| Field | Role |
| --- | --- |
| `slug` | Stable id (for example `canada-passport`, `united-states-visa`) |
| `country` | Display country or region (includes `Schengen Area`) |
| `document` | One of `passport`, `visa`, `immigration`, `citizenship`, `residence-card` |
| `name` | Human label (`Canada passport photo`) |
| `width_mm` / `height_mm` | Outer size |
| `width_in` / `height_in` | Inch conversion (2 in stored as 50.8 mm, not rounded to 51) |
| `px_300dpi` / `px_600dpi` | `[width, height]` pixel pairs |
| `head_min_mm` / `head_max_mm` | Published or ICAO-style chin-to-crown range |
| `head_source` | `official` or `icao` |
| `background` | Shade label used in the UI (plain white, light grey, cream, off-white, …) |
| `glasses` | `allowed-if-clear` or `not-allowed` |
| `expression` | `neutral` or `neutral-or-slight-smile` |
| `source_name` / `source_url` / `verified_at` | Citation when present |

Empty `source_url` means the millimetre head range should be treated as **guidance**, not a linked statute. See [SOURCES.md](SOURCES.md).

---

## How the editor uses a format (as described publicly)

From [passport-photo-maker](https://passportsize.getnorthpath.com/tools/passport-photo-maker) and [how-it-works](https://passportsize.getnorthpath.com/how-it-works):

1. **Locate** chin, eye line, and horizontal face centre (face-landmark model)
2. **Segment** the person to find the **true crown including hair** (landmarks alone tend to find the hairline)
3. **Scale** so chin-to-crown falls in the middle of `head_min_mm`–`head_max_mm`
4. **Place** the eye line at the expected height for that specification
5. **Render** the frame at the format’s pixel size
6. **Report** the measured millimetres so a person can check the number
7. Optionally **replace** the background with the format’s shade
8. **Encode** print DPI into the JPEG, or search JPEG quality to fit a portal’s kilobyte window

Users can override scale and position when hair, hats, or headscarves confuse the crown estimate.

---

## Size families (product copy)

Most formats fall into four groups ([passport-photo-size](https://passportsize.getnorthpath.com/passport-photo-size)):

| Family | Typical outer size | Examples |
| --- | --- | --- |
| ICAO portrait | 35×45 mm | UK, Ireland, Germany, India passport, Japan, Schengen visa, many others |
| US / India square | 50.8×50.8 mm (2×2 in) | US passport, US visa, USCIS, India visa, OCI |
| Canada / Brazil | 50×70 mm | Canada passport, citizenship, PR card; Brazil passport |
| One-offs | Various | China 33×48, Malaysia 35×50, Bangladesh 45×55, Finland 36×47, Spain 26×32, Greece 40×60, … |

**Same outer size does not mean the same head-height rule.** UK 29–34 mm and Ireland 31.5–36 mm share 35×45 mm.

---

## Extra constraints not in the JSON columns

Document hubs add rules the public table does not store as first-class fields, including:

- US **eye-line** band from the bottom edge
- China **head width** 15–22 mm and a **40–120 KB** window
- IRCC **420×540 px** floor and **4 MB** ceiling on a **35×45 mm** immigration frame (distinct from 50×70 mm prints)
- Recency (USCIS 30 days, citizenship 12 months, typical passports six months)
- Print annotations (photographer details on the back of one Canadian print)

Those belong on the document page and in [RULES.md](RULES.md), not as invented JSON keys.

---

## What this model is not

- Not an ICAO or ISO standard document
- Not a guarantee that a national office uses these millimetre figures tomorrow
- Not the internal implementation of the editor
