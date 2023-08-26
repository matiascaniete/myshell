## OpenAI GPT Chat

This script allows you to interact with the GPT-3.5 Turbo model using the OpenAI API for chat conversations.

### Usage

```shell
gpt [options] <message>

or

echo <message> | gpt [options]
```

### Options

- `-h`, `--help`: Show the help information.
- `-r <role>`, `--role <role>`: Specify the role of the message.
- `--list-roles`: List all available roles.
- `--create-role <role>`: Create a new role with the specified name.
- `--show-role <role>`: View the content of a role.
- `--list-models`: List all available models.
- `-f`, `--full-response`: Show the full response from the API.
- `-d`, `--debug`: Enable debug mode. Instead of making the actual API call, it shows the corresponding curl command.
- `-m <model>`, `--model <model>`: Specify the model to use.
- `-t <temperature>`, `--temperature <temperature>`: Specify the temperature.
- `--file <file_path>`: Specify a file to be modified.

### Examples

1. Send a message to the GPT-3.5 Turbo model:

```shell
gpt "Hello! How are you?"
```

2. Create a new role named "cat" and send a message:

```shell
echo "You are a very handsome cat" | gpt --create-role cat
```

3. Send a message with the "cat" role to the GPT-3.5 Turbo model:

```shell
gpt -r cat "What is your favorite food?"
```

4. View the content of the "cat" role:

```shell
gpt --show-role cat
```

5. List all available roles:

```shell
gpt --list-roles
```

6. List all available models:

```shell
gpt --list-models
```

7. Send a message to the GPT-3.5 Turbo model and show the full API response:

```shell
gpt -f "Hello! How are you?"
```

8. Enable debug mode. Instead of making the actual API call, it shows the curl command:

```shell
gpt -d "Hello! How are you?"
```

9. Specify a file to be modified using the `--file` option and show the output:

```shell
gpt --file <file_path> --role=cat "Some additional instructions."
```
