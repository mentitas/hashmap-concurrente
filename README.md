# Trabajo práctico 1 - Threading

Hemos realizado la implementación de una estructura de datos llamada HashMapConcurrente. Esta estructura es una tabla de hash abierta que utiliza listas enlazadas para gestionar las colisiones. Su interfaz de uso es similar a la de un mapa o diccionario, donde las claves son strings y los valores son enteros no negativos. El propósito principal de esta estructura es procesar archivos de texto y contar la cantidad de apariciones de palabras. En este caso, las palabras se utilizan como claves y el número de veces que aparecen se almacena como valor correspondiente.
En este trabajo práctico, hemos explorado la gestión de la concurrencia en los sistemas operativos, centrándonos en la ejecución concurrente de programas y las técnicas para evitar condiciones de carrera y gestionar la contención de recursos. Para ello, hemos utilizado threads, una herramienta proporcionada por los sistemas operativos que nos permite tener múltiples hilos de ejecución concurrentes dentro de un mismo programa, utilizando la interfaz pthreads del estándar POSIX. También hemos utilizado técnicas como bloqueo de secciones críticas, sincronización de hilos y control de acceso a recursos compartidos para evitar condiciones de carrera y garantizar la consistencia de los resultados.

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
