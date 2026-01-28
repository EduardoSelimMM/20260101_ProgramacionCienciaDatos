# Sesion 1: 27 de enero de 2026

## ¿Porqué R y Python?

-   Tienen un mantenimiento permanente y no centralizado.
-   Tiene conectividad con diversos tipos de datos y diversas fuentes de datos así como con otros sistemas.
-   Son suficientemente versátiles para ayudar en la resolución de problemas de diversas áreas.
-   Open source... que significa que cualquiera puede descargar y modificar el código. Esta libertad se conoce como "free as in speech".
-   Multiplataforma (Windows, macOS, Linux)
-   Se usan en la industria, gobierno, investigación, académica
-   Son gratis. Esta libertad se conoce como "free as in beer".
-   Como consecuencia de esta libertad se tiene que cualquiera puede acceder al código (PÚBLICO), modificarlo e idealmente mejorarlo; es por esto que varias buenas programadoras (sea lo que sea que eso signifique) contribuyan en mejoras y arreglos al código de R y Python

Ambos son:

-   Interpretados (como Java) y no compilados (como C, C++, Fortran, Pascal, etc), lo que significa que los comandos escritos en el teclado son ejecutados directamente sin necesidad de construir ejecutables.
-   De alto nivel, con sintaxis relativamente legible y productiva.
-   Orientados a la exploración interactiva (Read-Eval-Print Loop (REPL), notebooks).

Esto los hace ideales para:

-   Prototipado rápido
-   Análisis exploratorio de datos
-   Enseñanza y reproducibilidad
-   Enfoque moderno: ciencia de datos + producción
-   Hoy ambos convergen en data pipelines, APIs, MLOps, integración en cloud (AWS, GCP, Azure)

En ambos:

-   El tipado es dinámico: el tipo se asigna en tiempo de ejecución.
-   Las funciones son objetos (first-class citizens).
-   Característica importante: Puedes pasar funciones como argumentos, retornarlas, guardarlas en variables.

Por ejemplo,

-   R: `mi_funcion <- function(x) x^2`
-   Python: `def mi_funcion(x): return x**2`

Ambos soportan varios paradigmas:

-   Imperativo / procedural
-   Funcional (map, reduce, apply, list comprehensions, purrr, etc.)
-   Orientado a objetos

Aunque con diferencias:

-   R: S3, S4, R6
-   Python: clases "clásicas" (... específicas de Python)
-   Pero en la práctica, en data science se usan de forma híbrida.

