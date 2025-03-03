# El editor vi

Es el editor "básico" de Linux en terminales. Realmente se trata de un editor muy potente, pero extremadamente complejo de manejar. Esta guía pretende ofrecer algunas operaciones básicas para trabajar con el editor.

## Iniciar el editor

Para iniciar el editor desde un terminal, se invoca al programa indicando el fichero que se desea editar:

```sh
vi /tmp/fichero.txt
```

## Dentro del editor

Por defecto `vi` se inicia en el modo de comandos/acciones.

### Modo de comandos

Aquí no se edita el texto como tal. Algunos comandos comunes son:

- Pulsar `i` para entrar en el modo de inserción.
- Pulsar `d`,`d` para borrar la línea actual.
- Escribir `:wq` para guardar y salir (`w` de _write_, escritura, y `q` de _quit_, salir).
- Escribir `:q!` para salir sin guardar (la exclamación forzará la operación).

La lista completa de comandos se puede ver en la imagen siguiente:

![vi_keyboard](../img/vi_keyboard.png)

### Modo de inserción

En este modo se trabajaría con `vi` de una forma muy similar a cualquier otro editor de texto. Se indicará que está en este modo porque en la parte inferior aparecerá un texto como `--INSERT--`.

Para volver al modo de comandos, pulsar `Esc`.

### Modo de remplazo

Este modo es semejante al modo de inserción pero con la característica particular de que sustituirá el caracter sobre el que estará el cursor por el nuevo. Se identifica con el texto inferior de `--REPLACE--` y se entra con el comando `R`.

Para volver al modo de comandos, pulsar `Esc`