# Photo requirements (public overview)

Passport Size (live product: [GetNorthPath Passport Photo](https://passportsize.getnorthpath.com/)) is built around published passport, visa, and ID photo rules. This page summarises the requirements the site encodes in presets and explains on format pages. It is **not** official government policy.

If anything here disagrees with the issuing authority, **the official page wins**. Every format page on the live site links to a source where one is published.

Public dataset (CC BY 4.0, last modified **24 September 2026**): [JSON](https://passportsize.getnorthpath.com/data/passport-photo-formats.json) · [CSV](https://passportsize.getnorthpath.com/data/passport-photo-formats.csv)

Related: [SOURCES.md](SOURCES.md) · [FORMAT-MODEL.md](FORMAT-MODEL.md) · [photo-requirements](https://passportsize.getnorthpath.com/photo-requirements)

---

## How to read this page

The live site groups rules into four buckets. Size and head position cause more refusals than the rest combined.

1. **Size and head position** — outer millimetre size, chin-to-crown (hair included), centred/level head, space above the crown, and (for the United States) eye-line height
2. **Background** — shade for that country, uniform with no wall shadow, no other people or objects
3. **Face, expression, and eyes** — expression, both eyes visible, glasses, head coverings, even lighting
4. **Image quality and age** — sharpness, natural colour (no filters), recency, print stock where prints are required

Head height is measured **chin to crown, hair included**. The site reports the measured millimetre figure rather than asking you to guess from the crop.

---

## Common cross-cutting rules (from the live requirements guide)

| Topic | What the site states |
| --- | --- |
| Head height | The measurement that fails most applications. Canada 31–36 mm, UK 29–34 mm, US 25–35 mm (dataset: 25.4–34.9 mm) |
| Outer size | Must match the published size (for example Canada 50×70 mm, US 2×2 in). Hand-trimming usually breaks the ratio |
| Centred, level head | Square to the camera and centred horizontally |
| Space above the head | Most formats expect a small margin; Japan is described as explicit at 2–6 mm |
| US eye line | Eyes between 1 1/8 and 1 3/8 inches from the bottom edge |
| Background shade | Not always white. UK: light grey or cream. Germany and Ireland: plain light grey. Canada and US: white or off-white |
| Uniform background | No shadow behind the head; stand at least half a metre from the wall |
| Expression | Neutral, mouth closed, except the US (natural closed-mouth smile permitted). Infants are exempt in most countries |
| Glasses | US, Australia, Ireland and several others: remove glasses. Canada, Germany, UK: allowed only if eyes are clear with no glare, tint, or thick frames |
| Head coverings | Religious or medical reasons, full face visible chin to forehead, no shadow |
| Lighting | Even light on the face; no hot spots, red-eye, or one-sided shadow. Face a window |
| Sharpness | At least 600 px on the short side of the source; no filters or beautification |
| Recency | Usually within six months. USCIS: within 30 days of filing. Greece: within one month. Canadian PR: confirm on IRCC (the live PR page currently mentions both six and twelve months in different sections — use [IRCC PR photos](https://www.canada.ca/en/immigration-refugees-citizenship/services/permanent-residents/card/photos.html)) |
| Print stock | Matte or semi-matte photo paper, not glossy office paper |

Source for this section: [Photo requirements](https://passportsize.getnorthpath.com/photo-requirements) (live page, reviewed against site copy 5 October 2026).

---

## Supported formats (62 records, 54 countries)

Values below come from the public formats dataset (`head_source` is **Official** when the millimetre head range is taken from a cited authority page, or **ICAO general guidance** when the site uses ICAO-style defaults). Dataset date modified: **2026-09-24**.

| Document | Country | Type | Size | Head height | Background | Glasses | Expression | Head-height basis | Country page |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Canada passport photo | Canada | passport | 50 × 70 mm | 31–36 mm | Plain white | Allowed if eyes are clear | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/canada) |
| IRCC digital photo | Canada | immigration | 35 × 45 mm | 31–36 mm | Plain white | Allowed if eyes are clear | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/canada) |
| Canada citizenship photo | Canada | citizenship | 50 × 70 mm | 31–36 mm | Plain white | Allowed if eyes are clear | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/canada) |
| Canada PR card photo | Canada | residence-card | 50 × 70 mm | 31–36 mm | Plain white | Allowed if eyes are clear | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/canada) |
| US passport photo | United States | passport | 50.8 × 50.8 mm | 25.4–34.9 mm | White or off-white | Not allowed | Neutral or slight smile | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/united-states) |
| US visa photo | United States | visa | 50.8 × 50.8 mm | 25.4–34.9 mm | White or off-white | Not allowed | Neutral or slight smile | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/united-states) |
| USCIS photo | United States | immigration | 50.8 × 50.8 mm | 25.4–34.9 mm | White or off-white | Not allowed | Neutral or slight smile | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/united-states) |
| India passport photo | India | passport | 35 × 45 mm | 32–36 mm | Plain white | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/india) |
| India visa photo | India | visa | 50.8 × 50.8 mm | 25.4–34.9 mm | Plain white | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/india) |
| OCI card photo | India | immigration | 50.8 × 50.8 mm | 25.4–34.9 mm | Plain white | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/india) |
| UK passport photo | United Kingdom | passport | 35 × 45 mm | 29–34 mm | Light grey or cream | Allowed if eyes are clear | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/united-kingdom) |
| Australia passport photo | Australia | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Not allowed | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/australia) |
| New Zealand passport photo | New Zealand | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Not allowed | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/new-zealand) |
| Ireland passport photo | Ireland | passport | 35 × 45 mm | 31.5–36 mm | Plain light grey | Not allowed | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/ireland) |
| Germany passport photo | Germany | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Allowed if eyes are clear | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/germany) |
| Schengen visa photo | Schengen Area | visa | 35 × 45 mm | 32–36 mm | Plain light grey | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/schengen-area) |
| France passport photo | France | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Allowed if eyes are clear | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/france) |
| Italy passport photo | Italy | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/italy) |
| Spain passport photo | Spain | passport | 26 × 32 mm | 22–26 mm | Plain white | Allowed if eyes are clear | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/spain) |
| Netherlands passport photo | Netherlands | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/netherlands) |
| Belgium passport photo | Belgium | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/belgium) |
| Switzerland passport photo | Switzerland | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/switzerland) |
| Austria passport photo | Austria | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/austria) |
| Poland passport photo | Poland | passport | 35 × 45 mm | 32–36 mm | Plain white | Allowed if eyes are clear | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/poland) |
| Portugal passport photo | Portugal | passport | 35 × 45 mm | 32–36 mm | Plain white | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/portugal) |
| Sweden passport photo | Sweden | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/sweden) |
| Norway passport photo | Norway | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/norway) |
| Denmark passport photo | Denmark | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/denmark) |
| Finland passport photo | Finland | passport | 36 × 47 mm | 32–36 mm | Plain light grey | Allowed if eyes are clear | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/finland) |
| Greece passport photo | Greece | passport | 40 × 60 mm | 42.6–48 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/greece) |
| Czechia passport photo | Czechia | passport | 35 × 45 mm | 32–36 mm | Plain light grey | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/czechia) |
| Russia passport photo | Russia | passport | 35 × 45 mm | 32–36 mm | Plain white | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/russia) |
| Türkiye passport photo | Türkiye | passport | 50 × 60 mm | 42.6–48 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/turkiye) |
| Chinese visa photo | China | visa | 33 × 48 mm | 28–33 mm | Plain white | Not allowed | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/china) |
| China passport photo | China | passport | 33 × 48 mm | 28–33 mm | Plain white | Not allowed | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/china) |
| Japan passport photo | Japan | passport | 35 × 45 mm | 32–36 mm | Plain white | Allowed if eyes are clear | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/japan) |
| South Korea passport photo | South Korea | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/south-korea) |
| Singapore passport photo | Singapore | passport | 35 × 45 mm | 25–35 mm | Plain white | Not allowed | Neutral | Official | [Page](https://passportsize.getnorthpath.com/passport-photo/singapore) |
| Malaysia passport photo | Malaysia | passport | 35 × 50 mm | 35.5–40 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/malaysia) |
| Thailand passport photo | Thailand | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/thailand) |
| Vietnam passport photo | Vietnam | passport | 40 × 60 mm | 42.6–48 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/vietnam) |
| Indonesia passport photo | Indonesia | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/indonesia) |
| Philippines passport photo | Philippines | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/philippines) |
| Pakistan passport photo | Pakistan | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/pakistan) |
| Bangladesh passport photo | Bangladesh | passport | 45 × 55 mm | 39.1–44 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/bangladesh) |
| Sri Lanka passport photo | Sri Lanka | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/sri-lanka) |
| Nepal passport photo | Nepal | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/nepal) |
| UAE visa photo | United Arab Emirates | visa | 43 × 55 mm | 39.1–44 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/united-arab-emirates) |
| Saudi Arabia visa photo | Saudi Arabia | visa | 40 × 60 mm | 42.6–48 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/saudi-arabia) |
| Qatar visa photo | Qatar | visa | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/qatar) |
| Israel passport photo | Israel | passport | 35 × 45 mm | 32–36 mm | Plain white | Allowed if eyes are clear | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/israel) |
| Egypt visa photo | Egypt | visa | 40 × 60 mm | 42.6–48 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/egypt) |
| South Africa passport photo | South Africa | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/south-africa) |
| Nigeria passport photo | Nigeria | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/nigeria) |
| Kenya passport photo | Kenya | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/kenya) |
| Ghana passport photo | Ghana | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/ghana) |
| Ethiopia passport photo | Ethiopia | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/ethiopia) |
| Mexico passport photo | Mexico | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/mexico) |
| Brazil passport photo | Brazil | passport | 50 × 70 mm | 31–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/brazil) |
| Argentina passport photo | Argentina | passport | 40 × 40 mm | 26–32 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/argentina) |
| Colombia passport photo | Colombia | passport | 30 × 40 mm | 28.4–32 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/colombia) |
| Chile passport photo | Chile | passport | 35 × 45 mm | 32–36 mm | Plain white | Not allowed | Neutral | ICAO general guidance | [Page](https://passportsize.getnorthpath.com/passport-photo/chile) |

Dedicated document hubs (same formats, with extra digital/print notes): [Canada passport](https://passportsize.getnorthpath.com/canada-passport-photo), [IRCC digital](https://passportsize.getnorthpath.com/ircc-photo), [Canada citizenship](https://passportsize.getnorthpath.com/canada-citizenship-photo), [Canada PR card](https://passportsize.getnorthpath.com/canada-pr-card-photo), [US passport](https://passportsize.getnorthpath.com/us-passport-photo), [US visa](https://passportsize.getnorthpath.com/us-visa-photo), [USCIS](https://passportsize.getnorthpath.com/uscis-photo), [Chinese visa](https://passportsize.getnorthpath.com/chinese-visa-photo).

---

## Digital upload limits (formats that publish them)

From [Digital passport photo](https://passportsize.getnorthpath.com/digital-passport-photo) (live table). Confirm on the official portal before you upload.

| Document | Minimum pixels | Maximum pixels | File size | Format |
| --- | --- | --- | --- | --- |
| IRCC digital photo | 420 × 540 px | Not specified | Under 4096 KB | JPEG, PNG |
| Canada PR card photo | 715 × 1000 px | 2000 × 2800 px | Under 4096 KB | JPEG, PNG |
| US passport photo | 600 × 600 px | 1200 × 1200 px | Under 240 KB | JPEG |
| US visa photo | 600 × 600 px | 1200 × 1200 px | Under 240 KB | JPEG |
| India visa photo | 350 × 350 px | Not specified | 10–1024 KB | JPEG |
| OCI card photo | 360 × 360 px | Not specified | 10–200 KB | JPEG |
| UK passport photo | 600 × 750 px | Not specified | 50–10240 KB | JPEG |
| New Zealand passport photo | 900 × 1200 px | Not specified | 250–10240 KB | JPEG |
| Chinese visa photo | 354 × 472 px | 420 × 560 px | 40–120 KB | JPEG |
| Singapore passport photo | 400 × 514 px | Not specified | Under 1024 KB | JPEG |

The site also states extra Chinese visa geometry not stored as separate dataset columns: **head width 15–22 mm**, and a **pure white** background.

Print vs digital: printed photos are defined in millimetres and need a true DPI in the JPEG header; digital photos are defined in pixels and kilobytes. The editor offers separate print and digital presets where digital rules exist.

---

## Print sheets

The live FAQ and home page describe tiling onto **4×6**, **5×7**, **A4**, or **US Letter** with dashed cut guides, and showing how many copies fit before download.

---

## Source photos the tools accept

From the live FAQ and editor copy:

- **JPG, PNG, WEBP**; most modern browsers also handle **HEIC**
- Files **up to 25 MB**
- EXIF rotation is applied automatically
- Face-on head-and-shoulders with space around the hair works; arm’s-length selfies often cannot be cropped compliantly

---

## Signature image sizes (signature tool only)

From [Signature resize](https://passportsize.getnorthpath.com/tools/signature-resize):

| Preset | Pixels | File size |
| --- | --- | --- |
| India forms | 140 × 60 | Under 20 KB |
| Passport Seva | 350 × 150 | Under 50 KB |
| India OCI | 200 × 100 | Under 200 KB |
| General upload | 600 × 200 | Under 100 KB |

---

## Disclaimer

Not affiliated with IRCC, the US Department of State, USCIS, or any passport authority. Tools are helpers. The accepting officer has the final say. See [terms of service](https://passportsize.getnorthpath.com/terms-of-service).
