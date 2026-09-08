# Listas

## ¿Qué es una lista?

Una lista es una estructura de datos que consiste en una colección de datos en forma secuencial.

Las listas permiten almacenar múltiples elementos en una sola variable y pueden contener diferentes tipos de datos.

En ciberseguridad pueden utilizarse para almacenar:

- Nombres de usuario.
- Direcciones IP.
- URL.
- ID de dispositivos.
- Aplicaciones bloqueadas.
- Otros datos.

## Crear una lista

Las listas se crean utilizando corchetes y separando los elementos con comas.

```python
username_list = ["elarson", "fgarcia", "tshah"]
```

## Índices

Los índices de las listas comienzan en `0`.

La notación entre corchetes permite acceder a un elemento.

```python
username_list = ["elarson", "fgarcia", "tshah"]

print(username_list[2])
```

El resultado es:

```text
tshah
```

## Rebanado de listas

La notación `[inicio:fin]` también puede utilizarse para obtener una parte de una lista.

El resultado del rebanado es otra lista, llamada sublista.

## Concatenación de listas

El operador `+` combina dos listas.

```python
users = ["elarson", "bmoreno"] + ["tshah", "btang"]
```

El resultado es:

```text
["elarson", "bmoreno", "tshah", "btang"]
```

## Listas mutables

A diferencia de las cadenas, las listas son mutables. Sus elementos pueden modificarse, añadirse o eliminarse.

Un elemento puede modificarse mediante notación entre corchetes y asignación.

## Métodos de listas

### `.insert()`

Añade un elemento en una posición específica.

```python
username_list = ["elarson", "fgarcia", "tshah"]
username_list.insert(2, "wjaffrey")
```

La lista pasa a ser:

```text
["elarson", "fgarcia", "wjaffrey", "tshah"]
```

Los elementos posteriores se desplazan.

### `.remove()`

Elimina la primera aparición de un elemento específico.

```python
username_list = ["elarson", "bmoreno", "wjaffrey", "tshah"]
username_list.remove("elarson")
```

La lista pasa a ser:

```text
["bmoreno", "wjaffrey", "tshah"]
```

Si existen elementos duplicados, `.remove()` elimina solamente la primera aparición.

### `.append()`

Añade un elemento al final de una lista.

```python
username_list = ["bmoreno", "wjaffrey", "tshah"]
username_list.append("btang")
```

El nuevo elemento se agrega al final.

`.append()` puede utilizarse con un bucle `for` para construir una lista a partir de otra información.

### `.index()`

Busca la primera aparición de un elemento en una lista y devuelve su índice.

```python
username_list = ["bmoreno", "wjaffrey", "tshah", "btang"]

print(username_list.index("tshah"))
```

Resultado:

```text
2
```

El método `.index()` existe tanto para cadenas como para listas, pero son métodos pertenecientes a tipos de datos diferentes.

## Recorrer listas

Las listas pueden recorrerse con un bucle `for` y combinarse con condicionales. Esto permite procesar sus elementos individualmente.
