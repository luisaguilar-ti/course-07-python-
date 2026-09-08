# Cadenas

## ¿Qué es una cadena?

Una cadena (`string`) es una secuencia ordenada de caracteres.

Las cadenas son útiles para trabajar con información que no necesita manipulación matemática. En ciberseguridad pueden representar:

- Direcciones IP.
- Nombres de usuario.
- URL.
- ID de empleados.
- ID de dispositivos.

Las cadenas se escriben utilizando comillas simples o dobles. En el curso se utilizan comillas dobles.

## `str()`

`str()` convierte un objeto en una cadena.

```python
str(10)
```

El entero `10` se convierte en la cadena `"10"`.

## `len()`

`len()` devuelve el número de elementos de un objeto. En una cadena, devuelve el número de caracteres.

```python
print(len("security"))
```

El resultado es `8`.

En el curso también se utiliza `len()` para comprobar longitudes, por ejemplo, al validar un ID de dispositivo.

## Concatenación

El operador `+` combina dos cadenas.

```python
device_id = "IT" + "nwp12"
```

El resultado almacenado en `device_id` es:

```text
ITnwp12
```

No todos los operadores funcionan con cadenas. Por ejemplo, `-` no puede utilizarse para restar cadenas.

## Índices

Los índices indican la posición de cada elemento de una secuencia. En Python, el primer índice es `0`.

La notación entre corchetes permite extraer caracteres.

```python
print("h32rb17"[0])
```

El resultado es:

```text
h
```

También se pueden utilizar índices negativos para trabajar desde el final de la cadena.

## Rebanado

El rebanado permite extraer una parte de una cadena mediante `[inicio:fin]`.

```python
print("h32rb17"[0:3])
```

El resultado es:

```text
h32
```

El primer índice se incluye y el segundo se excluye.

Una subcadena es una secuencia continua de caracteres dentro de una cadena.

## Métodos de cadenas

Un método es una función que pertenece a un tipo de datos específico.

### `.upper()`

Devuelve una copia de la cadena en mayúsculas.

```python
print("Security".upper())
```

Resultado:

```text
SECURITY
```

### `.lower()`

Devuelve una copia de la cadena en minúsculas.

```python
print("Security".lower())
```

Resultado:

```text
security
```

### `.index()`

Busca la primera aparición de un carácter o subcadena y devuelve su índice.

```python
print("Security".index("c"))
```

Resultado:

```text
2
```

Si el elemento buscado no se encuentra, `.index()` genera un error.

Cuando existen varias apariciones, devuelve solamente la primera.

## Inmutabilidad

Las cadenas son inmutables. Esto significa que un objeto de cadena no se puede modificar después de crearlo y asignarle un valor.

Los métodos como `.upper()` y `.lower()` devuelven una copia de la cadena en lugar de modificar la cadena original.
