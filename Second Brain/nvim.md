
# neovim
I use neovim, here are my [[nvim-keybindings]]

Setup [[nvim]] from [[from-scratch]]
remaps

vim.g.mapleader = "  "
vim.keymap.set("n", "<leader>pv",  vim.cmd.Ex)
the .set params are (MODE, COMMAND, EXECUTABLE COMMAND)

packer manager
packer.nvim
when installing with packer, use :PackerSync to add packages

telescope requires ripgrep to use grep within the fuzzy finder `brew install ripgrep`


create my packer
install the plugin i want
go to after
add the file to config plugin

undo tree
vim.keymap.set("n", "<leader>u", vim.cmd.UndotreeToggle)

git integration with tpope/fugitive
git status
vim.keymap.set("n", "<leader>gs", vim.cmd.Git)


LSP
VIEW DIAGNOSTICS
<leader>vd = view diagnostics (view errors in popup)

cop and paste curr paragraph
"v" to enter visual mode, then "ap", then "y" for vim cp or "<leader>y" for system clip

delete line -> "D"




download neovim
mkdir .config/nvim && cd .config/nvim
touch init.lua then type print("hello")
source file :so
return to nvim folder
mkdir lua/skngstn
cd lua/skngstn
inside vim % creates file make another init.lua
inside there print("hello from skngstn")
source file
get package manager called packer by wbthomason