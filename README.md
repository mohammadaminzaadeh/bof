# BOYS OF FLIGHT (BOF) — Official Website

A responsive, bilingual (Persian/English) website for the BOYS OF FLIGHT game and its three-person team.

## Project structure
- `index.html` — page structure and metadata
- `assets/css/styles.css` — visual design and responsive layout
- `assets/js/main.js` — interactions and Persian/English translations
- `assets/js/site-config.js` — central editable project, team and download settings
- `assets/images/` — supplied BOF logo, favicon artwork, game visuals and team placeholders
- `downloads/BOF-Windows.zip` — Windows game package

## Run locally
Open `index.html` in a browser. For best results, use VS Code Live Server.

## Publish with GitHub Pages
1. Create a GitHub repository.
2. Upload the contents of this folder (not the outer folder itself).
3. In repository Settings → Pages, choose Deploy from a branch, select `main` and `/ (root)`.
4. Save and wait for GitHub Pages to publish the site.

## Edit project information
Most project information is centralized in `assets/js/site-config.js`.
- Game name and group name
- Download path
- Team names, roles, biographies and portrait paths
- Optional school section
- Optional group photo and social/contact links

The school section is intentionally disabled until the actual school name, approved description and image are provided. To enable it, set `school.enabled` to `true` and complete its fields.

## Replace team photos
Place approved portrait images in `assets/images/team/` and update the `image` paths in `site-config.js`. Current portrait SVG files are placeholders, not photographs.

## Replace the logo
- Main wordmark: `assets/images/bof-logo.png`
- Bird mark / favicon: `assets/images/bof-mark.png`

The supplied logo artwork was used as provided. If you later have a vector master (SVG), it can replace the PNG assets while retaining the same filenames only after updating the file extensions in `index.html` and the stylesheet.

## Windows game package
The download link points to `downloads/BOF-Windows.zip`. Extract the archive before running the executable. Keep the included `assets` directory beside the executable.

The Windows executable was renamed to `BOF.exe` and placed inside a `BOF/` folder in the archive. Renaming a packaged executable is normally supported, but test the archive on the intended Windows version before publishing.

## Important release checks
- Test the Windows package on a clean Windows computer.
- Confirm that the game starts and that all image, sound and font assets load.
- Confirm permission to redistribute the executable, artwork, sound effects and font.
- Replace placeholder team portraits only with photos approved for publication.
- Add a real group photo and school information only if you want those sections visible.
- Test both language directions and mobile navigation before publishing.

The website itself is a static HTML/CSS/JavaScript site; it does not run the Pygame game inside the browser.
