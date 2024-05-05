# Trabajo práctico 1 - Threading

## Estructura
* En la carpeta `src` se encuentra el código.
* En la carpeta `data` hay algunos archivos que usamos para probar la solución.
* En la carpeta `scripts` se encuentran algunos scripts para testear la solución.
  
## Compilación
* El `Makefile` debería permite compilar el código con el comando `make`.
  El ejecutable generado va a estar en la carpeta `build`.
* El ejecutable se puede correr de la siguiente forma:
  ```
  ./ContarPalabras <threads_lectura> <threads_maximo> <archivo1> [<archivo2>...]
  ```
  donde:
  * `threads_lectura` es la cantidad de threads que se usará para leer archivos,
  * `threads_maximo` es la cantidad de threads que se usará para computar
    la palabra con más apariciones, y
  * `archivo1`, `archivo2`, etc. son los nombres de los archivos a procesar.

## Tests
* Ejecutando `make test` se pueden compilar y ejecutar una pequeña suite de tests
  unitarios.
