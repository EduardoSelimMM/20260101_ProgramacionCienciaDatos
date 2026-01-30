# Sesion 2: 29 de enero de 2026

¿y porqué escogimos R y Python para el diplomado?

+ Básicamente porque con que entendamos muy poquitas estructuras... el mundo es nuestro.
+ Con estas estructuras y un poquito de lógica, ya seremos capaces de hacer algo de programación.
+ **Regla de oro:** Nunca se sabe suficiente programación.
+ **Regla de plata:** Haz que una rutina funcione, luego hacer que funcione mejor.

## En R:

Tipos atómicos básicos: Los objetillos más elementales

+ `numeric`: Numeros reales 2.75, 8.92, 567.97, etc.
+ `integer`: Números enteros -3, 7, 10000, 5, etc.
+ `logical`: Valores booleanos -> TRUE y FALSE (también se vale 1 y 0)
+ `character`: Cadenas de caracteres a.k.a strings, "hola", "hola mundo", "palabrejas"
+ `complex`: Numeros complejos -> a + ib, 7+ 8i, 78.9 + 43i, etc.
+ `NULL`: Representa ausencia de objeto
+ `NA`: faltante... 'Not Available'... pensémoslo como un "no sé"
+ `NaN`: indeterminado... 'Not a Number'
+ `Inf`y `-Inf`: infinito y menos infinito

Estructuras básicas... Estructuras para guardar objetos elementales

1. `vector`: Para guardar objetos de la misma naturaleza i.e. puros números, o puros strings, o puros boolenos, etc.
2. `matrix`: Para guardar arreglos bidimensionales de la misma naturaleza i.e. puros números, o puros strings, o puros boolenos, etc.
3. `array`: Para guardar arreglos n-dimensionales, puede que los objetos guardados no sean de la misma naturaleza
4. `list`: Para guardar objetos de distinta naturaleza i.e. puedo guardar en una misma lista un número, un string, un booleano, un vector, etc.
5. `data.frame`: En el corazón de R es una lista. En nuestro entender humano es básicamente una tabla: renglones y columnas.
6. `factor`: Básicamente puede ser un vector, lista o un array con un atributo adicional que se conoce como levels. Supongamos que tenemos un vector `("bajo", "medio", "alto", "alto", "medio")` donde además se sabe que `bajo` < `medio` < `alto`. Es muy común usarlos para variables categóricas
7. `function`: Es una función

+ No nos estresemos de las estructuras 1 - 6 debemos aprender, cómo crearlas, como acceder a sus elementos, como modificarlas (si es que se puede), cómo eliminarlas... i.e. cómo "desentierro" lo que tienen adentro estas estructuras.
+ La estructura `function` es un poquita más complicada que las anteriores.

### En Python:

Tipos atómicos básicos:

+ int: números enteros
+ float: números reales
+ complex: números complejos
+ bool: valores booleanos `true` y `false`
+ str: Cadenas de carácteres.
+ NoneType: Representa ausencia de valor

También existen los conceptos de infinito, NA, NaN pero estos no son universalmente básicos. Si no son objetos que depende de la librería de donde provengan tendrán diferentes propiedades.

Tipos estructuras (contenedores u objetos para guardar/agrupar objetos elementales) básicas

+ `list`: Lista heterogénea y mutable
+ `tuple`: Lista inmutable
+ Diccionario
+ `set`: Conjunto no ordenado, sin duplicados {'día', 'tarde', `noche'}
+ `function`: Función

Otros que no son minimales pero son muy populares. No son básicos de Python, sino de librerías.

+ `numpy.ndarray`: arreglo n-dimensional
+ pandas.Series: serie de valores
+ pandas.DataFrame: tabla

+ Mientras sepamos como crear, modificar, acceder, eliminar estas estructuras... el mundo es nuestro.
