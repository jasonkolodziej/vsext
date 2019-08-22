# vsext
export vscode extensions 
# How to export your VS Code extensions from terminal

_**Note:** [Unix-like systems](https://en.wikipedia.org/wiki/Operating_system#Unix_and_Unix-like_operating_systems) only._

1) Export your extensions to a shell file:

```sh
code --list-extensions | sed -e 's/^/code --install-extension /' > my_vscode_extensions.sh
```

2) Verify your extensions installer file:

```sh
less my_vscode_extesions.sh
```

### Install your extensions (optional)

Run your `my_vscode_extensions.sh` using [Bash](https://www.gnu.org/software/bash/) command:

```sh
bash my_vscode_extensions.sh
```
