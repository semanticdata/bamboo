# Bamboo CSS

A classless CSS utility for your HTML, which adds default styling for all HTML elements.

It's very useful when you need:

- A quick HTML/React/Vue demo without spending time styling elements
- A base style for your blog/website

Bamboo CSS uses [normalize.css](https://github.com/necolas/normalize.css/) and [sanitize.css](https://github.com/csstools/sanitize.css) to ensure consistent styling across browsers (with no IE support). When using Bamboo CSS, you don't need to include `normalize.css` or `sanitize.css` anymore.

Bamboo CSS is very lightweight, only **1.7KB** gzipped.

**[Demo](https://rilwis.github.io/bamboo/demo.html)**

## Features:

- Drop in to use, no configuration, no CSS classes
- Consistent styling across browsers thanks to `normalize.css` and `sanitize.css`
- Support light and dark themes (automatically detect the OS mode and switch)
- Lightweight

## Usage

### CDN

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/rilwis/bamboo@1.1.0/bamboo.min.css">
```

### NPM

```bash
npm install --save bamboo.css
```

### Download

See [https://rilwis.github.io/bamboo/bamboo.css](https://rilwis.github.io/bamboo/bamboo.css)

## Credits
- [new.css](https://github.com/xz/new.css): Bamboo is a fork of new.css
- [normalize.css](https://github.com/necolas/normalize.css/) and [sanitize.css](https://github.com/csstools/sanitize.css)
- [Nord theme](https://www.nordtheme.com) for color schemes