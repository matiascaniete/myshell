# OpenAI GPT Chat

Script que utiliza la API de OpenAI para chatear con el modelo GPT-3.5 Turbo.

## Uso

```bash
gpt [opciones] <mensaje>

or

echo <mensaje> | gpt [opciones]
```

## Opciones

- `-h` `--help`: Muestra información de ayuda.
- `-r <rol>` `--role <rol>`: Especifica el rol del mensaje.
- `--list-roles`: Lista los roles disponibles.
- `--create-role <rol>`: Crea un nuevo rol con el nombre especificado.
- `--show-role <rol>`: Muestra el contenido de un rol.
- `--list-models`: Lista los modelos disponibles.
- `-f` `--full-response`: Muestra la respuesta completa de la API.
- `-d` `--debug`: Modo de depuración.
- `-m <modelo>` `--model <modelo>`: Especifica el modelo a utilizar.
- `-t <temperatura>` `--temperature <temperatura>`: Especifica la temperatura.

## Ejemplos

### Ejemplo 1

```bash
gpt "¡Hola! ¿Cómo estás?"
```

Envía un mensaje al modelo GPT-3.5 Turbo.

### Ejemplo 2

```bash
echo "Eres un gato muy guapo" | gpt --create-role gato
```

Crea un nuevo rol llamado "bot".

### Ejemplo 3

```bash
gpt -r gato "¿Cual es tu comida favorita?"
```

Envía un mensaje con el rol "gato" al modelo GPT-3.5 Turbo.

### Ejemplo 4

```bash
gpt --show-role gato
```

Muestra el contenido del rol "gato".

### Ejemplo 5

```bash
gpt --list-roles
```

Lista los roles disponibles.

### Ejemplo 6

```bash
gpt --list-models
```

Lista los modelos disponibles.

### Ejemplo 7

```bash
gpt -f "¡Hola! ¿Cómo estás?"
```

Envía un mensaje al modelo GPT-3.5 Turbo y muestra la respuesta completa de la API.

### Ejemplo 8

```bash
gpt -d "¡Hola! ¿Cómo estás?"
```

Modo de depuración. Muestra el comando curl que se ejecutaría en lugar de realizar la llamada real a la API.
