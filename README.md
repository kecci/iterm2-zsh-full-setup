# iterm2-zsh-full-setup

## Install iTerm2

- Download: [https://iterm2.com/downloads.html](https://iterm2.com/downloads.html)

## Install Oh-My-ZSH

- Oh-My-Zsh
  `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

## Install Plugins ZSH

* autosuggesions plugin
  `git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions`
* zsh-syntax-highlighting plugin
  `git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting`
* zsh-fast-syntax-highlighting plugin
  `git clone https://github.com/zdharma-continuum/fast-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting`
* zsh-autocomplete plugin
  `git clone --depth 1 -- https://github.com/marlonrichert/zsh-autocomplete.git $ZSH_CUSTOM/plugins/zsh-autocomplete`
* zplug
  `curl -sL --proto-redir -all,https https://raw.githubusercontent.com/zplug/installer/master/installer.zsh | zsh`
* autojump
  `brew install autojump`

## Sample .zshrc

- Open `/.zshrc`

## Themes

- terminalcolors: [https://terminalcolors.com/iterm2/](https://terminalcolors.com/iterm2/)
- iterm2colorschemes: [https://iterm2colorschemes.com/](https://iterm2colorschemes.com/)

## References

- https://gist.github.com/n1snt/454b879b8f0b7995740ae04c5fb5b7df
