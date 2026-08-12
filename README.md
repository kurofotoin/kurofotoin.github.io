# Kurofotoin — Landing Page

Simple one-page portfolio site for Kurofotoin photography studio. Pure HTML/CSS/JS — no build step, no framework, so it deploys straight to GitHub Pages.

## Structure

```
index.html   — all page content/sections
style.css    — design system + layout
script.js    — nav toggle, footer year, scroll-reveal
assets/      — logo files
assets/work  — photo files

```

## Run locally

Just open `index.html` in a browser, or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Push this folder to a GitHub repo.
2. Go to **Settings → Pages**.
3. Under "Build and deployment", set **Source: Deploy from a branch**.
4. Pick the `main` branch and `/ (root)` folder, then Save.
5. Your site will be live at `https://<username>.github.io/<repo-name>/` in a minute or two.

## Things to swap before launch

- **Portfolio images** — the 6 boxes in the Work section are striped placeholders (`.frame__ph` in `style.css`). Replace each with a real photo: add `<img src="assets/work/xxx.jpg" alt="...">` inside the `.frame` div, above or in place of the `.frame__ph` div.
- **Testimonials** — the three quotes in the Testimonials section are sample copy. Swap in real client quotes once you have them.
- **WhatsApp number** — the "Message on WhatsApp" button currently points to `+62 877-7700-3015`. Update the `wa.me` link in `index.html` if you'd rather route to the other number.
- **Instagram link** — currently points to `instagram.com/kurofotoin`.

## Notes on the design

- Palette is pure black/white/gray — no color accent. That's intentional: it mirrors 黒 (kuro), "black," the word in your own name and logo.
- Headings use Noto Sans JP Bold/900, body text uses Noto Sans JP Regular, per your brand font.
- The large faint 黒 kanji watermark repeats in the hero and testimonials section as a recurring brand mark.
