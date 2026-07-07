# Codebook-Assisted Selective Token Denoising Demo

This repository is a GitHub Pages demo website for:

**Codebook-Assisted Selective Token Denoising for Neural Codec-Based Speech Restoration**

Authors: Zewei Wang, Tat Ming Lok, and Yao Tang.

## Structure

```text
.
├── index.html              # Main demo website
├── css/style.css           # Page style
├── js/main.js              # Small audio helper: pause other clips when one plays
├── Fig/                    # System and experiment figures
├── audio/                  # Audio demos
├── .nojekyll               # Disable Jekyll processing
└── README.md
```

## How to deploy with GitHub Pages

1. Create a new public GitHub repository, for example `CodebookSelectiveTokenDenoising_demo`.
2. Upload all files in this folder to the repository root.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/ (root)`
5. The website will be available at:

```text
https://<your-github-username>.github.io/<repo-name>/
```

## How to add your demos

Replace the placeholder paths by uploading `.wav` files into the `audio/` subfolders. The required filenames are listed in `audio/README.md`.

## How to update figures

Replace the placeholder SVG files in `Fig/` with your final figures. Keep the same filenames, or update the image paths in `index.html`.

## Notes

The page is intentionally static and does not require Node.js, Python, or a build step.
