# 🥢 Bamboo CSS

<p>
<img src="https://img.shields.io/github/languages/code-size/semanticdata/bamboo" />
<img src="https://img.shields.io/github/repo-size/semanticdata/bamboo" />
<img src="https://img.shields.io/github/commit-activity/t/semanticdata/bamboo" />
<img src="https://img.shields.io/github/last-commit/semanticdata/bamboo" />
<img src="https://img.shields.io/website/https/semanticdata.github.io/bamboo.svg" />
</p>

A classless CSS library which adds nice default style for all HTML elements. It saves you a lot of time when you need to style HTML for your HTML/React/Vue demo on CodePen/CodeSandbox. It can also be used as a base style for your blog/website.

Bamboo CSS uses [modern-normalize](https://github.com/sindresorhus/modern-normalize) and [sanitize.css](https://github.com/csstools/sanitize.css) to ensure consistent styling across browsers (no IE support). When using Bamboo CSS, you don't need to include `normalize.css` or `sanitize.css` anymore.

Bamboo CSS uses CSS variables for theming, allowing to dynamically change the theme if you want. By default, it provides 2 themes for light and dark modes. The theme is automatically switched based on the system mode.

<a href="https://semanticdata.github.io/bamboo">
<img src="https://img.shields.io/badge/Check out the Demo-F0E68C?style=for-the-badge&link=https://semanticdata.github.io/bamboo" alt="demo"; />
</a>

## 🖼 Screenshots

<details>
<summary>Expand</summary>

| ![screenshot](screenshots/desktopPage960x720.png) |
| --- |
</details>

## ✨ Features

- Drop in to use, no configuration, no CSS classes
- Consistent styling across browsers thanks to `modern-normalize` and `sanitize.css`
- Responsive
- Supports light and dark themes (automatically detect the OS mode and switch)
- Uses CSS variables (scoped with prefix `--b-`)[^1]
- Uses `rem`
- Compatible with other CSS frameworks
- Lightweight (**5.3KB** (unzipped) and **1.9KB** (gzipped).)

### ⭐ Notable Features

- Uses system fonts
- Uses smooth scroll
- Disables double click on button to zoom in iOS
- Beautiful toggle panel (similar to accordion) thanks to `<details>` and `<summary>` tags
- Sets `width: 100%` for all text inputs, textarea and selects
- Sets `cursor: pointer` for checkbox, radio, image inputs and also form labels
- Sets `-webkit-appearance: none` for search input to avoid default styling in Chrome and Safari
- Sets `text-wrap: balance` for headings
- Adds a custom arrow for selects

## 🚀 Getting Started

You have many options to integrate Bamboo CSS into your project.

### 🌙/☀ Automatic Theme via CDN

```html
<link rel="stylesheet" href="https://unpkg.com/bamboo.css">
```

### 🌙 Dark Theme via CDN

```html
<link rel="stylesheet" href="https://unpkg.com/bamboo.css/dist/dark.min.css">
```

### ☀ Light Theme via CDN

```html
<link rel="stylesheet" href="https://unpkg.com/bamboo.css/dist/light.min.css">
```

### Add via NPM

```bash
npm install --save bamboo.css
```

### Download

See [bamboo/dist/bamboo.min.css](https://semanticdata.github.io/bamboo/dist/bamboo.min.css).

### Customizing

Bamboo CSS provides the following CSS variables for theming:

```css
:root {
 --b-font-main: system-ui, sans-serif;
 --b-font-mono: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;

 --b-txt: #2e3440;
 --b-bg-1: #fff;
 --b-bg-2: #eceff4;
 --b-line: #eceff4;
 --b-link: #bf616a;
 --b-btn-bg: #242933;
 --b-btn-txt: #fff;
 --b-focus: #d8dee9;
}
```

All CSS variables are prefixed with `--b-` so it's safe to use Bamboo CSS with your existing websites.

## 🔀 Workflows

### Publish Demo 📢

```yml
name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v4
      - name: Setup Pages
        uses: actions/configure-pages@v5
      - name: Upload artifact
        uses: actions/upload-pages-artifact@v3
        with:
          path: "demo"
      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v4
```

## TODO

- [ ] Change project name away from `Bamboo`.
- [ ] Add automatic builds with [Husky](https://github.com/typicode/husky).
- [ ] Integrate [New.css](https://github.com/semanticdata/bamboo/blob/main/new/new.css).

## 🔄 Changes from Upstream

- Added new *scripts* within [package.json](package.json) to build the CSS files inside the `demo` folder.
- Added [workflow](.github/workflows/) to deploy the site via GitHub Actions.

## 💜 Acknowledgements

This repository is a fork of [Bamboo CSS](https://github.com/rilwis/bamboo). Same as its predecesor [modern-normalize](https://github.com/sindresorhus/modern-normalize), and [sanitize.css](https://github.com/csstools/sanitize.css) are a source of inspiration. For color schemes we have the [Nord theme](https://www.nordtheme.com) as source.

## © License

Source code in this repository is available under the [MIT License](LICENSE).

[^1]: All CSS variables are prefixed with `--b-`, allowing to use Bamboo CSS with any CSS framework without conflicts.
