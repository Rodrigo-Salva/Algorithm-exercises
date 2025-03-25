# 📊 Algoritmos y Estructuras de Datos

## 🔍 Lab02: Recursion and Backtracking

### 📚 Capacidades

- Conocer, comprender y aplicar los algoritmos de recursión y backtracking en la resolución de problemas de software.

### 🔒 Seguridad

- Generar un ambiente seguro.
- Evitar el consumo de alimentos.
- Dejar el ambiente ordenado y limpio.

### 📋 Preparación

- El alumno debe revisar previamente el material cargado.

### 💻 Recursos

- Computadora.

## 📑 Instrucciones

Cada integrante del grupo debe seleccionar un ejercicio diferente y desarrollarlo con la siguiente estructura:

1. **Nombre del alumno**
2. **Ejercicio a desarrollar**
3. **Prompt engineering**
   - Prompt ingresado y captura
   - Análisis del prompt
   - Ajustes del prompt y captura
4. **Comentarios de los compañeros**
5. **Código**
   - Código desarrollado
   - Análisis del código
   - Captura de la ejecución del código
6. **Comentarios de los compañeros**

> **Nota:** Desarrollar todo el código en inglés.

### 📚 Bibliotecas

- [matplotlib](https://matplotlib.org/stable/users/installing/index.html)

## 📊 Ejercicios

### 1️⃣ Recursividad

#### Factorial

1. **Explicación del algoritmo**

   Este algoritmo calcula el factorial de un número de manera recursiva.

   El bloque `if __name__ == "__main__":` asegura que el código solo se ejecute si el archivo se ejecuta directamente.

2. **Tarea a realizar**

   - Graficar el tiempo que demora en ejecutar una función factorial para los valores:

     `1, 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024, 2048, 2080, 2100, 4096.`

   - Hacer su diagrama de flujo.

3. **Comentarios del problema**

   - Hubo un problema con el código porque no se pudo imprimir el factorial usando recursión, por lo que se usó el módulo `math`.

   - ¿Es posible aumentar el tamaño del stack?

     Es posible aumentar el límite de recursión con el módulo `sys`:

     ```python
     import sys

     sys.setrecursionlimit(10000) # Aumentar el límite de recursión
     ```

### 🗼 Torre de Hanoi

1. **Explicación del algoritmo**

   El problema consiste en mover `n` discos de una torre de origen a una torre de destino utilizando una torre auxiliar, siguiendo estas reglas:

   - Solo se puede mover un disco a la vez.
   - Un disco grande no puede estar sobre uno más pequeño.
   - Solo se puede mover el disco superior de una torre.

   El algoritmo funciona recursivamente:

   - Si `n = 1`, el disco se mueve directamente.
   - Si `n > 1`, se sigue este proceso:

     1. Mover `n-1` discos de la torre de origen a la auxiliar.
     2. Mover el disco más grande a la torre de destino.
     3. Mover los `n-1` discos de la torre auxiliar a la torre de destino.

   El número de movimientos requeridos es `2^n - 1`.

2. **Tarea a realizar**

   - Graficar el tiempo que demora en resolverse una Torre de Hanoi con `1, 2, ..., 14` discos.

   - Hacer su diagrama de flujo.

3. **Comentarios del problema**

   - ¿Es posible aumentar el tamaño del stack?

     Sí, utilizando el módulo `sys` en Python.

### 🔢 Backtracking

#### Generación de Binarios

1. **Explicación del algoritmo**

   El algoritmo genera cadenas binarias de longitud `n` usando backtracking:

   - **Caso base:** Si la longitud del resultado es igual a `n`, se imprime la cadena.
   - **Llamadas recursivas:**

     1. Llama a sí misma agregando `0`.
     2. Llama a sí misma agregando `1`.

2. **Tarea a realizar**

   - Calcular el valor de permutación para `3, 4, 5, 6` bits.

   - Hacer su diagrama de flujo.

3. **Comentarios del problema**

   - Es posible aumentar el tamaño del stack con el módulo `sys`:

     ```python
     import sys

     sys.setrecursionlimit(10000)
     ```

### 🚀 Propuesta de Algoritmo

- Proponer un algoritmo que use Backtracking para resolver un problema del 1 al 8 de [adventjs.dev](https://adventjs.dev/), iterando hasta obtener 5 estrellas.

1. **Desarrollo**

   - Incrementos
   - Repositorio
   - Código fuente
   - Informe

## 📌 Conclusiones

- La recursión descompone problemas complejos en subproblemas más pequeños, pero puede consumir mucha memoria.
- El Backtracking explora todas las soluciones posibles descartando caminos no viables.
- Optimizar la recursión es crucial para evitar desbordamientos de pila y mejorar la eficiencia.

---

👨‍💻 **Autor:** [Rodrigo Salva Saccatoma](https://github.com/Rodrigo-Salva/Algorithm-exercises)
