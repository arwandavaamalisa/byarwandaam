# Arwanda Amalisa — Portfolio

A single-page, static portfolio site (plain HTML/CSS/JS — no build step) for
Arwanda Amalisa: Personal Assistant · Customer Service · Technical Virtual Assistant.

## Files

```
portfolio/
├── index.html      → all page content
├── style.css        → design system (colors, type, layout, responsive rules)
├── script.js         → mobile nav toggle + scroll-reveal animation
└── assets/           → put your CV PDF and any images here
```

## Already set up

- **Résumé PDF** — `assets/Arwanda_Nur_Fatta_Amalisa_Resume.pdf` is included
  and linked from both the hero "Download Résumé" button and the Contact
  section. If you upload a newer version later, keep the same filename (or
  update the two `href="assets/Arwanda_Nur_Fatta_Amalisa_Resume.pdf"`
  references in `index.html`).
- **Portrait photo** — `assets/profile.jpg` (pulled from your résumé) is
  displayed beside the hero text. Swap the file for a higher-res version any
  time — just keep the filename `profile.jpg`, or update the `<img
  src="assets/profile.jpg">` line in `index.html`.
- **Contact details** — email, WhatsApp, and LinkedIn in the Contact
  section are already filled in with your real info.

## Optional next steps

- Replace placeholder gradients in the "Selected Work" cards
  (`.work-thumb`) with real screenshots if you have them — swap the `<div
  class="work-thumb">` for an `<img>` tag.

## Deploying

### GitHub Pages
1. Push this folder to a new GitHub repo.
2. Repo Settings → Pages → Deploy from branch → `main` / root.
3. Your site will be live at `https://<username>.github.io/<repo>/`.

### Vercel
1. Push to GitHub.
2. Import the repo at vercel.com/new.
3. Framework preset: **Other** (it's static — no build command needed).
4. Deploy.

## Design system quick reference

- **Colors:** warm ivory paper (`#F1E7D6`), espresso text (`#2C2018`),
  antique gold accent (`#A97A3E`), deep wine accent (`#7A2B2B`) — used
  sparingly for emphasis (italic hero word, dates, hover states).
- **Type:** Fraunces (display/serif) + Work Sans (body) + IBM Plex Mono
  (labels, dates, tags) — loaded from Google Fonts.
- **Signature element:** the circular monogram seal (`A`) beside the About
  section, echoing the fine-rule dividers used throughout.

Everything is plain CSS with custom properties in `:root` at the top of
`style.css` — change a token there and it cascades through the whole site.
