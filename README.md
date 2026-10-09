# Harikrishnan S · Stardew-style portfolio

https://adu773.github.io/Harikrishnan-S/

A single-file, pixel-art portfolio inspired by Stardew Valley. No build step and no dependencies;
the only external request is Google Fonts.

```
index.html                  ← the whole site (HTML + CSS + JS + every sprite)
Harikrishnan_S_Resume.pdf   ← linked by the "Résumé" / "Download résumé" buttons
```

## Host it

Pick one; each takes about two minutes:

- **GitHub Pages**: create a repo, upload both files, then go to *Settings → Pages → Deploy from branch → `main` / root*.
  The site appears at `https://<username>.github.io/<repo>/`.
- **Netlify Drop**: drag this folder onto <https://app.netlify.com/drop>.
- **Vercel / Cloudflare Pages**: import the folder as a static site with no build command.

You can also just double-click `index.html` to open it locally.

## Edit it

Everything lives in `index.html`:

- **Text content**: each section is plain HTML (`#about`, `#skills`, `#experience`, `#projects`,
  `#education`, `#certs`, `#contact`). Edit the text in place.
- **Inventory items**: each `<button class="item">` sets its tooltip with `data-name`, `data-item`
  and `data-desc`, and its icon with `data-s` (the sprite name).
- **Sprites** are text grids in `window.SV_SPRITES` (one sprite per line). Each character is a
  palette colour key and `.` is transparent.
- **Résumé**: replace `Harikrishnan_S_Resume.pdf`, keeping the same file name.

## Things to try on the page

- Click the **date** in the clock to cycle seasons. Click the **sun/moon** to cycle day → dusk → night.
  By default both follow the visitor's real date and time.
- Hotbar keys **1–8** jump between sections. **9** waters the project crops, **0** digs up a Junimo,
  and **-** shakes the trees.
- Open a project ("Inspect crop") for full details. SmartNav360 includes a Dijkstra routing demo and
  Tic Tac Toe is playable.
- Pet the cat, click the chickens and Junimos, and fill all 10 friendship hearts.

*Fan-made tribute; not affiliated with or endorsed by ConcernedApe.*
