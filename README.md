# juanmaguzman.github.io

Personal site: plain HTML + CSS, no build step.

- `index.html`: the page
- `style.css`: styles (white background, near-black text, one blue accent)
- `cv/`: copies of the PDFs from `~/Personal/resume`. Re-copy them after rebuilding the CV:
  `cp ~/Personal/resume/Juan-Martin-Guzman-Salas_CV_*.pdf ~/Personal/website/cv/`

## Publish on GitHub Pages (first time)
1. On GitHub, create a **public** repo named exactly `juanmaguzman.github.io` (empty, no README).
2. From this folder:
   ```sh
   git init -b main
   git add .
   git commit -m "Personal site"
   git remote add origin https://github.com/JuanmaGuzman/juanmaguzman.github.io.git
   git push -u origin main
   ```
3. Repo → Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
4. After a minute or two the site is live at https://juanmaguzman.github.io

## Update
Edit, then `git add . && git commit -m "Update" && git push`.
