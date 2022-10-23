## macOS Configuration

1. Install [Homebrew](https://brew.sh/).

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Install [Git](https://git-scm.com/download/linux).

```bash
brew install git
```

3. Install [zsh](https://zsh.sourceforge.io/).

```bash
brew install zsh
```

4. Install [oh-my-zsh](https://ohmyz.sh/#install).

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

5. Configure [oh-my-zsh](https://github.com/gvelasq/dotfiles/tree/main/zsh).

6. Install [rig](https://github.com/r-lib/rig#linux).

```bash
curl -Ls https://github.com/gaborcsardi/rim/releases/download/v0.3.0/rim-linux-0.3.0.tar.gz |
  sudo tar xz -C /usr/local
```

7. Install [R](https://www.r-project.org/).

```bash
rig add release
```

8. Install [RStudio Desktop Preview](https://www.rstudio.com/products/rstudio/download/preview/).

```bash
brew tap homebrew/cask-versions
brew install --cask rstudio-preview
```

9. Install [Quarto](https://quarto.org/docs/get-started/).

```bash
brew install --cask quarto
```
