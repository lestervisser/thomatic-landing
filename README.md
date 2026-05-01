# thomatic.

Landing page for **thomatic.** — Thomas Krutsch, freier Videograf (Thurgau, CH).

Static single-file site. Deployed via Vercel.

## Structure

- `index.html` — full page (HTML + CSS + minimal JS for the YouTube reel)
- `vercel.json` — clean URLs + security headers
- `_design-source/` — original Claude Design handoff bundle (gitignored)

## Local preview

```sh
python3 -m http.server 4000
# open http://localhost:4000
```

## Deploy

```sh
npx vercel --prod
```

## Show reel

The hero reel embeds `https://youtu.be/CwnZzXtBNNQ` lazily — the YouTube iframe only loads after the user clicks play, so the page stays fast.
