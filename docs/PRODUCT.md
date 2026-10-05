# What Passport Size does

**Passport Size** ([GetNorthPath Passport Photo](https://passportsize.getnorthpath.com/)) is a free web app that helps people produce passport, visa, and ID photos that match published specifications: millimetre head height, the correct background shade, true print DPI, and portal pixel/kilobyte limits.

Live: [passportsize.getnorthpath.com](https://passportsize.getnorthpath.com/)

It is a **focused product**: a photo editor plus companion tools, country and document pages, size tables, requirements guides, and a public formats dataset. It is **not** a full immigration case-management system. Broader Canadian immigration tools live on [getnorthpath.com](https://www.getnorthpath.com). See [ABOUT.md](../ABOUT.md).

---

## Problem it solves

Passport and visa photos fail for practical reasons applicants hit every week:

- **Head height** that is off by a few millimetres (chin to crown, hair included) — the failure you cannot judge by eye
- **Wrong background shade** (white is not universal; UK wants light grey or cream)
- **Digital upload caps** that fight pixel minimums (US 600×600 px but under 240 KB; Chinese visas 40–120 KB)
- **Print files with no DPI**, so a correct crop prints at the wrong physical size
- Tools that **upload a biometric photo to a server**, watermark it, and charge to remove the watermark

Generic croppers only match an aspect ratio. This product measures the head and encodes the format’s published range.

---

## Product surfaces

```
passportsize.getnorthpath.com
├── Home                 product hub, four-step flow, tools, documents, FAQ
├── Tools                7 in-browser tools
├── Document hubs        Canada, IRCC, US, USCIS, China, baby, digital, 2×2
├── Countries            /passport-photo/{country} for 54 countries
├── Sizes                mm, inches, cm, pixels, aspect ratio
├── Guides               requirements, FAQ, how-it-works, blog
├── Dataset              JSON / CSV of 62 formats (CC BY 4.0)
└── Legal                privacy-policy, terms-of-service, contact
```

Details: [FEATURES.md](FEATURES.md) · [WORKFLOW.md](WORKFLOW.md) · [RULES.md](RULES.md)

---

## Who it is for

- People applying for a **passport or visa** who will photograph themselves at home
- Applicants uploading to **IRCC, DS-160, USCIS, or similar** portals
- Parents making **infant** photos (relaxed expression rules; size and background still apply)
- Community helpers who need **cited format pages** rather than a guess

---

## User journey (typical)

1. Land on the home hub or a country/document URL
2. Choose country and document (or use a dedicated hub such as IRCC digital)
3. Drop in a JPG, PNG, WEBP, or (in most modern browsers) HEIC, up to 25 MB
4. Review the compliance panel (head height in millimetres, background, glasses rule)
5. Optionally replace the background and use sliders if automatic crown detection misses hair volume
6. Export **print** (DPI written into the JPEG) and/or **digital** (pixels and kilobyte search)
7. Enter an **email to unlock** the download — the photo file still never leaves the browser

No account is required. See [PRIVACY.md](PRIVACY.md).

---

## Accuracy stance

| Source | Role |
| --- | --- |
| Issuing-authority photo pages | Official millimetre, background, glasses, and recency rules |
| Portal upload instructions | Pixel floors/ceilings and kilobyte windows |
| Public formats dataset | Machine-readable copy of what the product currently ships |
| ICAO-style defaults | Used only where the dataset marks `head_source` as ICAO general guidance |

If this app and the issuing authority disagree, **the authority wins**. The live site says specifications change, the officer has the final say, and every format page should be checked against its official source.

The product **does not guarantee acceptance**. Acceptance can depend on a human reviewer, whether appearance has changed, print quality, and rules that changed after the last review (dataset `verified_at` / `dateModified`: **2026-09-24**).

---

## Privacy (product architecture)

Photos are processed in the visitor’s browser. The [how-it-works](https://passportsize.getnorthpath.com/how-it-works) and [privacy policy](https://passportsize.getnorthpath.com/privacy-policy) pages state there is **no upload endpoint** and **no server-side image processing**. Optional email unlock and operational metadata are described in [PRIVACY.md](PRIVACY.md). Only those claims that can be verified from public pages are documented here.

---

## Limitations (verified from live copy)

- Automatic detection can miss voluminous or light hair, hats, or headscarves — sliders exist to override
- Background replacement cannot fix face shadows, glare, blur, or selfie perspective
- A tightly cropped original may have **no image above the crown**, so the head cannot be scaled into range
- Some formats in the dataset have **empty `source_url`** (ICAO-style defaults); treat those as guidance, not a cited statute
- The live Canada PR card page currently mentions **both six-month and twelve-month** recency in different sections — confirm on [IRCC](https://www.canada.ca/en/immigration-refugees-citizenship/services/permanent-residents/card/photos.html)

---

## Related GetNorthPath products

| Product | Job |
| --- | --- |
| **Passport Size** (this) | Free in-browser passport / visa / ID photos |
| **GetNorthPath** | Features and free DIY tools for Canadian immigration |
| **IRCC Ready Docs** | Free document tools and IRCC upload guides |
| **OINP Calculator** | Ontario PNP points |
| **AORTrack** | Community PR milestone timelines |
| **CRS calculator** | Federal Express Entry ranking |

© GetNorthPath Inc. Not affiliated with IRCC, the US Department of State, USCIS, or any passport authority.
