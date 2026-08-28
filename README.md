<p align="center">
  <img src="https://hub.buildauthority.com/logo.webp" alt="Builders of Authority" width="180">
</p>

# BOA - Mallory Portraits - Landing Page

Static landing page for **Mallory Portraits**, a heirloom family portrait studio in Portsmouth, New Hampshire. Built by **Builders of Authority** as a client-facing presentation build and as a reference layout for rebuild inside the GoHighLevel website builder.

No build step, no dependencies. Plain HTML and CSS.

---

## Contents

```
index.html        Main landing page
thank-you.html    Post-submission page
favicon.svg       Site icon
images/           12 web-optimised portraits (2.4 MB total)
.gitignore
README.md
```

## Run it locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploy to Vercel

Import the repo at [vercel.com/new](https://vercel.com/new). Framework preset: **Other**. Leave build command and output directory blank. Deploy.

---

## Design tokens

| Token | Hex | Use |
| --- | --- | --- |
| Ink | `#101215` | Dark gallery sections |
| Slate | `#191C21` | Footer |
| Ivory | `#F1ECE3` | Mat board, light type |
| Paper | `#FAF8F3` | Light sections |
| Brass | `#B08B4F` | Single accent, buttons, rules |
| Stone | `#8A8378` | Captions, labels |

**Type:** Cormorant Garamond (display) and Jost (body), both loaded from Google Fonts.

**Signature element:** every portrait sits inside a mat with a hairline brass frame, so the page demonstrates the offer itself. Portraits on a wall, not files on a phone.

---

## GoHighLevel rebuild map

Each section is a plain row and column stack. Nothing here needs custom code in GHL.

| Section | GHL structure |
| --- | --- |
| Hero | 2-column row, text left, image right |
| The years go by | 1-column text row, then 3-column stat row |
| The experience | 3-column row |
| Beautiful today | 2-column row, image left, text right |
| Get in the frame | 2-column row, text left, image right |
| Gallery | One 3-column row, three images stacked per column |
| Reviews | 3-column row |
| CTA and form | 1-column row, form centred |
| Footer | 1-column row |

Both fonts are in the GHL font picker. Recreate the frame effect with a container that has ivory background, 14px padding, and a 1px `#B08B4F` inner border.

---

## Before launch

- [ ] Replace the HTML form with a native GHL form and set its redirect to the thank-you page. The current form does not capture leads.
- [ ] Confirm the 14,000 families and 550+ reviews figures are current.
- [ ] Confirm review names and wording are approved for public use.
- [ ] Add tracking (GA4, Meta pixel, or GHL tracking) if the page will run paid traffic.
- [ ] Swap `favicon.svg` for the studio's own mark once supplied.

---

Builders of Authority
