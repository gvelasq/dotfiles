## [macOS Configuration](https://ivelasq.rbind.io/blog/macos-rig)

1. Install [Homebrew](https://brew.sh).

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

2. Install [Git](https://git-scm.com/download/mac).

```bash
brew install git
```

3. Configure [global Git settings](https://github.com/gvelasq/git-reference#setup).

```bash
git config --global user.name "<full-name>"
git config --global user.email "<email>"
```

4. Install [zsh](https://zsh.sourceforge.io).

```bash
brew install zsh
```

5. Install [iTerm2](https://iterm2.com).

```bash
brew install --cask iterm2
```

In iTerm2 settings, set `Profiles > Colors > Cursor` to green (`51bf37`) and disable `Profiles > Terminal > Show mark indicators`.

6. Install [oh-my-zsh](https://ohmyz.sh/#install).

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

7. Configure [oh-my-zsh](https://github.com/gvelasq/dotfiles/tree/main/zsh).

8. Install [rig](https://github.com/r-lib/rig?tab=readme-ov-file#installing-rig-on-macos-).

```bash
brew tap r-lib/rig
brew install --cask rig
```

9. Install [R](https://www.r-project.org).

```bash
rig add release
```

10. Install [RStudio Desktop](https://posit.co/download/rstudio-desktop).

```bash
brew install --cask rstudio
```

11. Configure [.Rprofile](https://github.com/gvelasq/dotfiles/blob/main/R/.Rprofile).

```r
usethis::edit_r_profile()
```

12. Configure [RStudio](https://github.com/gvelasq/dotfiles/tree/main/rstudio).

13. Create a [GitHub PAT](https://usethis.r-lib.org/reference/github-token.html).

```r
usethis::create_github_token()
```

14. Set [Git credentials](https://gitcreds.r-lib.org/reference/gitcreds_get.html).

```r
gitcreds::gitcreds_set()
```

15. Install [Quarto](https://quarto.org/docs/get-started).

```bash
brew install --cask quarto
```
