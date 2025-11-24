# ⚡ Advanced JavaScript Logic & Algorithms

> Colección de implementaciones algorítmicas optimizadas, enfocadas en el rendimiento (Big O Notation), estructuras de datos y patrones de diseño en JavaScript moderno.

![GitHub last commit](https://img.shields.io/github/last-commit/TU_USUARIO/TU_REPO)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-yellow)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📖 Sobre el Proyecto

Este repositorio no es solo una colección de ejercicios; es una demostración de ingeniería de software aplicada a la resolución de problemas.

El objetivo principal es pasar de soluciones ingenuas o de "fuerza bruta" ($O(n^2)$) a soluciones óptimas ($O(n)$ o $O(1)$) utilizando las estructuras de datos adecuadas.

### 🎯 Enfoque Técnico
* **Complejidad Temporal:** Reducción de bucles anidados mediante Hash Maps y Sets.
* **Gestión de Memoria:** Uso eficiente de punteros y mutabilidad controlada.
* **Clean Code:** Naming conventions, funciones puras y principios de responsabilidad única.

---

## 🚀 Highlights de Ingeniería

Aquí detallo las optimizaciones más relevantes aplicadas en el código:

| Patrón / Estructura | Problema Resuelto | Mejora de Rendimiento |
| :--- | :--- | :--- |
| **Hash Maps / Frequency Counter** | *Agrupador de Anagramas* | **De O(n log n) a O(n):** Evita ordenamientos repetitivos usando firmas hash. |
| **Set & Búsqueda O(1)** | *Two Sum (Suma de Dos)* | **De O(n²) a O(n):** Elimina el bucle anidado usando memoria para acceso instantáneo. |
| **Stack (LIFO)** | *Validador de Paréntesis* | Manejo robusto de anidación profunda y validación de sintaxis. |
| **Recursividad & Spread Operator** | *Aplanar Arrays (Deep Flat)* | Manipulación de estructuras de datos de profundidad desconocida sin usar `.flat()`. |
| **Optimización Matemática** | *Números Primos* | Reducción drástica de iteraciones limitando el bucle a la raíz cuadrada ($\sqrt{n}$). |

---

## 🛠️ Estructura del Proyecto

El proyecto está modularizado para facilitar la lectura y el testing:

```text
/
├── src
│   ├── algorithms      # Lógica pura (Two Pointers, Sliding Window, Recursion)
│   ├── data-structures # Implementaciones (Stacks, Queues, Sets)
│   └── utils           # Helpers y validadores
├── index.html          # UI interactiva para pruebas en tiempo real
├── style.css           # Estilos minimalistas
└── script.js           # Controlador principal (DOM Manipulation)
````

## 🧪 Pruebas y Demo

He construido una interfaz visual para probar los algoritmos con diferentes inputs y "edge cases".

👉 **[Ver Demo en Vivo (GitHub Pages)](https://www.google.com/search?q=LINK_A_TU_GITHUB_PAGES)**

### Ejemplo de Optimización (Código)

**Problema:** Encontrar dos números que sumen un objetivo.

*❌ Enfoque Ingenuo (Fuerza Bruta):*

```javascript
// Complejidad: O(n^2) - Lento con grandes volúmenes de datos
for (let i = 0; i < arr.length; i++) {
  for (let j = 0; j < arr.length; j++) { ... }
}
```

*✅ Mi Solución (Optimizada):*

```javascript
// Complejidad: O(n) - Escalable y eficiente
const vistos = new Set();
for (const num of arr) {
  if (vistos.has(objetivo - num)) return [objetivo - num, num];
  vistos.add(num);
}
```

-----

## 👨‍💻 Autor

**Julio César Agüero Gómez**
*Full Stack Engineer | Performance Specialist*

Conectando la lógica de backend (Java/Node) con la experiencia de usuario moderna (LitElement/React).

  * [LinkedIn](https://www.google.com/search?q=TU_LINKEDIN)
  * [Portafolio](https://www.google.com/search?q=TU_LINK_AL_PORTAFOLIO_O_GITHUB)

-----

*Este repositorio es parte de mi proceso de actualización continua en Ciencias de la Computación y Arquitectura de Software.*
