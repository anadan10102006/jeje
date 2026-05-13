# README: ASSIGNMENT III

**Integrantes:** *Maria Lucía Castillo García, Juliana González Sánchez y Ana Daniela Paredes Tovar*

---

# 1.1 Descripción General

La presente actividad tiene como propósito estudiar y comprender el funcionamiento del direccionamiento de memoria en C++ mediante la implementación de distintos ejercicios relacionados con variables, punteros, referencias, memoria dinámica y regiones de memoria como stack y heap.

A lo largo de la actividad se desarrollan diferentes ejercicios prácticos que permiten observar cómo se almacenan los datos en memoria y cómo pueden manipularse utilizando herramientas fundamentales del lenguaje C++.

En particular, la actividad aborda los siguientes temas:

* Variables enteras y direcciones de memoria
* Uso de punteros
* Modificación de variables mediante punteros
* Referencias
* Arrays y direccionamiento
* Memoria dinámica con `new` y `delete`
* Funcionamiento del stack
* Funcionamiento del heap
* Llamadas recursivas y crecimiento del stack

El objetivo principal es visualizar y analizar el comportamiento de la memoria durante la ejecución de un programa.

---

# 1.2 Descripción de la Actividad

La actividad fue desarrollada en C++ utilizando programación orientada a objetos para separar cada ejercicio en diferentes clases y archivos fuente.

Cada actividad busca demostrar un concepto específico relacionado con memoria y direccionamiento.

La implementación incluye:

* Clases para encapsular variables y operaciones sobre memoria
* Uso de punteros para acceder y modificar valores
* Uso de referencias como alias de memoria
* Ejemplos de memoria automática (stack)
* Ejemplos de memoria dinámica (heap)
* Construcción dinámica de arreglos y matrices utilizando `new`
* Liberación manual de memoria utilizando `delete`

Además, se incluyen demostraciones adicionales para visualizar direcciones de memoria y observar diferencias entre stack y heap.

---

# 1.3 Estructura General de la Actividad

La actividad se compone de varios archivos fuente en C++ organizados por ejercicio y demostración.

## Archivos principales

`main.cpp`
Archivo principal encargado de ejecutar todas las actividades y demostraciones.

`VariableEntera.cpp / VariableEntera.h`
Implementación de la actividad relacionada con variables enteras y punteros.

`PunteroVariable.cpp / PunteroVariable.h`
Implementación de la actividad relacionada con punteros y referencias.

`ArregloEnteros.cpp / ArregloEnteros.h`
Implementación de la actividad relacionada con arreglos y direccionamiento mediante punteros.

`MatrizDinamica.cpp / MatrizDinamica.h`
Implementación de matrices dinámicas utilizando memoria reservada manualmente.

`StackDemo.cpp / StackDemo.h`
Demostración del funcionamiento del stack mediante variables locales y llamadas recursivas.

`HeapDemo.cpp / HeapDemo.h`
Demostración del funcionamiento del heap utilizando memoria dinámica.

`CodeDemo.cpp / CodeDemo.h`
Archivo utilizado para demostraciones adicionales y pruebas de ejecución relacionadas con memoria y direccionamiento.

`README.md`
Archivo de documentación de la actividad.

---

# 1.4 Programas Implementados

## Actividad No. 1 — Variables y Punteros

En este punto se crea una variable entera y se realizan operaciones relacionadas con direccionamiento de memoria utilizando punteros.

El programa permite:

* Mostrar el valor de una variable
* Mostrar su dirección de memoria
* Modificar el valor utilizando punteros
* Observar cómo un puntero almacena la dirección de una variable

Durante la ejecución se utilizan los operadores `&` y `*` para acceder y modificar el contenido almacenado en memoria.

---

## Actividad No. 2 — Punteros y Referencias

En este punto se trabaja con punteros y referencias para modificar el valor de una variable encapsulada dentro de una clase.

El programa permite:

* Modificar variables utilizando punteros
* Modificar variables utilizando referencias
* Comparar direcciones de memoria
* Observar cómo referencias y punteros acceden al mismo espacio de memoria

También se muestran las direcciones correspondientes a:

* La variable original
* El puntero
* La referencia

Esto permite analizar cómo las referencias funcionan como alias de una variable existente.

