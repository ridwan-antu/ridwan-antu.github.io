# Portfolio: Md. Ridwanul Islam Antu

A static personal portfolio site made with plain HTML, one CSS file and a small JavaScript file. There is no framework and no build step.

```
index.html          Home: hero, About, Education
research.html       Research map + research project cards
projects.html       Hands-on builds
experience.html     Professional + Leadership and activities
publications.html   Publications (IEEE style)
contact.html        Email and links
404.html            Not-found page (GitHub Pages uses it automatically)
.nojekyll           Tells GitHub Pages to serve files as they are
assets/css/style.css
assets/js/main.js   Mobile menu only
assets/img/         Photos (4:3, compressed), profile.jpg, favicon.svg
assets/cv/          Md-Ridwanul-Islam-Antu-CV.pdf
```

## Deploy to GitHub Pages

1. Create a GitHub account if you don't have one, and sign in.
2. Create a new **public** repository named exactly `ridwan-antu.github.io` (your GitHub username + `.github.io`).
3. Upload the files:
   - **In the browser:** open the repository and click **Add file → Upload files**. Drag in *everything inside* this folder, including the `assets` folder and `.nojekyll`, so that `index.html` sits at the top level and not inside a subfolder. Then click **Commit changes**.
   - **Or with git:**
     ```bash
     cd path/to/this/folder
     git init
     git add .
     git commit -m "Initial portfolio"
     git branch -M main
     git remote add origin https://github.com/ridwan-antu/ridwan-antu.github.io.git
     git push -u origin main
     ```
4. In the repository, go to **Settings → Pages**. Under **Build and deployment**, set *Source* to **Deploy from a branch**, then *Branch* to **main** and folder **/ (root)**, and click **Save**.
5. Wait one or two minutes, then open `https://ridwan-antu.github.io`.

To update the site later, edit the files and upload or push them again. The site redeploys automatically.

> Note: `.nojekyll` starts with a dot, so Windows Explorer may hide it. It is optional, and the site works without it.

## Editing tips

- Every unfinished item is marked `PLACEHOLDER`. Search all files for that word.
- Social links: LinkedIn and GitHub are live in every footer and on Contact. Google Scholar is commented out in each footer and is a placeholder row on Contact; add the URL and remove the `<!--` / `-->` lines when ready.
- New photos: crop them to **4:3** (for example 960 × 720 px), save as JPG at about 75–80% quality (under ~150 KB), put them in `assets/img/`, and replace the placeholder `<div class="media-placeholder">…</div>` with
  `<img src="assets/img/NAME.jpg" alt="Describe the photo" width="960" height="720" loading="lazy">`.
- Colours (gunmetal and instrument-teal theme) live at the top of `assets/css/style.css` (`:root`). Change them there and every page updates.
- Each page already has a canonical link and `og:url` pointing to `https://ridwan-antu.github.io/`. If you use a different repository name or a custom domain, update them.
