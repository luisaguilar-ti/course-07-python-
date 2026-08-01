# Importar módulos en Python

## Introducción

Para utilizar el código contenido en un módulo, primero es necesario importarlo.

Python proporciona dos formas principales de importar módulos de la Biblioteca estándar:

- Importar el módulo completo.
- Importar únicamente las funciones necesarias.

Elegir una u otra dependerá de las necesidades del programa.

---

# La palabra clave `import`

La palabra reservada `import` permite cargar un módulo completo en nuestro programa.

Sintaxis:

```python
import nombre_del_modulo
```

Ejemplo:

```python
import statistics
```

A partir de ese momento, todas las funciones del módulo estarán disponibles.

---

# Utilizar funciones de un módulo

Cuando se importa un módulo completo, es necesario indicar de qué módulo proviene la función.

Se utiliza un punto (`.`).

Sintaxis:

```python
nombre_modulo.funcion()
```

Ejemplo:

```python
import statistics

numbers = [20, 17, 178, 33, 15]

average = statistics.mean(numbers)

print(average)
```

En este caso:

- `statistics` es el módulo.
- `mean()` es la función.

---

# Función `mean()`

La función `mean()` calcula la media (promedio) de un conjunto de datos numéricos.

Ejemplo:

```python
import statistics

numbers = [10, 20, 30]

print(statistics.mean(numbers))
```

Salida:

```
20
```

---

# Función `median()`

La función `median()` calcula la mediana de un conjunto de datos.

Ejemplo:

```python
import statistics

numbers = [10, 20, 30, 40, 100]

print(statistics.median(numbers))
```

Salida:

```
30
```

La mediana es especialmente útil cuando existen valores atípicos (outliers) que pueden alterar el promedio.

---

# Importar funciones específicas

Si solo se necesitan algunas funciones del módulo, es posible importarlas directamente.

Se utiliza la palabra reservada:

```python
from
```

Sintaxis:

```python
from modulo import funcion
```

Ejemplo:

```python
from statistics import mean

numbers = [10, 20, 30]

print(mean(numbers))
```

En este caso ya no es necesario escribir:

```python
statistics.mean()
```

Simplemente:

```python
mean()
```

---

# Importar varias funciones

También pueden importarse varias funciones al mismo tiempo.

Ejemplo:

```python
from statistics import mean, median
```

Ahora ambas funciones estarán disponibles.

```python
print(mean(numbers))

print(median(numbers))
```

---

# Diferencias entre ambos métodos

## Importar el módulo completo

```python
import statistics

statistics.mean(numbers)
```

### Ventajas

- El código indica claramente de qué módulo proviene cada función.
- Reduce conflictos entre funciones con el mismo nombre.

---

## Importar funciones específicas

```python
from statistics import mean

mean(numbers)
```

### Ventajas

- Código más corto.
- Más cómodo cuando solo se utilizan pocas funciones.

---

# Bibliotecas externas

Además de la Biblioteca estándar, Python permite instalar bibliotecas desarrolladas por la comunidad.

Antes de utilizarlas es necesario instalarlas.

Ejemplo en Jupyter Notebook o Google Colab:

```python
%pip install numpy
```

Una vez instalada:

```python
import numpy
```

Ya puede utilizarse dentro del programa.

---

# Bibliotecas mencionadas en el curso

## NumPy

Especializada en:

- Matemáticas.
- Álgebra lineal.
- Estadística.
- Matrices.
- Cálculos científicos.

---

## Beautiful Soup (bs4)

Especializada en:

- Analizar HTML.
- Extraer información de páginas web.
- Procesar documentos HTML.

---

# Aplicación en ciberseguridad

Importar módulos permite reutilizar herramientas especializadas para tareas como:

- Analizar registros.
- Calcular estadísticas.
- Procesar archivos CSV.
- Buscar patrones mediante expresiones regulares.
- Analizar directorios.
- Trabajar con fechas y horas.
- Automatizar procesos.

---

# Buenas prácticas

- Importar únicamente los módulos necesarios.
- Utilizar `import modulo` cuando se empleen muchas funciones del mismo módulo.
- Utilizar `from modulo import funcion` cuando solo se necesiten unas pocas funciones.
- Mantener los `import` al inicio del archivo.
- Evitar importar bibliotecas innecesarias.

---

# Resumen

| Sintaxis | Resultado |
|----------|-----------|
| `import statistics` | Importa todo el módulo |
| `statistics.mean()` | Llama una función del módulo |
| `from statistics import mean` | Importa solo la función `mean` |
| `mean()` | Llama directamente la función importada |

---

# Conceptos clave

- `import`
- `from`
- Biblioteca estándar
- Módulo
- `statistics`
- `mean()`
- `median()`
- NumPy
- Beautiful Soup
- Reutilización de código
