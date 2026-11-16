# The Leaf — free personal mathematics website

This is a simple, responsive static website designed for GitHub Pages. It uses plain HTML and CSS, with MathJax loaded from a public CDN to render LaTeX equations.

## Files
- `index.html` — homepage
- `writing.html` — writing archive
- `research.html` — research page
- `notes.html` — mathematical notes (includes a sample LaTeX note)
- `about.html` — the story and philosophy behind The Leaf
- `assets/style.css` — all visual styling

## Publish with GitHub Pages (free)

1. Sign in at https://github.com/ and create a new **public** repository.
2. Name it `the-leaf` (or another name you like). Do not add a README if you are uploading these files as-is.
3. Download and unzip this folder on your computer.
4. Open the repository on GitHub, choose **Add file → Upload files**, and upload the *contents* of this folder (the HTML files, `assets` folder, and README).
5. Commit the files to the `main` branch.
6. Open **Settings → Pages**.
7. Under **Build and deployment**, choose **Deploy from a branch**.
8. Select branch `main`, folder `/ (root)`, then Save.
9. Wait a few minutes. Your site will appear at `https://YOUR-USERNAME.github.io/the-leaf/`.

For a personal site at `https://YOUR-USERNAME.github.io/`, the repository must be named exactly `YOUR-USERNAME.github.io`.

## How to edit
- Change text directly in the relevant `.html` file using GitHub's pencil/Edit button.
- Change colors and typography in `assets/style.css`, inside the `:root` variables near the top.
- To add a new page, copy an existing HTML page, change its title and content, and add a navigation link in each page's header.

## Writing LaTeX
MathJax is already included in `index.html` and `notes.html`. For other pages that need equations, add these three script tags inside the `<head>` (the polyfill line is optional; MathJax itself is the important one):

```html
<script defer src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
```

Inline formula: `\( f(x)=x^2 \)`

Display formula:
```latex
\[
\lim_{n\to\infty} a_n = L.
\]
```

## Important
- GitHub Pages hosting is free for public repositories.
- You do not need to buy a domain. The default `github.io` address is enough.
- Do not publish private information such as your home address, school timetable, or personal phone number.
