# Comando `color`

El comando `color` se utiliza para colorear texto en la salida estándar. Puede recibir el texto como argumento o desde la entrada estándar.

## Uso

```
color color_name text
```

```
some_command | color color_name
```

## Colores disponibles

- red: Rojo
- green: Verde
- yellow: Amarillo
- blue: Azul
- magenta: Magenta
- cyan: Cian
- gray: Gris

## Opciones

- `color_name`: El nombre del color a utilizar.

## Ejemplos

Colorear texto rojo:

```
color red "Hello, world!"
```

Colorear texto verde:

```
color green "Hello, world!"
```

Colorear texto amarillo:

```
color yellow "Hello, world!"
```

Colorear texto azul:

```
color blue "Hello, world!"
```

Colorear texto magenta:

```
color magenta "Hello, world!"
```

Colorear texto cian:

```
color cyan "Hello, world!"
```

Colorear texto gris:

```
color gray "Hello, world!"
```

Colorear el texto de la salida estándar de un comando:

```
some_command | color red
```
