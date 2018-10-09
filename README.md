# vimrc

## Description

Listing configuration for my plugins and regular vim config

Install plugins

```shell

cd ~/.vim/bundle

plugins=(
mileszs/ack.vim
bkad/CamelCaseMotion
mattn/emmet-vim
scrooloose/nerdtree
scrooloose/nerdcommenter
flazz/vim-colorschemes
elixir-editors/vim-elixir
airblade/vim-gitgutter
shime/vim-livedown
tpope/vim-rails
dkarter/bullets.vim
wincent/command-t
roman/golden-ratio
othree/javascript-libraries-syntax.vim
vim-airline/vim-airline
rhysd/vim-crystal
tpope/vim-fugitive
vim-syntastic/syntastic
sheerun/vim-polyglot
tpope/vim-surround
)

for package in plugins[*];
do
  git clone git@github.com:$package.git
done
```


