# MyShell Scripts

## Installation

```
cd ~ && git clone git@github.com:matiascaniete/myshell.git
```

## Configuration and Autocompletion in Zsh

To enable autocompletion for the MyShell scripts in zsh, add the following line
to your `~/.zshrc` file:

```sh
fpath=(~/myshell/autocomplete $fpath)

autoload -Uz compinit
compinit
```

## List of Commands

You can find the complete list of commands in the following documentation files:

- [COMMANDS.md](docs/COMMANDS.md)
- [color.md](docs/color.md)
- [confirm.md](docs/confirm.md)
- [gpt.md](docs/gpt.md)
- [mysh.md](docs/mysh.md)
- [rascreen.md](docs/rascreen.md)
