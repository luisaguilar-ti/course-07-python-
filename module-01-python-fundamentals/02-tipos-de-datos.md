# 02 - Tipos de datos en Python

## Introducción

Los datos son la información con la que trabaja un programa. En Python, cada dato pertenece a una categoría denominada **tipo de dato**, la cual determina cómo se almacena y qué operaciones pueden realizarse sobre él.

Comprender los tipos de datos es fundamental para escribir programas correctos y evitar errores.

---

# Objetivos de aprendizaje

Al finalizar este tema podrás:

- Comprender qué es un tipo de dato.
- Identificar los tipos de datos básicos de Python.
- Reconocer las principales estructuras de datos introducidas en el curso.
- Utilizar la función `type()` para identificar el tipo de un dato.
- Comprender qué es un error de tipo (*TypeError*).

---

# ¿Qué es un tipo de dato?

Un **tipo de dato** es una categoría que clasifica un valor según la clase de información que representa.

Cada tipo de dato tiene características y comportamientos específicos.

---

# Datos enteros (Integer)

Los datos enteros representan números sin parte decimal.

### Ejemplos

```python
10
0
-25
1000
```

Se utilizan para contar elementos, almacenar cantidades o realizar operaciones matemáticas con números enteros.

---

# Datos flotantes (Float)

Los datos flotantes representan números que contienen un punto decimal.

### Ejemplos

```python
10.5
3.1416
0.25
-8.75
```

Se utilizan cuando es necesario trabajar con valores decimales.

---

# Datos booleanos (Boolean)

Los datos booleanos solo pueden tener uno de dos valores posibles:

- `True`
- `False`

Generalmente se utilizan para representar el resultado de una condición.

### Ejemplo

```python
True
False
9 < 7
```

La expresión `9 < 7` produce el valor:

```python
False
```

---

# Datos de cadena (String)

Una cadena es una secuencia ordenada de caracteres.

Las cadenas se escriben entre comillas simples o dobles.

### Ejemplos

```python
"Google"

"Cybersecurity"

"Login successful"
```

Las cadenas se utilizan para almacenar texto.

---

# Datos de lista (List)

Una lista es una colección ordenada de elementos.

Puede almacenar múltiples valores en una sola variable.

### Ejemplo

```python
["bmoreno", "tshah", "elarson"]
```

Las listas se utilizan con frecuencia para recorrer elementos mediante bucles.

---

# Datos de tupla (Tuple)

Una tupla es una colección ordenada de datos que **no puede modificarse** después de ser creada.

---

# Datos de conjunto (Set)

Un conjunto es una colección **desordenada** cuyos elementos son únicos.

No admite valores duplicados.

---

# Datos de diccionario (Dictionary)

Un diccionario almacena información mediante pares **clave-valor**.

Cada clave está asociada a un valor específico.

---

# Identificar el tipo de un dato

Python proporciona la función `type()` para conocer el tipo de un valor.

### Ejemplo

```python
print(type(51.1))
```

Salida

```python
<class 'float'>
```

Otro ejemplo:

```python
print(type(True))
```

Salida

```python
<class 'bool'>
```

---

# Error de tipo (TypeError)

Un **TypeError** ocurre cuando se intenta realizar una operación utilizando un tipo de dato incorrecto.

Comprender los tipos de datos ayuda a evitar este tipo de errores durante el desarrollo de programas.

---

# Resumen de tipos de datos

| Tipo | Descripción |
|------|-------------|
| Integer | Número sin decimal. |
| Float | Número con decimal. |
| Boolean | Solo puede ser `True` o `False`. |
| String | Secuencia de caracteres. |
| List | Colección ordenada de elementos. |
| Tuple | Colección ordenada que no puede modificarse. |
| Set | Colección desordenada de valores únicos. |
| Dictionary | Colección de pares clave-valor. |

---

# Puntos clave

- Todo valor en Python pertenece a un tipo de dato.
- Los enteros y flotantes representan valores numéricos.
- Los datos booleanos solo pueden ser `True` o `False`.
- Las cadenas almacenan texto.
- Las listas permiten agrupar varios elementos.
- Las tuplas son inmutables.
- Los conjuntos almacenan valores únicos.
- Los diccionarios utilizan pares clave-valor.
- La función `type()` permite identificar el tipo de un dato.
- Un **TypeError** ocurre cuando se utiliza un tipo de dato incorrecto.

---

## Siguiente tema

➡️ **[03 - Variables](03-variables.md)**

⬅️ **[Volver al índice del módulo](README.md)**
