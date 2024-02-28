# none-ls-php.nvim

Native PHP diagnostic source for none-ls.nvim

Since this diagnostic was deprecated from [none-ls.nvim](https://github.com/nvimtools/none-ls.nvim)
(see [this issue](https://github.com/nvimtools/none-ls.nvim/issues/58)) because a LSP alternative is available,
this repository allows to keep using native php linter with none-ls.nvim.

**Note:** This plugin is not intended to be used alone, it is a dependency of none-ls.nvim.

## 📦 Installation

This should be used as a dependency of **none-ls.nvim**.

### [lazy.nvim](https://github.com/folke/lazy.nvim)

```lua
{
  {
    "nvimtools/none-ls.nvim",
    config = function()
        require("null-ls").register(require("none-ls-php.diagnostics.php"))
    end,
    dependencies = {
        "gbprod/none-ls-php.nvim",
    },
  },
}
```
