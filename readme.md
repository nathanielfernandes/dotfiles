## nathan's dotfiles

### bootstrapping

```zsh
# command line tools
xcode-select --install

# clone .dotfiles
git clone https://github.com/nathanielfernandes/dotfiles.git ~/.dotfiles

# create symlinks
ln -s ~/.dotfiles/.zshrc ~/.zshrc
ln -s ~/.dotfiles/.gitconfig ~/.gitconfig
ln -s ~/.dotfiles/.vimrc ~/.vimrc
ln -s ~/.dotfiles/.p10k.zsh ~/.p10k.zsh
ln -s ~/.dotfiles/.gemrc ~/.gemrc

# homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# brew bundle
brew bundle --file ~/.dotfiles/Brewfile
```
