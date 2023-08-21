# Comando `confirm`

Este comando solicita una confirmación al usuario y retorna `0` si la respuesta es afirmativa ("sí"), y `1` en caso contrario ("no").

## Sintaxis

```
confirm MENSAJE [OPCIÓN_POR_DEFECTO]
```

- `MENSAJE`: El mensaje que se mostrará al usuario para solicitar la confirmación.
- `OPCIÓN_POR_DEFECTO`: (Opcional) La opción por defecto, puede ser `y` o `n`. Por defecto, la opción por defecto es `n`.

## Opciones

El comando `confirm` no tiene opciones adicionales.

## Ejemplos de uso

1. Solicitar confirmación con opción por defecto "n":

   ```
   $ confirm "¿Está seguro de continuar?"
   ¿Está seguro de continuar? [Y/n] n
   ```
   En este caso, al presionar Enter, se retornará `1`.

2. Solicitar confirmación con opción por defecto "y":

   ```
   $ confirm "¿Está seguro de continuar?" y
   ¿Está seguro de continuar? [y/N] y
   ```
   En este caso, al presionar Enter, se retornará `0`.

3. Solicitar confirmación sin opción por defecto:

   ```
   $ confirm "¿Está seguro de continuar?"
   ¿Está seguro de continuar? [Y/n] y
   ```
   En este caso, al presionar Enter, se retornará `0`.
