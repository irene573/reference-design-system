# Reference Design System

A static HTML/CSS design system for citation and reference UI: inline markers, footnotes, bibliography lists, source cards, and callouts.

## Quick start

**Live preview (no setup):** [https://irene573.github.io/reference-design-system/](https://irene573.github.io/reference-design-system/)

**Local preview:** the site is plain static files. Either open `index.html` in a browser, or start a server in this folder (the URL only works while the command is running):

```bash
cd reference-design-system
python3 -m http.server 8765
```

Then visit [http://127.0.0.1:8765/](http://127.0.0.1:8765/) (use `127.0.0.1` if `localhost` fails).

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
