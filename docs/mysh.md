# myshell manager

A command line tool for managing the myshell script.

## Usage

```
mysh <sub-command> [options] [arguments]
```

## Sub-commands

### `update`

Update the myshell script to the latest version.

Options:
- None

Examples:
```
mysh update
```

### `description`

Get the description of a command.

Options:
- `--printer|-p <printer>`: Specify the printer to use (`dp_plain` or `dp_markdown`) (Default: `dp_plain`)

Arguments:
- `<command>`: The command to get the description of.

Examples:
```
mysh description update
```
```
mysh description update --printer dp_markdown
```

### `list`

List all the available commands.

Options:
- None

Examples:
```
mysh list
```

### `md`

Generate the Markdown documentation of the available commands.

Options:
- None

Examples:
```
mysh md
```

### `md2doc`

Generate the Markdown documentation of the available commands and save it to `../docs/COMMANDS.md`.

Options:
- None

Examples:
```
mysh md2doc
```

### `commands`

Display the Markdown documentation of the available commands.

Options:
- None

Examples:
```
mysh commands
```

### `help`

Display the README documentation of the myshell script.

Options:
- None

Examples:
```
mysh help
```

### `create`

Create a new command file.

Options:
- None

Arguments:
- `<filename>`: The name of the file to create.

Examples:
```
mysh create mycommand.sh
```
