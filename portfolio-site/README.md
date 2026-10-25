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
2. Create a new **public** repository named exactly `YOUR-USERNAME.github.io`, using your own GitHub username.
3. Upload the files:
   - **In the browser:** open the repository and click **Add file → Upload files**. Drag in *everything inside* this folder, including the `assets` folder and `.nojekyll`, so that `index.html` sits at the top level and not inside a subfolder. Then click **Commit changes**.
   - **Or with git:**
     ```bash
     cd path/to/this/folder
     git init
     git add .
     git commit -m "Initial portfolio"
     git branch -M main
     git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git
     git push -u origin main
     ```
4. In the repository, go to **Settings → Pages**. Under **Build and deployment**, set *Source* to **Deploy from a branch**, then *Branch* to **main** and folder **/ (root)**, and click **Save**.
5. Wait one or two minutes, then open `https://YOUR-USERNAME.github.io`.

To update the site later, edit the files and upload or push them again. The site redeploys automatically.

> Note: `.nojekyll` starts with a dot, so Windows Explorer may hide it. It is optional, and the site works without it.

## Editing tips

- Every unfinished item is marked `PLACEHOLDER`. Search all files for that word.
- Social links: the footer of every page has a commented-out block for LinkedIn, GitHub and Google Scholar. Add your URLs and remove the `<!--` and `-->` lines. Contact also has matching placeholder rows.
- New photos: crop them to **4:3** (for example 960 × 720 px), save as JPG at about 75–80% quality (under ~150 KB), put them in `assets/img/`, and replace the placeholder `<div class="media-placeholder">…</div>` with
  `<img src="assets/img/NAME.jpg" alt="Describe the photo" width="960" height="720" loading="lazy">`.
- Colours live at the top of `assets/css/style.css` (`:root`).
- After the site is live, add `<link rel="canonical" href="https://YOUR-USERNAME.github.io/">` in each page's `<head>`. Each page has a comment marking where it goes.
