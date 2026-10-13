# Personal Portfolio

**My portfolio site: featured projects, a startup pitch, the five-architecture task board series, my toolbox and certifications.**

🔗 **Live:** https://tawan230666.github.io/

![HTML](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub_Pages-222222?logo=githubpages&logoColor=white)

## Design decisions

- **No framework, no build step.** The page is one HTML file, one stylesheet and about 20 lines of JavaScript, so it loads fast and deploys straight from `main` to GitHub Pages.
- **Images prepared for the web.** Event photos were resized, denoised and sharpened with OpenCV, and the pitch deck was re-exported from 28 MB to a 1.5 MB PDF plus lazy-loaded slide images. Phone numbers on the project poster were removed before publishing.
- **Content first.** Every project card links to a real repository, and every number on the page (such as 0.91 mAP@50) comes from that project's README.
- **Light and dark themes.** Colours are CSS custom properties. The site follows the OS setting by default, and the toggle remembers the visitor's choice (with a safe fallback when storage is blocked).
- **Responsive and accessible.** One-column layout on phones with no horizontal scroll, a skip link, semantic landmarks, descriptive `alt` text, and `prefers-reduced-motion` support.

## Structure

```
index.html        page content
css/style.css     design tokens, layout, light/dark themes
js/main.js        theme toggle and footer year
assets/           favicon, startup pitch photos, slides and deck PDF, certificates
```

## Run locally

```bash
git clone https://github.com/tawan230666/tawan230666.github.io.git
cd tawan230666.github.io
python3 -m http.server 8000   # then open http://localhost:8000
```
