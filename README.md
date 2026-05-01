# WEBP → JPG Converter

A fully client-side web application that converts folders of WEBP images to JPG format — no server required, everything runs in your browser.

🌐 **Live demo:** [https://alesoander.github.io/WEBP-to-PNG/](https://alesoander.github.io/WEBP-to-PNG/)

## Features

- **Folder upload** — select or drag-and-drop an entire folder of images
- **WEBP → JPG conversion** — powered by the browser's Canvas API
- **Adjustable JPG quality** — slide from 10% to 100%
- **Non-WEBP file handling** — convert other image formats too, skip them, or include them as-is
- **ZIP download** — get all converted images in a single ZIP file that mirrors the original folder structure
- **100% private** — no images are ever sent to a server

## Usage

1. Open the web page
2. Click **"Drop a folder here or click to browse"** (or drag-and-drop a folder)
3. Adjust quality and non-WEBP file handling options if needed
4. Click **"Convert & Download ZIP"**
5. A `converted_images.zip` file will be downloaded with all JPG images

## Auto-deployment

This app is automatically deployed to **GitHub Pages** on every push to `main` via the workflow in `.github/workflows/deploy.yml`.

To enable Pages in your own fork:

1. Go to **Settings → Pages**
2. Set **Source** to **GitHub Actions**
3. Push to `main` — the workflow will deploy the site automatically

## Development

The app is a single `index.html` file with no build step required. Simply open `index.html` in a browser to test locally.

## Tech stack

- HTML5 / CSS3 / Vanilla JavaScript
- [Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API) for image conversion
- [JSZip](https://stuk.github.io/jszip/) for ZIP creation (loaded from cdnjs)
- GitHub Actions + GitHub Pages for deployment
