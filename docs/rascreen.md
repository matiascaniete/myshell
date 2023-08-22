# rascreen

El comando `rascreen` se utiliza para enviar mensajes o comandos a una pantalla LCD conectada a una Raspberry Pi a través de un socket TCP. Puede enviar una cadena de texto o un comando como argumento, o leer el mensaje desde la entrada estándar.

## Uso

```
rascreen [listen|info|send]
```

## Subcomandos

### send

El subcomando `send` se utiliza para enviar mensajes o comandos a la pantalla LCD. Puede recibir una cadena de texto o un comando como argumento, o leer el mensaje desde la entrada estándar.

#### Opciones

- Ninguna

#### Argumentos

- `message`: El mensaje o comando a enviar a la pantalla LCD.

### listen

El subcomando `listen` se utiliza para escuchar mensajes entrantes en el puerto especificado y mostrarlos en la pantalla LCD.

#### Opciones

- Ninguna

#### Argumentos

- Ninguna

### info

El subcomando `info` se utiliza para mostrar la configuración actual de `rascreen`.

#### Opciones

- Ninguna

#### Argumentos

- Ninguna

## Variables de entorno

- `RASCREEN_HOST`: La dirección IP o el nombre de host de la Raspberry Pi. Por defecto: `raspberrypi.local`.
- `RASCREEN_PORT`: El puerto en el que se establece la conexión TCP. Por defecto: `8000`.
- `RASCREEN_TTY`: El dispositivo TTY en el que se muestra la salida de la pantalla LCD. Por defecto: `/dev/tty1`.

## Ejemplos de uso

1. Enviar un mensaje a la pantalla LCD:

```
rascreen send "Hello, world!"
```

2. Enviar la salida de un comando a la pantalla LCD:

```
rascreen send date
```

3. Escuchar mensajes entrantes en el puerto 8000:

```
rascreen listen
```

4. Mostrar la configuración actual de `rascreen`:

```
rascreen info
```
