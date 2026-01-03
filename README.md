# Contributing to meme-images

Thanks for contributing memes! 🎉  
This repository manages **all meme images and metadata** used by the meme-repo application.

---

## 🖼️ Adding memes

1. Add image files under the `images/` directory  
   Supported formats:
   - `.gif`
   - `.png`
   - `.jpg`
   - `.jpeg`
   - `.webp`

2. Follow naming guidelines:
   - Avoid spaces
   - Keep filenames short  
   Example: `confused-cat.gif`

3. Commit the image file.

---

## 🗂️ Updating metadata (`meta-data.json`)

Every meme must have a metadata entry in `meta-data.json`.

### Basic structure

```json
{
  "Id": "01234567-89ab-cdef-0123-456789abcdef",
  "Name": "Funny Cat",
  "File": "funny-cat.gif",
  "Keywords": ["cat", "funny", "meme"]
}
```
### Field descriptions

- **Id (string, required)** : A unique GUID identifying the meme.
- **Name (string, required)** : Human-readable display name.
- **File (string, required)** : Name of the file, must exactly match the filename under `images/`.
- **Keywords (array of strings, required)** : Used by the client-side search engine.
- **Optional fields (ignored by the app but allowed)**: Source, Description
---

## ✅ Validation checklist

Before submitting:

- meta-data.json is valid JSON (no trailing commas)
- File value matches the image filename exactly
- Id is present and unique
- Keywords are relevant and lowercase where possible

----

## 🧾 Removal requests (copyright / takedown)

If you believe you own the copyright to a meme and want it removed:

- Open a Removal request issue
    - (Issue template: .github/ISSUE_TEMPLATE/remove-meme.md)

- Include:
    - File path (e.g. images/funny-cat.gif) or clear identification
    - Proof of ownership (source link or documentation)
    - Optional contact information (email or GitHub handle)

We will review and remove content where appropriate.

---
## 🔗 Related Repository

Application code lives in:
👉 https://github.com/sriharshabammidi/meme-repo

Thanks for sharing memes responsibly 😄
