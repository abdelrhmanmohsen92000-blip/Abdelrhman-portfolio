# Abdelrhman Mohsen — Portfolio

A single-file portfolio site (`index.html`) built for GitHub Pages.

## How to publish it on GitHub Pages

1. Create a new repository on GitHub, for example `abdelrhman-portfolio`.
   - If you want it at `https://<your-username>.github.io` directly, name the repo exactly `<your-username>.github.io`.
2. Upload these two files to the repo (drag-and-drop works on github.com, or use git):
   - `index.html`
   - `Abdelrhman_Mohsen_BIM_Architect_CV.pdf`
3. Go to the repo's **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
5. Wait a minute, then your site will be live at:
   - `https://<your-username>.github.io/<repo-name>/` (or `https://<your-username>.github.io/` if you used the special repo name above).

## Editing content later

Everything — text, colors, project list, case studies — lives in `index.html`. Open it in any text editor:
- Section text is plain HTML you can edit directly.
- Colors and fonts are defined once at the top in the `:root` / `[data-theme]` CSS blocks.
- Images are WebP for smaller file size. To add or replace one, drop a `.webp` (or convert your file to WebP first) into the `img/` folder and update the matching `src="img/...">` path.
- The featured video in the Exterior section (`img/modern-facade.mp4`) is a compressed, muted, looping walkthrough. To swap it, replace the file with the same name, or update the `<video src="...">` path and its poster image.
- The Exterior / Interior / BIM galleries use `data-category` on each `.gallery-item` to power the filter tabs — set it to `modern`, `classical`, `masterplan`, `neoclassic`, `commercial`, `documentation`, `coordination`, or `schedules` to control which tab it appears under.
- To swap the CV file, replace `Abdelrhman_Mohsen_BIM_Architect_CV.pdf` with your updated PDF using the same filename (or update the `href` in the "Download CV" button).
- Update `og:url` (in `<head>`) to your live GitHub Pages link once it's up, so link previews on WhatsApp/LinkedIn work correctly.

## Note on the CV

The uploaded CV listed `Portfolio@google.com` as a contact — this looked like a placeholder rather than a real address, so it was left out of the site. Update the contact section in `index.html` if you'd like to add a real portfolio link.
