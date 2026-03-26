# Pac-Man Rules - Proyecto en Python

## Descripción

Este proyecto consiste en implementar algunas reglas básicas del clásico juego de arcade **Pac-Man** utilizando Python.

El objetivo es trabajar con **lógica booleana** y funciones que representan diferentes estados del juego, como ganar, perder o sumar puntos.

---

# Objetivo del Ejercicio

Implementar funciones en Python que simulen reglas del juego Pac-Man, combinando diferentes condiciones lógicas para obtener resultados correctos.

El ejercicio se enfoca en:

* Uso de valores booleanos (True / False)
* Uso de operadores lógicos (AND, OR, NOT)
* Definición de funciones
* Reutilización de código

---

# Reglas Implementadas

El programa incluye cuatro funciones principales que representan diferentes situaciones del juego.

---

## Tarea 1: Comer Fantasma

Función: `eat_ghost()`

Pac-Man puede comerse un fantasma **solo si**:

* Tiene una pastilla de energía activa
* Está tocando un fantasma

Regla lógica:

```text
True si: power_pellet_active AND touching_ghost
```

---

## Tarea 2: Anotar Puntos

Función: `score()`

Pac-Man obtiene puntos si:

* Está tocando una bolita de energía
* O está tocando un punto

Regla lógica:

```text
True si: touching_power_pellet OR touching_dot
```

---

## Tarea 3: Perder

Función: `lose()`

Pac-Man pierde si:

* Está tocando un fantasma
* Y no tiene una pastilla de energía activa

Regla lógica:

```text
True si: touching_ghost AND NOT power_pellet_active
```

---

## Tarea 4: Ganar

Función: `win()`

Pac-Man gana si:

* Se ha comido todos los puntos
* Y no ha perdido

Regla lógica:

```text
True si: has_eaten_all_dots AND NOT lose(...)
```

---

# Código del Proyecto

El programa está implementado en Python y contiene las siguientes funciones:

* `eat_ghost()`
* `score()`
* `lose()`
* `win()`

También incluye pruebas en consola para verificar el comportamiento de cada función.

---

# Ejemplo de Ejecución

Salida del programa:

```text
eat_ghost: True
score: True
lose: True
win: True
```

---

# Tecnologías Utilizadas

* Python
* Poetry (gestión de entorno)
* Git y GitHub (control de versiones)

---

# Conclusión

Este ejercicio permite comprender cómo aplicar lógica booleana en programación para modelar situaciones reales, en este caso, reglas del juego Pac-Man.

Además, ayuda a reforzar el uso de funciones, operadores lógicos y la organización del código en Python.
