# 📚 Implementación de Pilas en Java

## 📌 Descripción del proyecto

Este proyecto consiste en la implementación de una estructura de datos de tipo **pila (Stack)** utilizando el lenguaje de programación Java. La implementación se realiza mediante una lista enlazada, aplicando el principio **LIFO (Last In, First Out)**, según el cual el último elemento en entrar es el primero en salir.

El proyecto está organizado en cuatro clases y archivos Java que trabajan conjuntamente para definir las operaciones de la pila, gestionar sus elementos y comprobar su funcionamiento.

## 🗂️ Estructura del proyecto

```text
Pilas/
├── IStack.java
├── LinkedStack.java
├── Nodo.java
└── Main.java
```

## 🛠️ Descripción de las clases

### 1. IStack.java — Interfaz de la pila

Esta interfaz fue implementada para establecer las operaciones fundamentales que debe ofrecer una estructura de datos de tipo pila. Define los métodos necesarios para insertar elementos, consultar el elemento situado en la cima, extraerlo y comprobar si la pila está vacía.

Su propósito es establecer un contrato que debe cumplir cualquier clase que implemente esta interfaz, separando la definición de las operaciones de su implementación.

### 2. LinkedStack.java — Implementación de la pila

Esta clase fue implementada para desarrollar el funcionamiento de la pila mediante una lista enlazada. Es la encargada de gestionar los elementos almacenados y mantener la referencia al elemento situado en la cima.

Implementa las operaciones definidas en `IStack.java`, permitiendo insertar, consultar y eliminar elementos, así como determinar si la estructura está vacía. Además, utiliza la clase `Nodo.java` para organizar los elementos mediante referencias entre nodos.

### 3. Nodo.java — Estructura de los nodos

Esta clase fue implementada para representar cada elemento de la lista enlazada que constituye la pila. Cada nodo almacena un dato y una referencia al siguiente nodo, lo que permite conectar los elementos de la estructura.

Su función es proporcionar el mecanismo de almacenamiento y enlace necesario para que la pila pueda crecer y reducirse dinámicamente a medida que se insertan o eliminan elementos.

### 4. Main.java — Programa principal

Esta clase fue implementada para servir como punto de entrada del programa y comprobar el funcionamiento de la estructura de datos.

En ella se crea una pila de números enteros y se realizan varias operaciones de inserción, extracción y consulta. De esta manera, permite verificar el comportamiento LIFO y observar los resultados de las operaciones implementadas.

## ⚙️ Tecnologías y conceptos utilizados

* **Java:** lenguaje de programación utilizado para desarrollar el proyecto.
* **Programación orientada a objetos:** organización del código mediante clases y objetos.
* **Interfaces:** definición de las operaciones que debe proporcionar la pila.
* **Genéricos:** posibilidad de trabajar con diferentes tipos de datos.
* **Listas enlazadas:** estructura utilizada para almacenar y conectar los elementos.
* **Principio LIFO:** fundamento del funcionamiento de las pilas.

## 🚀 Cómo ejecutar el proyecto

Para ejecutar el programa, es necesario tener instalado el JDK de Java y abrir una terminal en la carpeta donde se encuentran los archivos.

**1. Compilar el proyecto:**

```bash
javac IStack.java Nodo.java LinkedStack.java Main.java
```

**2. Ejecutar el programa:**

```bash
java Main
```

## 📋 Resultado esperado

Al ejecutar el programa, la salida será:

```text
4 <- hace referencia al elemento top de la pila que se elimino 
3 <- y este hace referencia al nuevo elemento top de la pila 
```

Este resultado demuestra que el elemento insertado en último lugar es el primero en salir y que, después de extraerlo, es posible consultar el nuevo elemento situado en la cima de la pila.

## 🎯 Conclusión

Este proyecto permite comprender la implementación de una pila mediante una lista enlazada, mostrando cómo se pueden distribuir las responsabilidades entre una interfaz, una clase que administra la estructura, una clase que representa los nodos y un programa principal encargado de probar su funcionamiento.

La implementación aplica el principio LIFO y utiliza los conceptos de programación orientada a objetos y genéricos para construir una estructura de datos dinámica y reutilizable.
