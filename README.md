# Bamboo CSS

A classless CSS utility for your HTML, which adds default styling for all HTML elements.

It's very useful when you need:

- A quick HTML/React/Vue demo without spending time styling elements
- A base style for your blog/website

Bamboo CSS uses [normalize.css](https://github.com/necolas/normalize.css/) and [sanitize.css](https://github.com/csstools/sanitize.css) to ensure consistent styling across browsers (no IE support). When using Bamboo CSS, you don't need to include `normalize.css` or `sanitize.css` anymore.

Bamboo CSS uses CSS variables for theming, allowing to dynamically change the theme if you want. By default, it provides 2 themes for light and dark modes. The theme is automatically switched based on the system mode.

All CSS variables are prefixed with `--b-`, allowing to use Bamboo CSS with any CSS framework without conflicts.

Bamboo CSS is very lightweight, only **1.67KB** (minified and gzipped).

**[Demo](https://rilwis.github.io/bamboo/demo.html)**

## Features:

- Drop in to use, no configuration, no CSS classes
- Consistent styling across browsers thanks to `normalize.css` and `sanitize.css`
- Supports light and dark themes (automatically detect the OS mode and switch)
- Uses CSS variables (scoped with prefix `--b-`)
- Uses `rem`
- Compatible with other CSS frameworks
- Lightweight

## Usage

### CDN

Use any of the link below:

```html
<link rel="stylesheet" href="https://unpkg.com/bamboo.css">

<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/rilwis/bamboo/bamboo.min.css">
```

### NPM

```bash
npm install --save bamboo.css
```

### Download

See [https://rilwis.github.io/bamboo/bamboo.min.css](https://rilwis.github.io/bamboo/bamboo.min.css)

## Credits
- [new.css](https://github.com/xz/new.css): Bamboo is a fork of new.css
- [normalize.css](https://github.com/necolas/normalize.css/) and [sanitize.css](https://github.com/csstools/sanitize.css)
- [Nord theme](https://www.nordtheme.com) for color schemes