# Sesion 1: 27 de enero de 2026

## ¿Porqué R y Python? Como lenguajes de programación para Ciencia de Datos

### Razones no-técnicas pero sí intuivas

-   Tienen un mantenimiento permanente y no centralizado.
     + No pertenecen a una única entidad, ni están alojados en una única ubicación
     + De hecho cuando los instalamos en nuestras compus, ya tenemos una versión del lenguaje
-   Tiene conectividad con diversos tipos de datos y diversas fuentes de datos así como con otros sistemas.
    + SQL, INEGI (a través de Excels, CSVs, API), Yahoo Finance, Google*, Facebook*, Instragram*, X*, 
-   Son suficientemente versátiles para ayudar en la resolución de problemas de diversas áreas.
-   Open source... que significa que cualquiera puede descargar y modificar el código. Esta libertad se conoce como "free as in speech".
-   Multiplataforma (Windows, macOS, Linux)
-   Se usan en la industria, gobierno, investigación, academia.
-   Son gratis. Esta libertad se conoce como "free as in beer".
-   Como consecuencia de esta libertad se tiene que cualquiera puede acceder al código (PÚBLICO), modificarlo e idealmente mejorarlo; es por esto que varias buenas programadoras (sea lo que sea que eso signifique) contribuyan en mejoras y arreglos al código de R y Python

### Razon más técnicas

Ambos son:

-   Interpretados (como Java) y no compilados (como C, C++, Fortran, Pascal, etc), lo que significa que los comandos escritos en el teclado son ejecutados directamente sin necesidad de construir ejecutables.
-   De alto nivel, con sintaxis relativamente legible y productiva.
    + Lenguaje de alto nivel [lejano a la máquina/hardware]: Abstrae los detalles del hardware (le valen los detalles de hardware) y permite a la programadora expresar soluciones en términos más cercanos al problema y no al funcionamiento interno de la máquina.
-   Orientados a la exploración interactiva (Read-Eval-Print Loop (REPL), notebooks).

Esto los hace ideales para:

-   Prototipado rápido
-   Análisis exploratorio de datos
-   Enseñanza y reproducibilidad
-   **Enfoque moderno: ciencia de datos + producción**
-   **Hoy ambos convergen en data pipelines, APIs, MLOps, integración en cloud (AWS, GCP, Azure)**

En ambos:

-   El tipado es dinámico: el tipo se asigna en tiempo de ejecución.
  + No tenemos que definir a priori las variables
  + Se van definiendo conforme las voy necesitando
-   Las funciones son objetos nativos del lenguaje (se les conocen en el argot de programación como first-class citizens).
-   Característica importante: Puedes pasar funciones como argumentos, retornarlas, guardarlas en variables.

Por ejemplo,

-   R: `mi_funcion <- function(x) x^2`
-   Python: `def mi_funcion(x): return x**2`

Ambos soportan varios paradigmas de programación:

-   **Imperativo / procedural**
     + El paradigma imperativo en programación es un enfoque que describe los pasos detallados, de forma secuencial, que una computadora debe seguir para alcanzar un resultado, centrándose en el "cómo" se deben hacer las cosas
     + El paradigma procedural (o procedimental) es un enfoque imperativo basado en la estructuración del código en bloques reutilizables llamados procedimientos, funciones o subrutinas.
   
-   **Funcional** (map, reduce, apply, list comprehensions, purrr, etc.)
-   **Orientado a objetos**

Aunque con diferencias:

-   R: S3, S4, R6
-   Python: clases "clásicas" (... específicas de Python)
-   Pero en la práctica, en data science se usan de forma híbrida.

Administración de paquetes y comunidades abiertas:

-   Repositorios "centrales": R a su `CRAN` y Python a su `PyP`
-   **Crecen a placer/necesidad de la persona usuaria**
-   Les da más versatilidad: limpieza de datos, graficación, ajustes de modelos, etc.
-   Esto quiere decir que son extendibles, i.e. se agregran funcionalidades a través de bibliotecas/librerías
-   Lo más ordenado y funcional es escribir funcionalidades particulares y distribuirlas a partir de bibliotecas/librerías
-   Muchos métodos estadísticos "recientes" se publican conjuntamente con una biblioteca de R y/o Python.

