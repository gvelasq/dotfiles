## RStudio configuration

#### 1. `r.snippets`

Append the contents of [r.snippets](https://github.com/gvelasq/dotfiles/blob/main/rstudio/r.snippets) to the local version found here:

```bash
~/.config/rstudio/snippets/r.snippets
```

NOTE:

- Change the prefix of your snippets to your initials. Default is `gv`.

#### 2. `rstudio-prefs.json`

Add the contents of [rstudio-prefs.json](https://github.com/gvelasq/dotfiles/blob/main/rstudio/rstudio-prefs.json) to the local version found here:

```bash
~/.config/rstudio/rstudio-prefs.json
```

NOTE:

- Change `default_project_location` to your preferred directory. Default is `~/code`.
- Change `git_exe_path` to the location of your Git executable, which can be found by typing `which git` in a terminal. Default is `/usr/local/bin/git`.
- Change `document_author` to your name. Default is `gvelasq`.

#### 3. `rstudio_bindings.json`

Add the contents of [rstudio_bindings.json](https://github.com/gvelasq/dotfiles/blob/main/rstudio/rstudio_bindings.json) to the local version found here:

```bash
~/.config/rstudio/keybindings/rstudio_bindings.json
```
