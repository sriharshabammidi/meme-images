# 🖼️ Meme Images

This repository contains **all meme assets** used by the Meme Repo application.

It is responsible for:
- Meme image files
- Meme metadata (`meta-data.json`)
- Hosting assets via **GitHub Pages**

The application logic and UI live in a separate repository:  
👉 https://github.com/sriharshabammidi/meme-repo

---

## 📦 What This Repo Contains

### 🖼️ Images
- Located under the `images/` directory
- Supported formats:
  - `.gif`
  - `.png`
  - `.jpg`
  - `.jpeg`
  - `.webp`

### 🗂️ Metadata
- `meta-data.json` contains searchable metadata for all memes
- Used by the client-side search engine in `meme-repo`

---

## 🌐 Hosting

This repository is hosted using **GitHub Pages** and serves as a static asset CDN.

Base URL: https://sriharshabammidi.github.io/meme-images

Assets are consumed dynamically by the UI using this base URL.

---

## 🗂️ Repository Structure
```
meme-images/
├── images/
│ ├── meme1.webp
│ ├── meme2.gif
│ └── ...
├── meta-data.json
└── README.md
```
## 🧠 Metadata Format (`meta-data.json`)

Each meme must have an entry in `meta-data.json`.

### Example

```json
{
  "Id": "01234567-89ab-cdef-0123-456789abcdef",
  "Name": "Funny Cat",
  "File": "funny-cat.gif",
  "Keywords": ["cat", "funny", "meme"]
}
```
### 🔗 Related Repository

Application UI and logic:
👉 https://github.com/sriharshabammidi/meme-repo

## 🤝 Contribution Guidelines
- Keep all UI and logic changes in `meme-repo`

- Keep all images and metadata in `meme-images`

- Ensure configuration changes go through config.js

- Read more on [CONTRIBUTING.md](/CONTRIBUTING.md)

### 📄 License

All images belong to their respective owners.

This repository is intended for educational and demonstrational purposes.
