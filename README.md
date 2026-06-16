# UTPB Geophysics & Geomodeling Lab Website

A static website for the Geophysics & Geomodeling Lab at The University of Texas Permian Basin, built with plain HTML, CSS, and a small amount of JavaScript. No build step is required, so the site can be hosted directly on GitHub Pages.

## File structure

```
.
├── index.html          Home
├── research.html       Research areas, facilities, projects
├── people.html         PI, students, alumni, collaborators
├── publications.html   Journal articles, manuscripts, conferences
├── teaching.html       Courses and mentoring
├── news.html           Lab news
├── join.html           Information for prospective students
├── css/style.css       All styles and design tokens
├── js/main.js          Mobile navigation toggle
└── images/             Place photos and figures here (see images/README.txt)
```

## Deploying to GitHub Pages

You need a free GitHub account (https://github.com). There are two ways to host the site.

### Option A: Personal site (recommended for a single main site)

1. Create a new repository named exactly `YOURUSERNAME.github.io`, replacing YOURUSERNAME with your GitHub username. Keep it Public.
2. On the repository page, choose "Add file" then "Upload files".
3. Drag all the files and folders from this package (index.html, the other .html files, css, js, images) into the upload area. Do not upload the parent folder itself; upload its contents so that index.html sits at the top level of the repository.
4. Click "Commit changes".
5. After a minute or two, the site is live at `https://YOURUSERNAME.github.io`.

### Option B: Project site (keeps your username URL free for other uses)

1. Create a new Public repository with any name, for example `utpb-geomodeling-lab`.
2. Upload the files exactly as in Option A, steps 2 to 4.
3. Go to the repository's Settings, then Pages (in the left sidebar).
4. Under "Build and deployment", set Source to "Deploy from a branch", choose the `main` branch and the `/ (root)` folder, then click Save.
5. After a minute or two, the site is live at `https://YOURUSERNAME.github.io/utpb-geomodeling-lab/`.

All links in the site are relative, so both options work without any changes to the code.

### Updating the site later

Edit a file directly on GitHub (open the file, click the pencil icon, commit) or upload a replacement file with the same name. GitHub Pages republishes automatically within a minute or two of each commit.

## Photos and figures

All twelve photos and figures are already included in the `images` folder and shown on the site. To change one later, upload a replacement with the same filename, or edit the `<img>` tag in the relevant HTML file. The filenames in use are:

| File | Used on | Content |
| --- | --- | --- |
| images/jake-lee.jpg | People | Headshot of Dr. Lee |
| images/chukwudi-onyeakusi.jpg | People | Headshot |
| images/toby-ude-akpeh.jpg | People | Headshot |
| images/jerrika-stark.jpg | People | Headshot |
| images/prasad-pothana.jpg | People | Headshot |
| images/fig-rock-physics.png | Research | Rock physics crossplot |
| images/fig-machine-learning.png | Research | ML log prediction comparison |
| images/fig-geomodeling.png | Research | 3D basin model screenshot |
| images/fig-ccus.png | Research | CO2 storage map or 4D seismic image |
| images/fig-induced-seismicity.png | Research | Earthquake relocation map |
| images/fig-geothermal.png | Research | Geothermal prospect map |
| images/lab-st1222.jpg | Research | Lab workstation photo |

## Adding a CV link

Create a folder named `cv` in the repository, upload your CV PDF (for example `cv/Jake-Lee-CV.pdf`), then open `people.html` and uncomment the CV link in the `pi-links` section.

## Customizing colors and fonts

All design tokens live at the top of `css/style.css` in the `:root` block. Changing `--accent` updates the orange accent everywhere; changing `--ink` updates the navy. Fonts are loaded from Google Fonts in the `<head>` of each page; replace the font names there and in the `--font-*` variables to switch typefaces.

## Verifying before launch

All twelve photos and figures are already placed, and the "UTPB Geology M.S. program" button on the Join Us page points to the program page. The site is ready to publish as is. If you want to change any photo later, replace the file in the `images` folder with one of the same name, or edit the `<img>` tag in the relevant HTML file.
