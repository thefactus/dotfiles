# My Dotfiles

Just [Chris Oliver's](https://twitter.com/excid3) dotfiles. You can copy these in and everything is ready for the races.

## Installation

1. Clone this repo

    ```
    mkdir -p ~/code && cd ~/code && git clone https://github.com/excid3/dotfiles.git
    ```

2. Install Homebrew

    ```
    /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
    ```

3. Install MacVim, rbenv, ruby-build, and more

    ```
    brew install macvim rbenv ruby-build postgresql elasticsearch redis zsh
    brew install Caskroom/cask/iterm2
    brew install Caskroom/cask/google-chrome
    ```

4. Install Oh-My-ZSH

    ```
    sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
    ```

5. Install Janus for Vim

    ```
    curl -L https://bit.ly/janus-bootstrap | bash
    ```

6. Symlink configs

    ```
    ln -s ~/code/dotfiles/zsh/themes/excid3.zsh-theme ~/.oh-my-zsh/themes/excid3.zsh-theme
    ln -s ~/code/dotfiles/zsh/zshrc ~/.zshrc
    ln -s ~/code/dotfiles/vim/gvimrc.after ~/.gvimrc.after
    ln -s ~/code/dotfiles/psqlrc ~/.psqlrc
   ```

7. Open iTerm and import color scheme from iterm folder

# Other tips

Here are some other useful commands I like to use:

#### Pretty ```git lg```

	git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --"
