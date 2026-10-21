# Saffron Atelier — VS Code Theme

A warm cream-and-beige light theme with readable charcoal text, muted olive green, soft blue, terracotta, and restrained gold accents.

## Palette

| Role | Color |
|---|---|
| Editor background | `#FBF7EF` |
| Text | `#403A32` |
| Accent (terracotta) | `#A86F4D` |
| Keywords | `#98613F` |
| Strings (olive) | `#617D58` |
| Types (soft blue) | `#587C91` |
| Numbers (gold) | `#A87927` |
| Properties (mauve) | `#98718D` |

## Install

**From VSIX (easiest):** download `saffron-atelier-x.y.z.vsix` from the [Releases](https://github.com/vasikmansuri/saffron-atelier-vscode-theme/releases) page, then in VS Code: Extensions → `...` → **Install from VSIX...**

**From source:**
```bash
git clone https://github.com/vasikmansuri/saffron-atelier-vscode-theme.git
cd saffron-atelier-vscode-theme
npx @vscode/vsce package
code --install-extension saffron-atelier-*.vsix
```

Then run **Preferences: Color Theme** → `Saffron Atelier`.

## Recommended fonts

VS Code themes can't set fonts, so add them in `settings.json`. The theme uses italics for comments, parameters, modifiers and `this`/`self`, so pick a font with a real italic.

Recommended: **[IBM Plex Mono](https://github.com/IBM/plex)**. Its warm, humanist shapes suit the palette and its italic is a true cursive. Alternatives: **[Monaspace Radon / Argon](https://monaspace.githubnext.com/)**, **[JetBrains Mono](https://www.jetbrains.com/lp/mono/)**.

```bash
brew install --cask font-ibm-plex-mono   # macOS
```

```jsonc
{
  "workbench.colorTheme": "Saffron Atelier",
  "editor.fontFamily": "'IBM Plex Mono', 'JetBrains Mono', Menlo, monospace",
  "editor.fontSize": 14,
  "editor.lineHeight": 1.7,
  "editor.fontWeight": "400",
  "editor.fontLigatures": false,
  "editor.letterSpacing": 0.2,
  "terminal.integrated.fontFamily": "'IBM Plex Mono', 'JetBrains Mono', monospace",
  "terminal.integrated.fontSize": 13,
  "terminal.integrated.lineHeight": 1.3,
  "markdown.preview.fontFamily": "'IBM Plex Sans', -apple-system, sans-serif"
}
```

> Using JetBrains Mono or Monaspace instead? Set `"editor.fontLigatures": true`.

## License

[MIT](LICENSE)
