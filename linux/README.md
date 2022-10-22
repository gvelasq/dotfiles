## Linux configuration

1. Install [Git](https://git-scm.com/download/linux).

```bash
sudo apt install git
```

2. Configure [global Git settings](https://github.com/gvelasq/git-reference#setup).

```bash
git config --global user.name "<full-name>"
git config --global user.email "<email>"
```

3. Install [zsh](https://zsh.sourceforge.io/).

```bash
sudo apt install zsh
```

4. Install [oh-my-zsh](https://ohmyz.sh/#install).

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

5. Configure [oh-my-zsh](https://github.com/gvelasq/dotfiles/tree/main/zsh).

6. Install [GCM](https://github.com/GitCredentialManager/git-credential-manager#linux).

7. Configure GCM and the [credential store](https://github.com/GitCredentialManager/git-credential-manager/blob/main/docs/credstores.md#gits-built-in-credential-cache).

```bash
git-credential-manager-core configure
git config --global credential.credentialStore cache
```

8. Install [rig](https://github.com/r-lib/rig#macos-homebrew).

```bash
brew tap r-lib/rig
brew install --cask rig
```

9. Install [R](https://www.r-project.org/).

```bash
rig add release
```

10. Install [RStudio Desktop Preview](https://www.rstudio.com/products/rstudio/download/preview/).

11. Configure [.Rprofile](https://github.com/gvelasq/dotfiles/blob/main/R/.Rprofile).

12. Configure [RStudio](https://github.com/gvelasq/dotfiles/tree/main/rstudio).

13. Set Git credentials in R.

```r
gitcreds::gitcreds_set()
```

14. Install [Quarto](https://quarto.org/docs/get-started/).

15. Install [kinto](https://github.com/rbreaves/kinto) for macOS-style keyboard shortcuts.

```bash
/bin/bash -c "$(wget -qO- https://raw.githubusercontent.com/rbreaves/kinto/HEAD/install/linux.sh || curl -fsSL https://raw.githubusercontent.com/rbreaves/kinto/HEAD/install/linux.sh)"
```