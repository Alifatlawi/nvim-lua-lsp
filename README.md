# nvim-lua-lsp
Neovim .config

To set up nvim-lua-lsp in Neovim, you need to add the files to your Appdata/Local/nvim directory.
If this directory doesn't exist, create a new one.

# problem

If you encounter an issue where libraries cannot be read, such as a missing iostream file, you can use clangd to fix the problem. To do this, create a new file called .clangd in your user folder and add the following code after everything:

CompileFlags:
  Add: ["--target=x86_64-w64-mingw64"]

This should resolve the issue and allow you to use nvim-lua-lsp without any problems.
