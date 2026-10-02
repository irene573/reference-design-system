# Terraformer Design System (HTML reference)

A simple static page for **Terraformer foundations**: typography, colors (`#d9d9d9` chrome, `#2a2a2a` node caps, `#141414` canvas), spacing, and radii. Tokens are copied from [world-client/terraformer/design/system](https://github.com/Overworldai/world-client/tree/main/terraformer/design/system).

**Live:** [https://irene573.github.io/reference-design-system/](https://irene573.github.io/reference-design-system/)

## Local

```bash
python3 -m http.server 8765
```

Open [http://127.0.0.1:8765/](http://127.0.0.1:8765/).

## Files

| Path | Purpose |
| --- | --- |
| `css/styles.css` | Entry — imports tokens + layout |
| `css/terraformer/*.css` | Synced from `terraformer/design/system/tokens/` |
| `css/foundations.css` | Specimen layout |
| `index.html` | The reference page |

## Sync tokens from world-client

```bash
cp world-client/terraformer/design/system/tokens/{colors,typography,spacing,effects}.css \
  reference-design-system/css/terraformer/
```