---

## Actividad No. 3 — Arrays y Direccionamiento

En este punto se implementa un arreglo dinámico de enteros utilizando memoria reservada manualmente.

El programa permite:

* Reservar memoria dinámica para arreglos
* Llenar el arreglo por consola
* Modificar posiciones mediante aritmética de punteros
* Mostrar direcciones de memoria de cada elemento
* Liberar memoria utilizando `delete[]`

Cada elemento del arreglo puede ser accedido utilizando punteros y desplazamientos de memoria, permitiendo observar cómo se almacenan los elementos de forma contigua.

---

## Actividad No. 4 — Memoria Dinámica

En este punto se implementa una matriz dinámica bidimensional utilizando memoria reservada en el heap mediante `new`.

El programa permite:

* Reserva dinámica de memoria
* Ingreso de datos por consola
* Visualización de valores almacenados
* Visualización de direcciones de memoria
* Liberación manual de memoria con `delete`

La matriz se construye utilizando punteros dobles (`int**`) y memoria dinámica para filas y columnas.

---

## Demostración del Stack

La demostración del stack utiliza variables locales y llamadas recursivas para visualizar cómo se comporta la memoria automática durante la ejecución del programa.

En cada llamada recursiva se imprime:

* Nivel de llamada
* Valor de la variable local
* Dirección de memoria correspondiente

Esto permite observar cómo el stack crece a medida que se realizan nuevas llamadas a funciones.


---

## Demostración del Heap

La demostración del heap utiliza memoria dinámica creada mediante `new`.

El programa muestra:

* Dirección del puntero
* Dirección reservada en heap
* Liberación manual de memoria

Además, se implementa un arreglo dinámico para observar cómo se almacenan estructuras reservadas dinámicamente.

---

# 2. Formato de Entrada

El programa solicita diferentes valores por consola dependiendo de la actividad ejecutada.

Ejemplo:

```txt
Ingrese el valor inicial de la variable entera:
Ingrese el nuevo valor para modificar la variable:
Ingrese la cantidad de niveles:
Ingrese la cantidad de filas:
Ingrese la cantidad de columnas:
Ingrese el tamanio del arreglo dinamico:
```

En el caso de arreglos y matrices dinámicas, el usuario también debe ingresar los valores correspondientes a cada posición.

---

# 2.1 Formato de Salida

La salida del programa muestra:

* Valores almacenados
* Direcciones de memoria
* Cambios realizados mediante punteros
* Direcciones correspondientes al stack y heap

Ejemplo:

```txt
Valor de la variable: 10
Direccion de memoria de la variable: 0x61ff08
```

Ejemplo para llamadas recursivas:

```txt
Nivel de llamada: 3
Direccion de memoria de la variable local: 0x61fed4
```

Ejemplo para heap:

```txt
Direccion de memoria reservada en heap: 0x98ab20
```

---

# 2.2 Cumplimiento de los Requerimientos

La actividad cumple con los siguientes requerimientos:

## Implementación de actividades de memoria

* Variables y punteros
* Referencias
* Arrays y direccionamiento
* Memoria dinámica

## Uso de programación orientada a objetos

* Clases
* Encapsulamiento
* Separación en archivos `.h` y `.cpp`

## Gestión de memoria dinámica

* Uso de `new`
* Uso de `delete`

## Inclusión de documentación

* README con explicación de la actividad
* Explicación de compilación y ejecución

---

# 3. Compilación de la Actividad en Docker

> Espacio reservado para documentación del Dockerfile y compilación en Docker.

---

# 3.1 Ejecución en Docker

> Espacio reservado para comandos de ejecución en Docker.

---

# 3.2 Ejecución fuera de Docker

Si se desea compilar y ejecutar directamente con `g++`, pueden utilizarse los siguientes comandos.

## Compilación completa del programa

```bash
g++ main.cpp VariableEntera.cpp PunteroVariable.cpp ArregloEnteros.cpp StackDemo.cpp HeapDemo.cpp MatrizDinamica.cpp -o programa
```

## Compilación usando todos los archivos `.cpp`

```bash
g++ *.cpp -o programa
```

## Ejecución en Windows

```bash
programa.exe
```

## Ejecución en Linux / macOS

```bash
./programa
```

---
