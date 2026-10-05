# Official sources

Photo specifications on Passport Size are a **reading of published requirements**, not government policy. Always confirm on the issuing-authority page before you submit.

This list is limited to sources that appear on the live product ([llms.txt](https://passportsize.getnorthpath.com/llms.txt) official-sources block, footer, format dataset `source_url` / `source_name` / `verified_at`, and individual document hubs).

**Dataset date modified:** 24 September 2026  
**This documentation pass:** 5 October 2026  
**Live disclaimer:** “Photo specifications change and the accepting officer has the final say.”

Where `head_source` on a format is **ICAO general guidance** and `source_url` is empty, the product is **not** claiming a cited national PDF for that millimetre range. Those rows are listed in [RULES.md](RULES.md) but are **not** given a fake official URL here.

---

## Sources the live site highlights

| Authority | What it is for | URL | Cited on |
| --- | --- | --- | --- |
| Government of Canada | Canadian passport photos | [canada.ca passport photos](https://www.canada.ca/en/immigration-refugees-citizenship/services/canadian-passports/photos.html) | Footer, llms.txt, dataset (`canada-passport`, verified 2026-09-24) |
| IRCC | Permanent resident card photos | [IRCC PR photos](https://www.canada.ca/en/immigration-refugees-citizenship/services/permanent-residents/card/photos.html) | Footer, llms.txt, dataset (`canada-pr-card`, verified 2026-09-24) |
| IRCC | Temporary resident photograph specifications | [TRV photograph specifications](https://www.canada.ca/en/immigration-refugees-citizenship/services/application/application-forms-guides/temporary-resident-visa-application-photograph-specifications.html) | Dataset (`canada-ircc-digital`, verified 2026-09-24) |
| IRCC | Citizenship application photograph specifications | [CIT photograph specifications](https://www.canada.ca/en/immigration-refugees-citizenship/services/application/application-forms-guides/citizenship-application-photograph-specifications.html) | Dataset (`canada-citizenship`, verified 2026-09-24) |
| US Department of State | US passport photos | [travel.state.gov photos](https://travel.state.gov/content/travel/en/passports/how-apply/photos.html) | Footer, llms.txt, dataset (`united-states-passport`, verified 2026-09-24) |
| US Department of State | US visa photos | [travel.state.gov visa photos](https://travel.state.gov/content/travel/en/us-visas/visa-information-resources/photos.html) | Dataset (`united-states-visa`, verified 2026-09-24) |
| USCIS | Photograph requirements (policy manual) | [USCIS Volume 7 Part A Chapter 4](https://www.uscis.gov/policy-manual/volume-7-part-a-chapter-4) | Dataset (`united-states-uscis`, verified 2026-09-24) |
| GOV.UK | UK passport photos | [gov.uk/photos-for-passports](https://www.gov.uk/photos-for-passports) | Footer, llms.txt, dataset (`united-kingdom-passport`, verified 2026-09-24) |

---

## Additional dataset citations (`verified_at` 2026-09-24)

| Dataset name | Format slug | URL |
| --- | --- | --- |
| Passport Seva photo guidance | `india-passport` | [passportindia.gov.in](https://www.passportindia.gov.in/) |
| Indian e-Visa photo requirements | `india-visa` | [indianvisaonline.gov.in e-Visa](https://indianvisaonline.gov.in/evisa/tvoa.html) |
| Australian Passport Office | `australia-passport` | [passports.gov.au PhotoGuidelines](https://www.passports.gov.au/PhotoGuidelines) |
| New Zealand Passports photo requirements | `new-zealand-passport` | [passports.govt.nz/passport-photos](https://www.passports.govt.nz/passport-photos/) |
| Department of Foreign Affairs photo guidelines (Ireland) | `ireland-passport` | [ireland.ie photo guidelines](https://www.ireland.ie/en/dfa/passports/photo-guidelines/) |
| Bundesdruckerei photo template | `germany-passport` | [bundesdruckerei.de](https://www.bundesdruckerei.de/en) |
| China visa application photo standard | `china-visa` | [visaforchina.cn](https://www.visaforchina.cn/) |
| Ministry of Foreign Affairs of Japan | `japan-passport` | [mofa.go.jp IC photo](https://www.mofa.go.jp/mofaj/toko/passport/ic_photo.html) |
| ICA photo guidelines (Singapore) | `singapore-passport` | [ica.gov.sg](https://www.ica.gov.sg/) |

`india-oci` (OCI card photo) has **no `source_url` in the public dataset**. Do not treat that row as independently cited.

---

## Product and policy pages (not government)

| Document | URL | Last updated (as published) |
| --- | --- | --- |
| Passport Size privacy policy | [privacy-policy](https://passportsize.getnorthpath.com/privacy-policy) | 23 September 2026 |
| Passport Size terms of service | [terms-of-service](https://passportsize.getnorthpath.com/terms-of-service) | 23 September 2026 |
| GetNorthPath privacy policy | [getnorthpath.com/privacy](https://www.getnorthpath.com/privacy) | 21 September 2026 |
| GetNorthPath terms of use | [getnorthpath.com/terms](https://www.getnorthpath.com/terms) | 21 September 2026 |
| GetNorthPath cookie policy | [getnorthpath.com/cookies](https://www.getnorthpath.com/cookies) | 21 September 2026 |
| Formats dataset | [JSON](https://passportsize.getnorthpath.com/data/passport-photo-formats.json) · [CSV](https://passportsize.getnorthpath.com/data/passport-photo-formats.csv) | `dateModified` 2026-09-24 · CC BY 4.0 |

---

## How to report a stale figure

The contact page asks for country, document type, and where the official requirement is published: [info@getnorthpath.com](mailto:info@getnorthpath.com). Do not attach a photo.