Para análisis de datos y estadística:

-   R: `stats`, `lme4`, `mgcv`, `survival`
-   Python: `scipy`, `statsmodels`, `pymc`

Para machine learning:

-   R: `caret`, `mlr3`, `xgboost`, `randomForest`
-   Python: `scikit-learn`, `xgboost`, `lightgbm`, `tensorflow`, `pytorch`

Ambos están diseñados para:

- Quizá esta es la característica más importante con respecto a desempeño
-   Operar sobre vectores, matrices y arreglos de forma eficiente.
-   Minimizar ciclos explícitos.

Esta herencia de estar vectirizados, viene de:

-   R: S / estadística... S era un software estadístico privados desarrallodo por Ithaka
-   Python científico: NumPy/SciPy (inspirados en MATLAB y R)

Sistemas estándar de instalación:

-   R: `install.packages()`
-   Python: `pip`, `conda`

Integración con C/C++/Fortran para alto rendimiento

-   Llamar código en C/C++/Fortran para acelerar partes críticas.
-   R: Rcpp, .Call
-   Python: cython, ctypes, numba
-   Muchas librerías populares están escritas en C/C++ debajo.
-   Se pueden conectar con otros lenguajes
-   En particular, se han hecho esfuerzos adicionales para conectarlos con sistemas de base de datos. Por ejemplo, los paquetes `RODBC` que lee bases de datos usando el Open Database Connectivity protocol (ODBC) y `ROracle` para leer bases de datos.
-   Gráficos bastante bonitos. Por ejemplo, el departamento gráfico del New York Times usa R.

  Soporte fuerte para reproducibilidad:

-   Notebooks:
    -   R: RMarkdown, Quarto
    -   Python: Jupyter
-   Control de versiones con Git
-   Entornos reproducibles:
    -   R: `renv`, `packrat`
    -   Python: `venv`, `conda`, `poetry`

# Instalación

-   R y RStudio en Windows https://youtu.be/fu_K\_69BDbw?si=fRTORmtNi5ktcbxC

-   R y RStudio en Mac https://youtu.be/EosOpvabcac?si=uAxyAgXA9wttHMOJ

-   R y RStudio en Ubuntu (Linux) https://youtu.be/DGCEFBpkLjM?si=5mxIuZA6P15gqO-R

-   Python en Windows https://youtu.be/QvQgKagWKYk?si=nFUUNv0HXNd9ArRh

-   Python en Mac https://youtu.be/VJjeMdl6yWA?si=14TZtM_fYn5an7ON

-   Python en Ubuntu (Linux) https://youtu.be/m7kDHhuSqVg?si=D5Y8pDD4GUgECGe5

-   Crearse una cuenta en Posit Cloud: https://posit.cloud/

-   Crearse una cuenta de Google y con eso ya tiene una de Google Colab

Tareita para el próximo jueves: Instalar R, RStudio, Python y crearse las cuentas de Posit Cloud y Google Colab

# ¿Dónde tiramos líneas de código?

-   R y Python: En la línea de comando/terminal de nuestra computadora

### Para tirar código de R

-   La consola de R (no lo recomiendo)
-   El editor básico de R (no lo recomiendo... cuesta trabajito hacer REPL)
-   RStudio en mi propia compu (sí lo recomiendo)
-   RStudio Cloud... RStudio en la nube... Sí lo recomiendo para los 3 módulos
-   VS Code (Visual Studio Code)
-   Emacs y Emacs + ESS (Emacs Speaks Statistics)
-   Vim (con plugins Nvim + R plugins)
-   Jupyter Notebook / JupyterLab (sí recomiedo)
-   Sublime Text

### Para tirar código de Python

-   IDLE (el básico que viene con Python) (no lo recomiendo... cuesta trabajito hacer REPL)
-   Jupyter Notebook / JupyterLab
-   RStudio
-   RStudio Cloud
-   VS Code (Visual Studio Code)
-   PyCharm (si sólo quieren hacer Python)
-   Spyder
-   Binder / Kaggle Notebooks
-   Atom
-   Sublime Text

### Para tirar código de Python y R conjuntamente

RStudio con Quarto o Jupyter Notebook / JupyterLab

