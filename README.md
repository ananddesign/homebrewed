# Brewed by Anand — the listening corner

My portfolio as a sunlit coffee-and-vinyl corner, built with Three.js. Scroll and the camera walks through the room, from the intro to each project to a night-time "let's talk". Every record on the wall is a project; open one and its case study slides up in place over the room.

- **Intro → about → six projects → skills → contact**, with the sun setting as you scroll
- **Case studies open in the page**: Price Genie, QWEEN, JUGL, Imagio, CityScope, Design Cop
- **Everything in the room is clickable**: records play their own lo-fi loop on the turntable, mugs swing, the espresso machine pulls a shot, drawers open
- Golden hour / night toggle, sound toggle, film grain

## Run it

It's a single static file. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Direct links open a case study: `index.html#price-genie`, `#qween`, `#jugl`, `#imagio`, `#cityscope`, `#design-cop`, `#about`, `#resume`, `#contact`.

## Editing

All content lives near the top of the script in `index.html`:

- `RECORDS` — title, summary, facts, links, cover style and music loop for each record
- `CASES` — the sections of each in-page case study
- The story chapters are the `<section class="ch">` blocks in the markup

Three.js r128 loads from cdnjs; fonts from Google Fonts. Everything else (textures, covers, sounds) is generated in code.

Full case studies: [brewedbyanand.com](https://www.brewedbyanand.com/)
