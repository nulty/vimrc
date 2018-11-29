# vimrc

## Install Vim

```
$ sudo apt-get install vim-athena
$ brew install vim --with-ruby --with-python3 --with-clipboard

```
It's advised to install this version of Vim because it comes with many compiler features
enabled. Scripting language support is required by some of the plugins listed below.

| Plugin    | Dependency |
|-----------|------------|
| Command-T | Ruby       |
| UltiSnip  | Python     |

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
godlygeek/tabular
benmills/vimux
honza/vim-snippets
SirVer/ultisnips
christoomey/vim-tmux-navigator
tpope/vim-endwise
Asheq/close-buffers.vim

)

for package in ${plugins[*]};
do
  git clone git@github.com:$package.git
done
```

## Install Powerline fonts for vim-airline
`$ sudo apt-get install fonts-powerline`

## Install LivedownPreview
`$ npm install livedown`

## Install Ripgrep
```shell
$ curl -LO https://github.com/BurntSushi/ripgrep/releases/download/0.10.0/ripgrep_0.10.0_amd64.deb
$ sudo dpkg -i ripgrep_0.10.0_amd64.deb
```

# Install CommandT
```
# Check what Ruby version vim was built with and make sure its the global/system version on the system

$ cd ~/.vim/bundle/command-t/ruby/command-t/ext/command-t/
$ ruby extconf.rb
$ make
```

