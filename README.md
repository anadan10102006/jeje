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
* Ejemplos de memoria automática (stack)
* Ejemplos de memoria dinámica (heap)
* Construcción dinámica de matrices utilizando `new`
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

`StackDemo.cpp / StackDemo.h`
Demostración del funcionamiento del stack mediante variables locales y llamadas recursivas.

`HeapDemo.cpp / HeapDemo.h`
Demostración del funcionamiento del heap utilizando memoria dinámica.

`MatrizDinamica.cpp / MatrizDinamica.h`
Implementación de matrices dinámicas utilizando memoria reservada manualmente.

`README.md`
Archivo de documentación de la actividad.

---

# 1.4 Actividades Implementadas

## Actividad No. 1 — Variables y Punteros

En esta actividad se crea una variable entera y se realizan operaciones relacionadas con direccionamiento de memoria.

La actividad permite:

* Mostrar el valor de una variable
* Mostrar su dirección de memoria
* Modificar el valor utilizando punteros

### Conceptos trabajados

* Variables
* Punteros
* Direcciones de memoria
* Operadores `&` y `*`

---

## Actividad No. 2 — Punteros y Referencias

> Espacio reservado para documentación de la Actividad No. 2.

### Conceptos trabajados

* Referencias
* Punteros
* Modificación indirecta de variables
* Alias de memoria

---

## Actividad No. 3 — Arrays y Direccionamiento

> Espacio reservado para documentación de la Actividad No. 3.

### Conceptos trabajados

* Arrays
* Aritmética de punteros
* Direccionamiento de memoria en arreglos
* Acceso mediante índices y punteros

---

## Actividad No. 4 — Memoria Dinámica

En esta actividad se implementa una matriz dinámica bidimensional utilizando memoria reservada en el heap mediante `new`.

La actividad incluye:

* Reserva dinámica de memoria
* Ingreso de datos por consola
* Visualización de valores almacenados
* Visualización de direcciones de memoria
* Liberación manual de memoria con `delete`

### Conceptos trabajados

* Heap
* `new`
* `delete`
* Matrices dinámicas
* Gestión manual de memoria

---

# 2. Funcionamiento de la Actividad

El funcionamiento general de la actividad puede describirse en las siguientes etapas:

## Creación de variables y objetos

El programa solicita datos al usuario y crea las estructuras necesarias para cada actividad.

## Manipulación de memoria

Dependiendo de la actividad ejecutada, el programa:

* Accede a variables mediante punteros
* Modifica valores indirectamente
* Reserva memoria dinámica
* Libera memoria manualmente

## Visualización de direcciones

El programa imprime direcciones de memoria para permitir observar:

* Ubicación de variables en stack
* Ubicación de datos en heap
* Diferencias entre memoria automática y dinámica

## Demostraciones adicionales

Se incluyen ejemplos recursivos y estructuras dinámicas para analizar el crecimiento del stack y el uso del heap.

---

# 2.1 Funcionamiento de las Actividades

## Variables y Punteros

La variable entera es almacenada en memoria y posteriormente se utiliza un puntero para acceder a su dirección y modificar su valor.

Características:

* Uso básico de punteros
* Acceso indirecto
* Visualización de direcciones de memoria

---

## Stack

La demostración del stack utiliza variables locales y llamadas recursivas.

En cada llamada recursiva se imprime:

* Nivel de llamada
* Valor de la variable local
* Dirección de memoria

Esto permite observar cómo el stack crece con cada llamada.

Características:

* Memoria automática
* Liberación automática
* Uso de variables locales
* Recursividad

---

## Heap

La demostración del heap utiliza memoria dinámica creada mediante `new`.

Se muestran:

* Dirección del puntero
* Dirección reservada en heap
* Liberación manual de memoria

Características:

* Memoria dinámica
* Persistencia hasta `delete`
* Gestión manual de memoria

---

## Matriz Dinámica

La matriz dinámica se construye utilizando punteros dobles (`int**`) y memoria reservada dinámicamente.

Características:

* Reserva dinámica por filas y columnas
* Acceso bidimensional
* Liberación manual de memoria

---

# 2.2 Formato de Entrada

El programa solicita diferentes valores por consola dependiendo de la actividad ejecutada.

Ejemplo:

```txt
Ingrese el valor inicial de la variable entera:
Ingrese el nuevo valor para modificar la variable:
Ingrese la cantidad de niveles:
Ingrese la cantidad de filas:
Ingrese la cantidad de columnas:
```

En el caso de la matriz dinámica, el usuario también debe ingresar los valores de cada posición.

---

# 2.3 Formato de Salida

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


# 3. Compilación de la Actividad en Docker

> Espacio reservado para documentación del Dockerfile y compilación en Docker.

---

# 3.1 Ejecución en Docker

> Espacio reservado para comandos de ejecución en Docker.

---

# 3.2 Ejecución fuera de Docker

Si se desea compilar y ejecutar directamente con `g++`, pueden utilizarse los siguientes comandos.

## Compilación

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

# 4. Archivos Incluidos

La entrega incluye los siguientes archivos:

```txt
main.cpp
VariableEntera.cpp
VariableEntera.h
StackDemo.cpp
StackDemo.h
HeapDemo.cpp
HeapDemo.h
MatrizDinamica.cpp
MatrizDinamica.h
README.md
```

---
