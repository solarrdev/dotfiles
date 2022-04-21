# Linux dotfiles

![dotfiles_preview](https://github.com/solarrdev/dotfiles/blob/master/screenshot_01.png)

Welcome to my Linux dotfiles repository. The terminal in the screenshot above is from WSL but the colorscheme [gruvbox](https://github.com/YV31/gruvbox-css) and the font [Hack](https://github.com/source-foundry/Hack) can be applied in putty, xterm, etc.

## Overview

The triumvirate that enables a powerful terminal workflow consists of zsh, tmux and vim. From left to right the tmux bar indicates name of session, user, window/plane indices, windows, time, date, and hostname. The [Powerline](https://github.com/jimeh/tmux-themepack) themepack repo needs to be pulled and configured in the .tmux.conf file as indicated.

![tmux bar](https://github.com/solarrdev/dotfiles/blob/master/tmux_bar.png)

The same Powerline bar format is applied in the vimrc file, which will be configured during the vimrc setup described in the installation section.

![vim_bar](https://github.com/solarrdev/dotfiles/blob/master/vim_bar.png)

## Installation

This assumes that zsh, tmux, vim and git are installed on system.


*Set zsh as shell*
```
chsh -s $(which zsh)
```

*Clone oh-my-zsh plugins, tmux custom vimrc repositories*
```
git clone https://github.com/solarrdev/dotfiles
git clone http://github.com/robbyrussell/oh-my-zsh ~/.oh-my-zsh
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting
git clone https://github.com/zdharma/history-search-multi-word.git ~/.oh-my-zsh/custom/plugins/history-search-multi-word
git clone https://github.com/zsh-users/zsh-history-substring-search.git ~/.oh-my-zsh/custom/plugins/zsh-history-substring-search 
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
git clone https://github.com/CaffeineViking/vimrc.git ~/.vim_temp
sh ~/.vim_temp/setup.sh
```
