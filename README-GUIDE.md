# TahmidCZ GitHub Profile — Setup Guide

A black-and-neon-violet cyberpunk profile README for **MD Tahmidul Islam** (`TahmidCZ`).

## 1. Upload the project to GitHub

1. Sign in to GitHub and open [github.com/new](https://github.com/new).
2. Create a **public** repository named exactly `TahmidCZ` (the repository name must match your username).
3. Upload `README.md`, the `assets/` folder, and the `animations/` folder from this project. You can upload the entire unzipped folder contents using **Add file → Upload files**.
4. Commit the files to the repository's `main` branch.
5. Open `https://github.com/TahmidCZ` to see the profile README.

You can also use Git:

```bash
git clone https://github.com/TahmidCZ/TahmidCZ.git
# Copy this project's contents into the cloned repository.
cd TahmidCZ
git add .
git commit -m "Create cyberpunk GitHub profile"
git push origin main
```

## 2. Replace each image

The README references these local files:

| File | Purpose |
|---|---|
| `assets/hero.svg` | Static hero title banner |
| `assets/about-life.svg` | About / interests banner |
| `assets/stack.svg` | Skills and technology layout |
| `assets/id-dashboard.svg` | Developer ID card |
| `assets/connect.svg` | Contact banner |
| `animations/hero.gif` | Animated workstation artwork |
| `animations/contributions.gif` | Decorative animated city artwork |

Keep the filenames and folders unchanged if you do not also update the matching paths in `README.md`.

To replace an image, upload your new file to the same path and filename. For a new image name, update the corresponding Markdown `src` attribute.

## 3. Change the anime hero artwork

`animations/hero.gif` is the animated anime-inspired workstation image. Replace it with artwork you own or are licensed to use. For a static image, use PNG or WebP and update the README:

```html
<img src="assets/my-hero.webp" alt="My developer banner" width="100%">
```

The SVG hero title banner (`assets/hero.svg`) is separate from the anime artwork. Edit its text in a vector editor or a text editor. Keep the SVG XML valid.

## 4. Customize the colors

The current palette is black, deep violet, neon purple, and lavender. In the SVG files, the main color values are:

- Background: `#080610`
- Panel: `#120d20`
- Neon purple: `#a855f7`
- Violet: `#7c3aed`
- Lavender: `#c4b5fd`
- Main text: `#f5f3ff`

Use your editor's **Find and Replace** to update these values consistently across all five SVGs. The GitHub statistics cards use URL parameters such as `bg_color=080610`, `title_color=c084fc`, and `icon_color=a855f7`; update those separately in `README.md`.

## 5. Add technology icons

You can add shields.io badges under the appropriate skill group in `README.md`. Example:

```markdown
![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white)
```

Only add technologies you actually use. Keep development skills separate from creative and office tools.

## 6. Update projects

When you have a public project repository, replace the Coming Soon placeholder in the **Projects** section with a real link:

```markdown
- [Project name](https://github.com/TahmidCZ/your-real-repository) — A short, accurate description.
```

Do not add a repository or achievement until it exists and the description is accurate.

## 7. Change animation GIFs

Replace `animations/hero.gif` or `animations/contributions.gif` with another optimized GIF using the same filename. Keep animations subtle and loopable; smaller dimensions and fewer colors generally reduce file size.

The contributions animation is explicitly decorative, not a contribution graph. If you later add a real contribution visualization, use a data-backed source and label it accurately.

## 8. Troubleshoot broken image links

- **Check spelling and capitalization:** GitHub paths are case-sensitive.
- **Check the branch:** the files must be committed to the repository's default branch.
- **Check the relative path:** from `README.md`, use `assets/hero.svg`, not a local computer path.
- **Check the raw file:** open the image file in the repository and confirm GitHub can display it.
- **Check SVG syntax:** ensure the file starts with `<svg ...>` and all tags/attributes are valid XML.
- **Check external services:** GitHub stats and activity graph cards are hosted by third-party services; they may be temporarily unavailable or rate-limited.
- **Use a local fallback:** if an external card fails, remove it or replace it with a locally hosted image.

## 9. Markdown and HTML image examples

Markdown:

```markdown
![Hero banner](assets/hero.svg)
```

HTML (useful for alignment and width):

```html
<div align="center">
  <img src="assets/hero.svg" alt="Hero banner" width="100%">
</div>
```

GitHub sanitizes README HTML and does not allow arbitrary JavaScript or CSS. Use GIFs or supported image formats for animation.

---

**Profile repository:** [github.com/TahmidCZ](https://github.com/TahmidCZ)  
**Contact:** [webdevelopertahmid@gmail.com](mailto:webdevelopertahmid@gmail.com)
