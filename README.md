# plg
Simple CLI Neovim plugin manager. This program is basically a thin wrapper
around `git clone`, nothing special. To manage plugins with `plg`:

1. Create a configuration at `~/.config/nvim/plugins.sh`, example:
```bash
# List of packages to clone (from github.com if unspecified)
export PKGS=(
    "tpope/vim-fugitive"
    "ibhagwan/fzf-lua"
    "neovim/nvim-lspconfig"
    "hrsh7th/nvim-cmp"
    "hrsh7th/cmp-buffer"
    "hrsh7th/cmp-nvim-lsp"
    "dcampos/cmp-snippy"
    "dcampos/nvim-snippy"
    "nvim-treesitter/nvim-treesitter"
    "kafva/startpage.nvim"
)

# Patch files from PLG_PATCHDIR to apply after cloning/updating
export PATCHES=(
    "vim-fugitive"
)
```
2. Run `plg sync`
