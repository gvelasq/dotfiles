## Linux configuration

These instructions have been tested with [Ubuntu MATE 22.04](https://ubuntu-mate.org/blog/ubuntu-mate-jammy-jellyfish-release-notes).

1. Install [Git](https://git-scm.com/download/linux).

```bash
sudo apt install git
```

2. Configure [global Git settings](https://github.com/gvelasq/git-reference#setup).

```bash
git config --global user.name "<full-name>"
git config --global user.email "<email>"
git config --global core.editor "vi"
```

3. Install [zsh](https://zsh.sourceforge.io).

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

8. Install [rig](https://github.com/r-lib/rig#linux).

9. Install [R](https://www.r-project.org).

```bash
rig add release
```

10. Install [RStudio Desktop]([https://posit.co/download/rstudio-desktop).

11. Configure [.Rprofile](https://github.com/gvelasq/dotfiles/blob/main/R/.Rprofile).

```r
usethis::edit_r_profile()
```

12. Configure [RStudio](https://github.com/gvelasq/dotfiles/tree/main/rstudio).

13. Set Git credentials in R.

```r
gitcreds::gitcreds_set()
```

14. Install [Quarto](https://quarto.org/docs/get-started).

15. Install [kinto](https://github.com/rbreaves/kinto) for macOS-style keyboard shortcuts.

```bash
/bin/bash -c "$(wget -qO- https://raw.githubusercontent.com/rbreaves/kinto/HEAD/install/linux.sh || curl -fsSL https://raw.githubusercontent.com/rbreaves/kinto/HEAD/install/linux.sh)"
```

16. Install [Compiz](https://launchpad.net/compiz) and the Compiz configuration settings manager.

```bash
sudo apt install compiz
sudo apt install compizconfig-settings-manager
sudo apt install compiz-plugins-extra
```

17. Configure Compiz.
