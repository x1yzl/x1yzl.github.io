# x1yzl — portfolio

My personal portfolio. Dark, minimal, a bit over-engineered. Built as a single HTML file so I can just drop it anywhere without dealing with build tools or deployment pipelines.

## stack

- Plain HTML + CSS + React (loaded via CDN, compiled in-browser with Babel)
- No build step, no bundler, no node_modules — just open the file
- Particle canvas background, custom cursor, scroll-triggered animations

## structure

```
portfolio.html   <- everything lives here, self-contained
uploads/         <- project screenshots and assets
portrait.png     <- profile photo
```

## running it

Just open `portfolio.html` in a browser. That's it.

If you want to serve it locally for any reason:

```bash
npx serve .
# or
python -m http.server
```

## sections

- Hero
- About
- Skills
- Projects
- Services
- Contact

## notes

The accent color, particle count and a couple other things are tweakable through a hidden panel — it shows up when the page receives an `__activate_edit_mode` message (used during development). In production it just stays hidden, doesn't affect anything.