# Reference Design System

A static HTML/CSS design system for citation and reference UI: inline markers, footnotes, bibliography lists, source cards, and callouts.

## Quick start

Open `index.html` in a browser, or serve the folder locally:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Structure

| File | Purpose |
| --- | --- |
| `css/tokens.css` | Design tokens (color, type, space, radius) |
| `css/base.css` | Reset, page layout, typography defaults |
| `css/components.css` | Reference UI components |
| `index.html` | Living documentation and examples |

## Usage

Link the stylesheets in order:

```html
<link rel="stylesheet" href="css/tokens.css" />
<link rel="stylesheet" href="css/base.css" />
<link rel="stylesheet" href="css/components.css" />
```

Copy the markup patterns from `index.html` and adjust content. All components use the `ref-` prefix and BEM-style modifiers (e.g. `ref-cite--superscript`).

## Customization

Override tokens on `:root` or a wrapper (e.g. `.ref-theme-dark`) to retheme without touching component rules.
