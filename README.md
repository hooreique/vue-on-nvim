```bash
# See https://vuejs.org/guide/quick-start.html#creating-a-vue-application
nix develop --command pnpm create vue@3.16.4 .
```

```lua
-- Using github:neovim/nvim-lspconfig
if vim.fn.executable 'vue-language-server' == 1 then
  vim.lsp.config('vue_ls', {
    init_options = { vue = { hybridMode = false } },
    filetypes = {
      'javascript',
      'javascriptreact',
      'typescript',
      'typescriptreact',
      'vue',
    },
  })
  vim.lsp.enable 'vue_ls'
end
```
