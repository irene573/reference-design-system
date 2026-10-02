# References · Terraformer Design System

HTML/CSS patterns for **citations and source metadata**, styled with the same tokens as [Terraformer’s design system](https://github.com/Overworldai/world-client/tree/main/terraformer/design/system) (near-black canvas, light chrome, flat surfaces, `--tf-edge-*` for links and accents).

## Quick start

**Live preview:** [https://irene573.github.io/reference-design-system/](https://irene573.github.io/reference-design-system/)

**Local:**

```bash
cd reference-design-system
python3 -m http.server 8765
```

Open [http://127.0.0.1:8765/](http://127.0.0.1:8765/).

## Structure

| Path | Purpose |
| --- | --- |
| `css/styles.css` | Single entry (imports Terraformer tokens + reference components) |
| `css/terraformer/*.css` | Copy of `terraformer/design/system/tokens/` — sync when tokens change |
| `css/base.css` | Docs shell, section layout |
| `css/components.css` | `ref-*` citation/bibliography components |
| `index.html` | Specimens |

## Usage

Link one stylesheet:

```html
<link rel="stylesheet" href="css/styles.css" />
```

Use semantic Terraformer variables in custom markup (`--surface-chrome`, `--text-primary`, `--tf-edge-blue`, …). Reference-specific classes use the `ref-` prefix (see `index.html`).

## Syncing tokens

When Terraformer tokens change in world-client, refresh this repo:

```bash
cp world-client/terraformer/design/system/tokens/{colors,typography,spacing,effects}.css \
  reference-design-system/css/terraformer/
```

Brand fonts (Overused Grotesk) ship with the main design system under `assets/fonts/`; this site uses system-ui fallbacks plus Fragment Mono from Google Fonts until self-hosted files are added.
