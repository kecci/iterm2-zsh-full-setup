# iTerm2 & Zsh Full Setup

This repository provides a comprehensive setup for iTerm2 and Zsh, pre-configured with essential plugins and themes to enhance your terminal experience. It aims to offer a powerful, efficient, and visually appealing command-line environment for developers.

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

## Configuration

The `.zshrc` file in this repository contains the core configuration for Zsh, including plugin loading, theme settings, and custom aliases/functions.

**To use this configuration:**

1.  **Backup your existing .zshrc:** It's highly recommended to back up your current Zsh configuration before proceeding.
    ```bash
    mv ~/.zshrc ~/.zshrc.bak
    ```
2.  **Copy the provided .zshrc:** Copy the `.zshrc` file from this repository to your home directory.
    ```bash
    cp .zshrc ~/.zshrc
    ```
3.  **Reload your Zsh configuration:**
    ```bash
    source ~/.zshrc
    ```

## Usage

Once the setup is complete and your `.zshrc` is sourced, you can immediately benefit from the following features:

*   **Autosuggestions:** As you type, you'll see command suggestions based on your history and common commands. Press the `right arrow` key to accept a suggestion.
*   **Syntax Highlighting:** Commands will be highlighted with different colors as you type, making it easier to spot errors and improve readability.
*   **Autocompletion:** Press `Tab` for intelligent command and path completion.
*   **Autojump:** Quickly navigate directories by typing `j <part_of_directory_name>`. For example, `j proj` might jump to `~/Documents/Projects`.

## Customization

This setup is designed to be a solid starting point. You can further customize it to fit your workflow:

*   **Themes:** Explore more themes at [https://iterm2colorschemes.com/](https://iterm2colorschemes.com/) or [https://terminalcolors.com/iterm2/](https://terminalcolors.com/iterm2/). You can change your Zsh theme by editing the `ZSH_THEME` variable in your `~/.zshrc` file.
*   **Plugins:** Add or remove Zsh plugins by modifying the `plugins` array in your `~/.zshrc`. Refer to the Oh My Zsh [wiki](https://github.com/ohmyzsh/ohmyzsh/wiki/Plugins) for a list of available plugins.
*   **Aliases & Functions:** Personalize your command-line experience by adding custom aliases and functions to your `~/.zshrc`.

## Troubleshooting

*   **Plugins not loading:** Ensure that `source ~/.zshrc` was run after copying the file. Check if the plugin directories exist under `$ZSH_CUSTOM/plugins`.
*   **Theme issues:** Verify that the `ZSH_THEME` variable in `~/.zshrc` is set to a valid theme. You might need to install additional fonts (like Powerline fonts) for some themes to display correctly.
*   **Autojump not working:** Make sure `autojump` is installed via Homebrew (`brew install autojump`) and that it's enabled in your `.zshrc` plugins.

## Contributing

Contributions are welcome! If you have suggestions for improvements, new plugins, themes, or bug fixes, please feel free to:

1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature/your-feature-name`).
3.  Make your changes.
4.  Commit your changes (`git commit -m 'Add some feature'`).
5.  Push to the branch (`git push origin feature/your-feature-name`).
6.  Open a Pull Request.

## References

- https://gist.github.com/n1snt/454b879b8f0b7995740ae04c5fb5b7df

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

