# PDF Size Reducer

A lightweight browser-based PDF compressor built as a single HTML file.  
It helps reduce PDF file size by re-rendering pages as compressed JPEG images and rebuilding a downloadable PDF.

## Features

- Drag-and-drop PDF upload
- Adjustable image quality slider
- Progress indicator during compression
- Compression result summary with size comparison
- One-click download of compressed PDF
- Runs fully in the browser (no backend required)

## How It Works

1. Loads the selected PDF using `pdf.js`.
2. Renders each page to a canvas.
3. Converts each page to JPEG with selected quality.
4. Rebuilds a minimal PDF from those compressed page images.

## Usage

1. Open `index.html` in any modern browser.
2. Upload or drag-and-drop a PDF file.
3. Adjust quality (recommended 40-60% for balance).
4. Click **Compress PDF**.
5. Download the generated compressed file.

## Deploy on GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings -> Pages** in your repo.
3. Under **Build and deployment**, choose:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` (or your default branch)
   - **Folder:** `/ (root)`
4. Save and wait for GitHub Pages to publish.
5. Open your site at: `https://<your-username>.github.io/<your-repo>/`

Because this app is fully static and runs entirely in the browser, it works on GitHub Pages without a backend.

## Notes

- This approach works best for image-heavy PDFs.
- Text-focused PDFs may show limited reduction.
- The current UI target is to keep output under 19.5 MB where possible.

## Tech Stack

- HTML, CSS, JavaScript
- [pdf.js](https://mozilla.github.io/pdf.js/) via CDN

## Credits
- Created with assistance from the Anthropic Claude Sonnet model.
