# Hotemet — Mobile Watermark Tool

A lightweight, privacy-focused web app for adding a logo or watermark to images directly on a phone or computer.

The interface is designed mobile-first, supports Hebrew RTL, and works on iPhone, Android, and desktop browsers.

## Features

- Upload a photo and a logo directly from the device
- Apply a single watermark or a repeating watermark pattern
- Adjust size, opacity, spacing, and position
- Drag the logo directly on the image
- Save the selected logo and settings locally for future use
- Quick Mode: automatically process and download every newly selected image
- Export as JPG, PNG, or WEBP
- Install on the home screen as a Progressive Web App (PWA)
- No account, backend, or server-side image processing required

## Privacy

Image processing is performed locally in the browser using Canvas. Photos and logos are not uploaded by this application to an external server.

The selected logo and preferences may be stored on the device using IndexedDB and localStorage so they are available the next time the app is opened. Clearing browser data may remove these saved items.

If the app is hosted by a third-party provider, that provider may still collect ordinary technical request data such as IP addresses, browser details, or access logs under its own privacy policy.

## Using the App

1. Select a photo.
2. Select a logo.
3. Choose a single or repeating watermark.
4. Adjust the watermark settings and position.
55555555555.
5Select **Download protected image**.

### Quick Mode

After choosing and positioning a logo, enable **Quick Mode**. Each new photo selected afterward will be processed and downloaded automatically using the saved settings.

## Install on a Phone

### iPhone

Open the hosted website in Safari, tap **Share**, and select **Add to Home Screen**.

### Android

Open the hosted website in Chrome and select **Install app** or **Add to Home screen**.

## Run Locally

The app is static and has no build step. It can be opened directly from `index.html`, but running a local web server is recommended for PWA and offline-cache features:

```bash
python -m http.server 4173
```

Then open `http://localhost:4173`.

## Deployment

Publish the repository as a static website using GitHub Pages, Cloudflare Pages, Netlify, or another static hosting provider.

Core files:

- `index.html`
- `styles.css`
- `app.js`
- `sw.js`
- `manifest.webmanifest`

## Browser Support and Limitations

Modern versions of Safari, Chrome, Edge, and Firefox are recommended. Very large images, unsupported image formats, limited device memory, browser restrictions, or operating-system behavior may affect performance or output quality. Users should verify downloaded images before deleting or replacing originals.

## Responsible Use

You are responsible for ensuring that you have the necessary rights and permissions to use every photo, logo, trademark, or other asset processed with this tool. Do not use the tool to infringe copyright, trademark, privacy, publicity, contractual, or other legal rights.

A watermark may discourage casual copying, but it does not guarantee ownership protection, prevent removal, establish copyright, or provide complete security.

## Disclaimer and Limitation of Liability

This project and its software are provided **“as is”** and **“as available,”** without warranties of any kind, express or implied, including warranties of accuracy, reliability, availability, fitness for a particular purpose, non-infringement, or preservation of image quality or data.

Use of the software is entirely at your own risk. To the fullest extent permitted by applicable law, the project owner, authors, contributors, and hosting providers shall not be liable for any direct, indirect, incidental, special, consequential, exemplary, or other damages or losses arising from or related to the software or its use. This includes, without limitation, loss of files or data, reduced image quality, failed downloads, unauthorized copying, misuse of images or logos, intellectual-property claims, business interruption, or loss of profits.

Users are responsible for maintaining backups, reviewing the generated output, complying with applicable laws and third-party terms, and obtaining any necessary professional advice. Nothing in this README constitutes legal advice, and no statement here excludes liability that cannot lawfully be excluded.

## Security

Do not add passwords, API keys, access tokens, private customer images, or other secrets to the repository. If you discover a security issue, report it privately to the repository owner rather than publishing sensitive details in a public issue.

## Contributions

Suggestions and pull requests are welcome. By contributing, you confirm that you have the right to submit your contribution and understand that it may become publicly visible.

## Copyright and License

Copyright © 2026 Chen Goren. All rights reserved.

Making this repository publicly viewable does not by itself grant permission to copy, modify, redistribute, sublicense, or commercially use its source code or assets. A separate license may be added later if broader reuse is intended.
