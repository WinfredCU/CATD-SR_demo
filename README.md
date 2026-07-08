# CATD-SR Demo

This repository hosts the GitHub Pages demo website for:

**CATD-SR: Channel-Assisted and Codebook-Aware Token Denoising for Speech Restoration**

Website:

```text
https://winfredcu.github.io/CATD-SR_demo/#
```

The website is a static page. The root repository can keep the same simple structure:

```text
CATD-SR_demo/
├── Fig/
├── audio/
├── LICENSE
├── README.md
└── index.html
```

`index.html` is self-contained. No separate CSS or JavaScript files are required.

## Main website revisions

- The paper-result graph section is removed from the website.
- Experimental design, results explanation, and audio demos are combined into one section.
- The proposed-system section now explains CATD-SR step by step and highlights the novelty/contribution at each step.
- The final structured bit-error replacement demo includes benchmark audio comparisons.

## Audio files used by the page

Upload WAV files into the `audio/` folder with the following names.

### 1. I.i.d. mask corruption

```text
audio/iid_mask_clean.wav
audio/iid_mask_corrupted.wav
audio/iid_mask_catd_sr.wav
```

### 2. I.i.d. valid-token replacement

```text
audio/iid_replace_clean.wav
audio/iid_replace_corrupted.wav
audio/iid_replace_catd_sr.wav
```

### 3. Burst mask corruption

```text
audio/burst_mask_clean.wav
audio/burst_mask_corrupted.wav
audio/burst_mask_catd_sr.wav
```

### 4. Burst valid-token replacement

```text
audio/burst_replace_clean.wav
audio/burst_replace_corrupted.wav
audio/burst_replace_catd_sr.wav
```

### 5. Structured bit-error replacement with benchmark comparison

```text
audio/biterror_clean.wav
audio/biterror_corrupted.wav
audio/biterror_denoiser_only.wav
audio/biterror_catd_sr.wav

audio/biterror_rnnoise.wav
audio/biterror_facebook_denoiser.wav
audio/biterror_deepfilternet.wav
audio/biterror_fullregen.wav
```

The final demo block compares clean reference, corrupted-token decoding, denoiser-only restoration, CATD-SR with posterior fusion, and benchmark demos under the same bit-error replacement condition.

## Figure

The page currently uses:

```text
Fig/proposed_system.svg
```

You may replace it with a final figure using the same file name. For GitHub Pages, `.png`, `.jpg`, or `.svg` is recommended. Convert `.eps` files before uploading.

## GitHub Pages settings

Open the repository settings and enable:

```text
Settings → Pages → Deploy from branch → main → /(root)
```

After deployment, visit:

```text
https://winfredcu.github.io/CATD-SR_demo/#
```
