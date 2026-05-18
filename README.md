# Rosé Pine for Nimbalyst

> All natural pine, faux fur and a bit of soho vibes for the classy minimalist.

A [Nimbalyst](https://nimbalyst.com) theme extension that contributes the three official [Rosé Pine](https://rosepinetheme.com) palette variants:

- **Rosé Pine** — the original soho dark
- **Rosé Pine Moon** — a softer, lower-contrast dark
- **Rosé Pine Dawn** — the warm, paper-like light variant

---

## Installation

Nimbalyst does not (yet) ship a marketplace, so installation is manual: clone this repository into the user-extensions directory for your OS, then restart the app.

### Linux

```bash
mkdir -p ~/.config/@nimbalyst/electron/extensions
cd ~/.config/@nimbalyst/electron/extensions
git clone https://github.com/omartelo/rose-pine-nimbalyst.git rose-pine
```

### macOS

```bash
mkdir -p ~/Library/Application\ Support/@nimbalyst/electron/extensions
cd ~/Library/Application\ Support/@nimbalyst/electron/extensions
git clone https://github.com/omartelo/rose-pine-nimbalyst.git rose-pine
```

### Windows (PowerShell)

```powershell
$dir = "$env:APPDATA\@nimbalyst\electron\extensions"
New-Item -ItemType Directory -Force -Path $dir | Out-Null
cd $dir
git clone https://github.com/omartelo/rose-pine-nimbalyst.git rose-pine
```

Then:

1. Restart Nimbalyst.
2. Open **Settings → Extensions** and confirm that **Rosé Pine** is listed and enabled.
3. Open the **theme picker** (in the navigation gutter) and select one of the three variants.

---

## Themes

| Theme | Mode | Background | Text | Primary |
|-------|------|------------|------|---------|
| Rosé Pine      | dark  | `#191724` | `#e0def4` | `#ebbcba` (rose) |
| Rosé Pine Moon | dark  | `#232136` | `#e0def4` | `#ea9a97` (rose) |
| Rosé Pine Dawn | light | `#faf4ed` | `#575279` | `#d7827e` (rose) |

Full palette mapping uses the official Rosé Pine roles:

- `base / surface / overlay` → `bg / bg-secondary / bg-tertiary`
- `highlight low / med / high` → `bg-hover / bg-selected / bg-active`
- `text / subtle / muted` → `text / text-muted / text-faint`
- `rose / love` → `primary / primary-hover` and `error`
- `foam` → `link` and `info`
- `iris` → `border-focus` and `link-hover`
- `pine` → `success`
- `gold` → `warning`

Domain-specific colors (tables, code blocks, scrollbar, terminal) are derived automatically by the Nimbalyst runtime from the overrides above — see [`theme-extension-guide.md`](https://github.com/nimbalyst/nimbalyst/blob/main/docs/EXTENSION_THEMING.md) §5.

---

## Updating

```bash
cd <your-extensions-dir>/rose-pine
git pull
```

Restart Nimbalyst to pick up changes.

---

## Credits

- Original palette: [Rosé Pine](https://rosepinetheme.com) — © Rosé Pine contributors, licensed under MIT.
- This port: © 2026 [omartelo](https://github.com/omartelo).

---

## License

[MIT](./LICENSE)
