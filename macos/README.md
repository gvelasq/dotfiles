## macOS Configuration

1. Install [Homebrew](https://brew.sh/).

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Install [Git](https://git-scm.com/download/linux).

```bash
brew install git
```

3. Configure [global Git settings](https://github.com/gvelasq/git-reference#setup).

```bash
git config --global user.name "<full-name>"
git config --global user.email "<email>"
```

4. Install [zsh](https://zsh.sourceforge.io/).

```bash
brew install zsh
```

5. Install [oh-my-zsh](https://ohmyz.sh/#install).

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

6. Configure [oh-my-zsh](https://github.com/gvelasq/dotfiles/tree/main/zsh).

7. Install [rig](https://github.com/r-lib/rig#linux).

```bash
curl -Ls https://github.com/gaborcsardi/rim/releases/download/v0.3.0/rim-linux-0.3.0.tar.gz |
  sudo tar xz -C /usr/local
```

8. Install [R](https://www.r-project.org/).

```bash
rig add release
```

9. Install [RStudio Desktop Preview](https://www.rstudio.com/products/rstudio/download/preview/).

```bash
brew tap homebrew/cask-versions
brew install --cask rstudio-preview
```

10. Configure [.Rprofile](https://github.com/gvelasq/dotfiles/blob/main/R/.Rprofile).

11. Configure [RStudio](https://github.com/gvelasq/dotfiles/tree/main/rstudio).

12. Set Git credentials in R.

```r
gitcreds::gitcreds_set()
```

13. Install [Quarto](https://quarto.org/docs/get-started/).

```bash
brew install --cask quarto
```
