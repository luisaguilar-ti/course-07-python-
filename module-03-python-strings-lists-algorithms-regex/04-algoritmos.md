# Algoritmos

## ¿Qué es un algoritmo?

Un algoritmo es un conjunto de reglas que resuelve un problema.

De forma más específica, es un conjunto de pasos que recibe una entrada, realiza tareas y devuelve una solución o salida.

## Diseñar un algoritmo

Antes de escribir código, un problema puede dividirse en partes más pequeñas.

El módulo presenta un ejemplo relacionado con ciberseguridad:

> Un analista de seguridad tiene una lista de direcciones IP y necesita obtener los primeros tres caracteres de cada dirección.

El problema puede dividirse en pasos:

1. Crear una lista de IP.
2. Extraer los primeros tres caracteres de cada IP mediante rebanado.
3. Recorrer la lista con un bucle `for`.
4. Añadir cada resultado a una nueva lista mediante `.append()`.

## Ejemplo del concepto

Para extraer los primeros tres caracteres de una cadena se puede utilizar:

```python
ip_address[0:3]
```

Para almacenar los resultados, se puede crear una lista vacía:

```python
networks = []
```

Y utilizar `.append()` para añadir cada resultado.

La idea principal es **dividir el problema en problemas más pequeños antes de comenzar a programar**.
