# Privacy (verified behaviour)

This page records **only** privacy and data-processing behaviour that can be verified from public Passport Size and GetNorthPath pages. It is not a substitute for the live legal documents.

**Authoritative product policy:** [passportsize.getnorthpath.com/privacy-policy](https://passportsize.getnorthpath.com/privacy-policy) (last updated **23 September 2026**).

**Parent policy (getnorthpath.com tools and forms):** [getnorthpath.com/privacy](https://www.getnorthpath.com/privacy) (last updated **21 September 2026**).

---

## Photo files

Verified claims from the privacy policy, [how-it-works](https://passportsize.getnorthpath.com/how-it-works), FAQ, and home page:

- Selecting a photo uses the browser **File API**; subsequent steps run **on the device**
- Face landmark detection, background segmentation, cropping, background replacement, JPEG encoding, and print-sheet layout are described as **in-tab**
- The privacy policy states **there is no upload endpoint** and **no server-side image processing**
- How-it-works: `/api/feedback` accepts a **written note, not a photo**
- [robots.txt](https://passportsize.getnorthpath.com/robots.txt) disallows `/api/`
- Visitor verification suggested by the site: DevTools → Network → upload and export; you should see model files if uncached, and **no request whose body is the image**
- How-it-works: after load, remaining network requests are described as **models, analytics, and embedded videos**
- Contact page and privacy policy: **do not email photos** to support

This documentation repo does not inspect private servers. The architectural claim is what the public pages and CSP `connect-src` description assert.

How-it-works states the **Content-Security-Policy `connect-src`** lists this site, analytics, Microsoft Clarity, and two model hosts, and **does not list an image-upload host**. The live `robots.txt` / document response headers observed on 5 October 2026 included `connect-src` for the site, Google Analytics, Tag Manager, Clarity, Bing, jsDelivr, and `storage.googleapis.com` (model hosting). That matches the published explanation; it is still not a forensic audit.

---

## Models downloaded to the device

From the privacy policy and how-it-works:

- Two machine-learning models and a small WebAssembly runtime download **the first time** the editor is used
- Served from **public CDNs** (how-it-works: Google’s public model host and jsDelivr; editor copy names MediaPipe face landmarks and a selfie segmenter)
- Those requests carry ordinary client metadata (IP, user agent) like any file download; they are stated **not** to include the photo
- Models are **cached** by the browser for later visits
- The site says the tool **works offline once the page has loaded** (models already cached)

---

## Email unlock and operational metadata

No account or login. To unlock a download, the site **asks for an email**.

The privacy policy states that email is sent with **operational metadata** about the download (examples listed: tool, format, file size, output type, approximate dimensions, original **filename** not image bytes, page URL). **The photo file is never uploaded.**

If environment variables are configured, those events may be forwarded to a **private Discord channel** used by the team; if not configured, events are discarded.

Optional in-editor feedback: email is used only if the team needs to follow up (on-page copy).

---

## Hosting logs and analytics

- Page requests reach the **hosting provider**; standard access logs (IP, user agent, path, timestamp) may be kept on the host’s schedule
- When configured, **Google Analytics 4** and **Microsoft Clarity** may load (first-party cookies or similar; pages viewed, device/browser, approximate location; Clarity may use **masked** session recordings and heatmaps)
- Privacy policy: analytics **do not receive the photo file**
- If analytics environment variables are not set, those scripts are **not loaded**
- A Google Analytics script id was present on the live homepage HTML on 5 October 2026 (`G-454HF7GDGB`), which is consistent with analytics being configured in production at that time

---

## Contact, children, and GetNorthPath referrals

- Emailing [info@getnorthpath.com](mailto:info@getnorthpath.com) means GetNorthPath holds the **message and email** long enough to respond and keep correspondence
- The tool is used to make photos of **children including infants**; it is **not directed at children as users**. Because no photo is transmitted, making a child’s passport photo is stated **not** to result in GetNorthPath holding the image. Metadata events may still fire
- Links to [getnorthpath.com](https://www.getnorthpath.com) carry **UTM parameters** so the parent site can see the referral source, not identity. Walkthrough or waitlist forms on GetNorthPath are covered by **GetNorthPath’s own privacy policy**

Parent privacy also states: no sale of personal information; PIPEDA access/correction/deletion requests to info@getnorthpath.com; tools meant for adults planning immigration (or helping a family member); no knowing collection from children under 13 on the parent site.

---

## What this repo does not document

- Internal Discord configuration, environment variable names, or infrastructure diagrams
- Whether a specific visitor’s analytics cookies were set
- Anything not stated on the public pages or response headers above
