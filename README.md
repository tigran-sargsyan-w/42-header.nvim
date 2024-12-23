<h1 align="center">🚀 42 Header for NVIM</h1>

This plugin is whole re-write of [42header](https://github.com/42Paris/42header) in Lua.

## ✨ Features

- Command: `Stdheader`
- Auto update on save (optional)
- Supports `commentstring`

## ⚡ Requirements
- NVIM v0.10+

## 🛠️ Setup

### 📦 Packer.nvim

```lua
use {
  "tigran-sargsyan-w//42-header.nvim",
  cmd = { "Stdheader" },
  config = function()
    require "42header"setup {
      default_map = true, -- Default mapping <F1> in normal mode.
      auto_update = true, -- Update header when saving.
      user = "username", -- Your user.
      mail = "your@email.com", -- Your mail.
    -- add other options.
    }
  end,
}
```

### 😴 Lazy.nvim

```lua
{
  "tigran-sargsyan-w//42-header.nvim",
  cmd = { "Stdheader" },
  keys = { "<F1>" },
  opts = {
    default_map = true, -- Default mapping <F1> in normal mode.
    auto_update = true, -- Update header when saving.
    user = "username", -- Your user.
    mail = "your@email.com", -- Your mail.
    -- add other options.
  },
  config = function(_, opts)
    require("42header").setup(opts)
  end,
}
```

</details>
