# Terraformer design system (HTML reference)

Static reference for **Terraformer** tokens — not a separate visual language.

**Live:** [https://irene573.github.io/reference-design-system/](https://irene573.github.io/reference-design-system/)

**Source of truth:** [world-client/terraformer/design/system](https://github.com/Overworldai/world-client/tree/main/terraformer/design/system)

## What’s on the page

- **Colors** — `#d9d9d9` (chrome) and `#2a2a2a` (node caption)
- **Typography** — **Overused Grotesk** + **Fragment Mono** (Terraformer’s shipped mono; weights and sizes with real call sites)
- **Text padding** — panel header/body, log/response bubbles, composer, buttons (values from design/system + `ui.ts`)

## Local

```bash
python3 -m http.server 8765
```

Fonts are self-hosted under `fonts/` (copied from `terraformer/public/fonts/`).

## Sync CSS tokens

```bash
cp world-client/terraformer/design/system/tokens/{colors,typography,spacing,effects}.css \
  reference-design-system/css/terraformer/
```
