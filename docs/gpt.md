# OpenAI GPT Chat

This script uses the OpenAI API to chat with the GPT-3.5 Turbo model.

## Usage

```bash
gpt [options] <message>

or

echo <message> | gpt [options]
```

## Options

- `-h`, `--help`: Show help information.
- `-r <role>`, `--role <role>`: Specify the role of the message.
- `--list-roles`: List the available roles.
- `--create-role <role>`: Create a new role with the specified name.
- `--show-role <role>`: Show the content of a role.
- `--list-models`: List the available models.
- `-f`, `--full-response`: Show the full response from the API.
- `-d`, `--debug`: Debug mode.
- `-m <model>`, `--model <model>`: Specify the model to use.
- `-t <temperature>`, `--temperature <temperature>`: Specify the temperature.

## Examples

### Example 1

```bash
gpt "Hello! How are you?"
```

Send a message to the GPT-3.5 Turbo model.

### Example 2

```bash
echo "You are a very handsome cat" | gpt --create-role cat
```

Create a new role called "cat".

### Example 3

```bash
gpt -r cat "What is your favorite food?"
```

Send a message with the "cat" role to the GPT-3.5 Turbo model.

### Example 4

```bash
gpt --show-role cat
```

Show the content of the "cat" role.

### Example 5

```bash
gpt --list-roles
```

List the available roles.

### Example 6

```bash
gpt --list-models
```

List the available models.

### Example 7

```bash
gpt -f "Hello! How are you?"
```

Send a message to the GPT-3.5 Turbo model and show the full API response.

### Example 8

```bash
gpt -d "Hello! How are you?"
```

Debug mode. Show the curl command that would be executed instead of making the actual API call.
