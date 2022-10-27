## Doom Emacs Configuration

### Linux

1. Install [Emacs](https://github.com/doomemacs/doomemacs/blob/master/docs/getting_started.org#on-linux).

```bash
sudo add-apt-repository ppa:kelleyk/emacs
sudo apt update
sudo apt install emacs28-nativecomp
sudo apt install ripgrep fd-find
```

2. Install [Doom Emacs](https://github.com/doomemacs/doomemacs/blob/master/docs/getting_started.org#doom-emacs).

```bash
git clone https://github.com/hlissner/doom-emacs ~/.emacs.d
~/.emacs.d/bin/doom install
```

### macOS

1. Install [Emacs](https://github.com/doomemacs/doomemacs/blob/master/docs/getting_started.org#on-macos).

```bash
brew install git ripgrep
brew install coreutils fd
xcode-select --install
brew tap railwaycat/emacsmacport
brew install --cask emacs-mac
```

2. Install [Doom Emacs](https://github.com/doomemacs/doomemacs/blob/master/docs/getting_started.org#doom-emacs).

```bash
git clone https://github.com/hlissner/doom-emacs ~/.emacs.d
~/.emacs.d/bin/doom install
```

3. Add Doom Emacs to PATH in [.zshrc](https://github.com/gvelasq/dotfiles/blob/main/zsh/.zshrc#L1-L2).
