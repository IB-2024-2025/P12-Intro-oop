# Práctica 11. Introducción a la Programación Orientada a Objetos. Depuración.

# Factor de ponderación: 10

### Objetivos
Los objetivos de esta práctica son que el alumnado:
* Sea capaz de resolver problemas sencillos en C++ usando todos los conocimientos adquiridos hasta ahora,
  y en particular utilizando funciones y ficheros de texto
* Diseñe, desarrolle y utilice funciones en sus programas haciendo que sus programas sean modulares
* Configure y practique el uso de Visual Studio Code (VSC) para editar ficheros de forma remota en su VM

### Rúbrica de evaluacion de esta práctica
Se señalan a continuación los aspectos más relevantes (la lista no es exhaustiva) que se tendrán en cuenta a la hora de evaluar esta práctica.
Se comprobará que el alumnado:
* Conoce los conceptos expuestos en el material de referencia de esta práctica.
* Ha realizado todos los ejercicios propuestos en este enunciado
* Es capaz de escribir programas simples en C++ que resuelvan problemas de complejidad similar a los que se proponen en este documento
* Sea capaz de utilizar VSC para editar y compilar programas de forma remota en su Máquina Virtual
* Conoce la plataforma Exercism y es capaz de descargar y realizar problemas sencillos interaccionando con ella.
* Es capaz de escribir un fichero `CMakeLists.txt` para automatizar el proceso de compilación de sus programas con `cmake` y `make`
* Ha automatizado la compilación de sus programas usando un fichero `Makefile` para cada uno de los programas que desarrolle
* Hace que sus programas se estructuren en torno a diferentes funciones (sean modulares)
* Todos sus programas se estructuran en directorios diferentes para cada "proyecto" haciendo que cada uno de
  ellos contenga un fichero `CMakeLists.txt` con la configuración de despliegue del proyecto.
* Utiliza en todos sus programas comentarios adecuados en el formato requerido por
[Doxygen](https://www.doxygen.nl/index.html)
* Acredita que todas las prácticas realizadas hasta la fecha se encuentran alojadas en repositorios privados de
[GitHub](https://github.com/).
* Acredita que es capaz de subir programas a la plataforma
[Jutge](https://jutge.org/)
para su evaluación
* Ha incluido un comentario prólogo en todos los ficheros (`*.cc`, `*.h`) de sus ejercicios
* Que todos los programas que desarrolla, antes de su ejecución imprimen en pantalla un mensaje indicando la
  finalidad del programa así como la información que precisará del usuario para su correcta ejecución.
* Hace que todos los programas que se presentan para su evaluación cumplan con los estándares definidos en la
[Guía de estilo de Google para C++](https://google.github.io/styleguide/cppguide.html)
* Utiliza siempre identificadores significativos en su programa (para constantes, variables, etc.) y
  no utiliza nunca identificadores de una única letra, tal vez con la excepción de las variables que utilice para iterar en un bucle.
* Acredita que es capaz de editar ficheros remotos en su VM usando vi
* Ha realizado todos sus ejercicios en la máquina virtual Ubuntu de la asignatura.
* Demuestra que es capaz de ejecutar comandos Linux en su VM

#### Visual Studio Code

### Material de estudio complementario
Además de los contenidos revisados en las
[Transparencias de clase](https://docs.google.com/presentation/d/1k2IyoAsmd60a6EzP96eLuhgISdf9e35nPRPIBb92a3E/edit?usp=sharing)
correspondientes al tema de Entrada/Salida así como los
[Ejemplos de código](https://github.com/IB-2022-2023/IB-class-code-examples/tree/master/Functions)
correspondientes a ese material,
estudie del
[tutorial de referencia](https://www.learncpp.com/)
en la asignatura los siguientes apartados:
* [23.1 Input and output (I/O) streams](https://www.learncpp.com/cpp-tutorial/input-and-output-io-streams/)
* [23.2 Input with istream](https://www.learncpp.com/cpp-tutorial/input-with-istream/)
* [23.3 Output with ostream and ios](https://www.learncpp.com/cpp-tutorial/output-with-ostream-and-ios/)
* [23.6 Basic file I/O](https://www.learncpp.com/cpp-tutorial/basic-file-io/)

### Ejercicios
* Al realizar los ejercicios cree dentro de su repositorio de esta práctica un directorio diferente
para cada uno de los ejercicios.
Asigne a cada uno de esos directorios nombres significativos.
* Automatice la compilación del programa correspondiente a cada ejercicio con un fichero `Makefile`
independiente para cada programa e inclúyalo en el correspondiente directorio. 
Alternativamente podría también usarse `cmake` con un fichero `CMakeLists`, si se prefiere.
* Haga que todos los programas tomen su entrada por la línea de comandos y en caso de que se ejecuten sin
  pasarles el número adecuado de parámetros impriman en pantalla un mensaje indicando el modo correcto de
  ejecutar el programa.
* El código de cada uno de los programas deberá organizarse de forma modular, es decir haciendo uso de funciones
* Cada función deberá realizar una única tarea y hacerlo correctamente
* El identificador de una función debe reflejar claramente la finalidad de la función

1. 
