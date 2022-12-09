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

1. Desarrolle una clase `Point2D` para representar puntos en el espacio bidimensional a través de sus
coordenadas. 
Incluya al menos los siguientes métodos:
* *Show()* para mostrar en pantalla las coordenadas del punto
* *Move* para cambiar las coordenadas del punto
* *Distance* para calcular la 
[distancia](https://www.mathwarehouse.com/algebra/distance_formula/index.php)
entre dos puntos
* *Middle* para calcular el 
[punto medio](https://en.wikipedia.org/wiki/Midpoint)
del segmento que une dos puntos

2. Diseñe una clase `Circulo` que permita representar círculos utilizando como atributos el centro,
el radio y el color del círculo.
Utilice una
[enumeración](https://www.learncpp.com/cpp-tutorial/unscoped-enumerations/)
(`enum`) para representar el color del círculo.
Incluya métodos *Area*, *Perimetro* y *Print* que permitan respectivamente calcular el área, el perímetro del
círculo así como imprimir en pantalla la información relativa al círculo en cuestión.
Incluya asimimsmo un método *EsInterior* que determine si un punto del espacio cartesiano `(x, y)` está o no
dentro del círculo.

3. La clase `Complejo`.

Todo
[número complejo](https://es.wikipedia.org/wiki/N%C3%BAmero_complejo)
puede representarse como la suma de un número real y un número imaginario, de la forma `a + bi` donde el
término `a` es la parte real, `b` la parte imaginaria e `i` la
[unidad imaginaria](https://es.wikipedia.org/wiki/Unidad_imaginaria).

En este ejercicio se propone desarrollar una clase `Complejo` que permita representar y operar con números complejos.

Separe el diseño de su clase `Complejo` en dos ficheros, `complejo.h` y `complejo.cc` conteniendo
respectivamente la declaración y la definición de la clase.
Siga las indicaciones del tutorial 
[Class code and header files](https://www.learncpp.com/cpp-tutorial/89-class-code-and-header-files/)
para realizar esta separación de su clase en dos ficheros.
Siga igualmente las indicaciones del tutorial 
[Header guards](https://www.learncpp.com/cpp-tutorial/header-guards/)
para incluir *header guards* (guardas de cabecera) en sus ficheros de
definiciones (`*.h`) de modo que se evite la inclusión múltiple del mismo fichero.

Desarrolle un programa cliente `complejos.cc` que permita operar con números complejos y haga uso de la clase `Complejo` que diseñe.
La clase `Complejo` ha de contener al menos métodos que implementen la sobrecarga de los operadores de suma y
resta de números complejos así como de los operadores de inserción y extracción en flujos (*streams*).
Así la función `main` del programa `complejos.cc` podría contener (entre otras) sentencias como las siguientes:

```
main() {
  Complejo complejo1{4, 5}, complejo2{7, -8};
  Complejo resultado;
  resultado = complejo1 + complejo2;
  std::cout << resultado;
  resultado = complejo1 - complejo2;
  std::cout << resultado;
}
```
Incluya (discrecionalmente) cualesquiera otras operaciones que considere adecuadas como métodos en la clase `Complejo`.

4. Utilice su clase `Complejo` del ejercicio anterior para resolver el ejercicio
[Complex Numbers](https://exercism.org/tracks/cpp/exercises/complex-numbers)
de Exercism. 
En Exercism el nombre de la clase ha de ser *Complex*.
Es posible que tenga que realizar alguna otra modificación sobre su implementación de la 
clase *Complejo*.
Estudie el fichero `complex_numbers_test.cpp` que contiene los tests de ese problema en Exercism.

5. La clase Fecha.

Desarrolle una clase `Fecha` que permita representar y gestionar fechas.
Incorpore en la clase los miembros de datos y métodos que considere adecuados para la finalidad que se
persigue en este ejercicio.
Incluya un método que permita determinar si el año correspondiente a una fecha es un año bisiesto o
no.
Resuelva el problema 
[Valid Dates](https://jutge.org/problems/P58459_en)
de Jutge y súbalo a la plataforma para su evaluación.
A partir de la solución de ese problema haga que el constructor de la clase `Fecha` solo admita una fecha si
es válida.

Realice un programa cliente `fechas.cc` que tome como parámetro una fecha, un número y un nombre de fichero:
```
./fechas - Gestión de fechas
Modo de uso: ./fechas dd/mm/aa N fichero_salida.txt
Pruebe ./fechas --help para más información
```
El programa deberá imprimir en el fichero de salida (tercer parámetro) las N (segundo parámetro) fechas cronológicamente posteriores a la
introducida (primer parámetro) con una separación de un día entre fechas sucesivas.

