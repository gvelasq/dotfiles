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

10. Install [RStudio Desktop](https://posit.co/download/rstudio-desktop).

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

16. Install [kinto](https://github.com/rbreaves/kinto) for macOS-style keyboard shortcuts.

```bash
/bin/bash -c "$(wget -qO- https://raw.githubusercontent.com/rbreaves/kinto/HEAD/install/linux.sh || curl -fsSL https://raw.githubusercontent.com/rbreaves/kinto/HEAD/install/linux.sh)"
```

17. Install [Compiz](https://launchpad.net/compiz) and the Compiz configuration settings manager.

```bash
sudo apt install compiz
sudo apt install compizconfig-settings-manager
sudo apt install compiz-plugins-extra
```

18. Configure Compiz.

`CompizConfig Settings Manager > Scale > Bindings > Initiate Window Picker` should be set to  `<Super>w`, to allow Touchégg to use the `<Super>w` keyboard shortcut with the three-finger swipe gesture below.

```bash
[scale]
# ...
s0_initiate_key = <Super>w
# ...
s0_click_on_desktop = 2
```

19. Install [Touchégg](https://github.com/JoseExposito/touchegg?tab=readme-ov-file#ubuntu-debian-and-derivatives).

```bash
sudo add-apt-repository ppa:touchegg/stable
sudo apt update
sudo apt install touchegg
```

20. Configure Touchégg at `~/.config/touchegg/touchegg.conf`.

```xml
<touchégg>
  <settings>
    <property name="animation_delay">150</property>
    <property name="action_execute_threshold">20</property>
    <property name="color">auto</property>
    <property name="borderColor">auto</property>
  </settings>
  <application name="All">
    <gesture type="SWIPE" fingers="3" direction="UP">
      <action type="SEND_KEYS">
        <modifiers>Super_L</modifiers>
        <keys>w</keys>
        <repeat>false</repeat>
        <animation>NONE</animation>
        <on>begin</on>
      </action>
    </gesture>
    <gesture type="SWIPE" fingers="3" direction="DOWN">
      <action type="SEND_KEYS">
        <modifiers>Super_L</modifiers>
        <keys>w</keys>
        <repeat>false</repeat>
        <animation>NONE</animation>
        <on>begin</on>
      </action>
    </gesture>
  </application>
</touchégg>
```
