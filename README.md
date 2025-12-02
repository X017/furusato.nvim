# Furusato.nvim
> **“Furusato” (ふるさと)** — *a cozy place you return to.*

A dark, modern Neovim colorscheme with soft blues, greys, and subtle contrasts.  
Supports Treesitter, LSP, Git signs, Telescope, and file explorers (NvimTree / Neo-tree).

## ✨ Features
- Full **Neovim** colorscheme (`colors/furusato.lua`)
- **Transparent background** option
- Configurable **italics** (comments, keywords, functions, variables)
- **Treesitter** highlight groups
- **LSP diagnostics** + LspReference highlights
- **GitSigns** colors
- **Telescope** styling
- **NvimTree / Neo-tree** support
- **Mini.statusline** integration

## 📦 Installation

### Lazy.nvim
```lua
{
  "x017/furusato.nvim",
  lazy = false,
  priority = 1000,
  config = function()
    vim.g.setup = {
      transparent = false,
      italic_comments = true,
      italic_keywords = false,
      italic_functions = false,
      italic_variables = false,
    }
    vim.cmd("colorscheme furusato")
  end
}
```

### Packer
```lua
use {
  "x017/furusato.nvim",
  config = function()
    vim.g.setup = {}
    vim.cmd("colorscheme furusato")
  end
}
```

### Manual
Place the file at:

```
~/.config/nvim/colors/furusato.lua
```

Then:

```
:colorscheme furusato
```

## ⚙️ Configuration

All configuration uses `vim.g.setup`:

```lua
vim.g.setup = {
  transparent = true,
  italic_comments = true,
  italic_keywords = false,
  italic_functions = false,
  italic_variables = false,
}
```

## 🎨 Palette Overview

Furusato uses muted cool tones:

- Blues + sea-blues
- Muted pinks
- Warm yellows
- Soft greys
- Dark minimal background

## ✔️ Supported Integrations
- Treesitter (`@variables`, `@functions`, etc.)
- LSP diagnostics + references
- GitSigns
- Telescope UI
- NvimTree + Neo-tree
- Mini.statusline

---

Enjoy the Furusato atmosphere 🌙
