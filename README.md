# Caden Lau — Game Design Portfolio

A dependency-free, responsive static website. All content is plain HTML and CSS, with replaceable project images. No JavaScript, external fonts, analytics, build process, or third-party services are required.

## Preview locally

1. Extract the ZIP archive.
2. Open `index.html` in a web browser. All project and résumé pages are linked locally.
3. Alternatively, open a terminal in this folder and run `python3 -m http.server 8000`, then visit `http://localhost:8000`.

## Edit

- `index.html` — homepage, project cards, About, and contact links.
- `projects/*.html` — six individual design case studies. Change the copy directly in the relevant HTML file.
- `assets/styles.css` — shared styles; the color variables at the top make it easy to change the palette.
- `resume.html` — public résumé page.
- `assets/caden-lau-public-resume.tex` and `.pdf` — public-safe résumé source and compiled PDF. The site links to the PDF; if you change the TeX, recompile and replace the PDF.

## Suggested next edits

- Replace the conceptual graphics with approved images (see Image guide below).
- Review the first-person descriptions for accuracy and voice. Takeaways are draft interpretations, not verified quotations.
- Add a concrete, nonconfidential design iteration example or annotated screenshot to the public digital case studies.
- The two tabletop pages now describe the broad mechanics, roster size and simulation scale. They still omit specific rules, effects, artwork and raw balance data. The public résumé remains more conservative and omits detailed card counts, simulation volume and mechanics, as well as personal phone and home location. Review the public-facing information with your business partner before publishing.
- Confirm you have permission to post any team-owned artwork, videos, or other material.

## Image guide

All six project covers are stored in `assets/images/`. Each cover is shared by its homepage card and individual project page. Replace the corresponding PNG with your own image, keeping its exact filename:

- `legends-of-the-abyss.png`
- `rainy-days.png`
- `little-wonder.png`
- `mimis-midnight-brew.png`
- `drizzle-dash.png`
- `dga-studios.png`

A 1200 × 800 or 1600 × 900 PNG works well. Covers use `object-fit: cover`, so edges may crop differently on the homepage and the project page. Keep important content near the center. To use JPEG or WebP instead, update the `src` in `index.html` and the corresponding project HTML. Update the empty `alt` text on the project page if the replacement conveys useful information.

To insert a screenshot within a project page, put the file in `assets/images/` and add this HTML inside the relevant `<section>` in `projects/your-project.html`:

```html
<figure class="project-image">
  <img src="../assets/images/example.png" alt="Describe the screenshot" loading="lazy">
  <figcaption>Explain what the image demonstrates about your design.</figcaption>
</figure>
```

Use `assets/images/` rather than `../assets/images/` when adding images to the homepage. Only publish screenshots, cards, and artwork you have permission to share.

## Publish to GitHub Pages

1. Create a public repository named `CadenLau.github.io` on GitHub, assuming that name is available under your account.
2. Upload the **contents** of this folder to the repository root (not the enclosing folder). `index.html` must be in the root.
3. Open the repository's Settings → Pages. Set the publishing source to **Deploy from a branch**, then select `main` and `/(root)` and save.
4. When GitHub finishes deploying, check the URL shown in Settings → Pages. For a user site this should be `https://cadenlau.github.io/`.

If you already have a user site, a regular project repository also works; all local links use relative paths. The site has not been published by ChatGPT.
# CadenLau.github.io
