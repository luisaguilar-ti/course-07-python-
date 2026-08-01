# Bibliotecas y módulos

## Introducción

Python incluye una gran cantidad de código reutilizable que permite desarrollar programas de forma más rápida y eficiente.

En lugar de escribir todas las funciones desde cero, los programadores pueden reutilizar código ya existente mediante **módulos** y **bibliotecas**.

Este enfoque reduce el tiempo de desarrollo y facilita el mantenimiento del código.

---

# ¿Qué es un módulo?

Un módulo es un archivo de Python que contiene código reutilizable.

Un módulo puede incluir:

- Funciones.
- Variables.
- Clases.
- Constantes.
- Código ejecutable.

En otras palabras, un módulo es un archivo `.py` creado para reutilizar código.

---

# ¿Qué es una biblioteca?

Una biblioteca es una colección de módulos relacionados entre sí.

Una biblioteca agrupa varios módulos que resuelven problemas de una misma área.

```
Biblioteca
│
├── Módulo A
├── Módulo B
├── Módulo C
└── Módulo D
```

Las bibliotecas permiten acceder a miles de funciones ya desarrolladas.

---

# Biblioteca estándar de Python

Python incluye una colección de módulos denominada **Biblioteca estándar de Python** (*Python Standard Library*).

Esta biblioteca viene instalada junto con Python, por lo que no es necesario descargarla.

Contiene herramientas para trabajar con:

- Archivos.
- Fechas.
- Expresiones regulares.
- Estadísticas.
- Directorios.
- Sistema operativo.
- Redes.
- Procesos.
- Matemáticas.
- Y muchas otras tareas.

---

# Módulos mencionados en el curso

## re

Permite trabajar con **expresiones regulares**.

Se utiliza para buscar patrones dentro de un texto.

Aplicaciones en ciberseguridad:

- Buscar direcciones IP.
- Buscar correos electrónicos.
- Detectar patrones en archivos de registro.
- Analizar eventos de seguridad.

---

## csv

Permite trabajar fácilmente con archivos CSV.

Aplicaciones:

- Leer registros.
- Exportar resultados.
- Procesar grandes volúmenes de datos.

---

## os

Permite interactuar con el sistema operativo.

Puede utilizarse para:

- Navegar carpetas.
- Obtener rutas.
- Crear directorios.
- Ejecutar operaciones sobre archivos.

---

## glob

Facilita la búsqueda de archivos utilizando patrones.

Ejemplos:

- Buscar todos los archivos `.log`.
- Buscar todos los archivos `.txt`.
- Localizar archivos por nombre.

---

## time

Permite trabajar con el tiempo del sistema.

Aplicaciones:

- Medir tiempos de ejecución.
- Esperar determinados segundos.
- Automatizar procesos.

---

## datetime

Permite trabajar con fechas y horas.

Aplicaciones:

- Registrar eventos.
- Analizar marcas de tiempo.
- Comparar fechas.
- Crear registros de auditoría.

---

# Bibliotecas externas

Además de la Biblioteca estándar existen miles de bibliotecas desarrolladas por la comunidad.

Estas bibliotecas deben instalarse antes de poder utilizarlas.

El curso menciona dos ejemplos.

---

## Beautiful Soup (bs4)

Se utiliza para analizar documentos HTML.

Aplicaciones:

- Extraer información de páginas web.
- Automatizar consultas.
- Analizar contenido HTML.

---

## NumPy

Biblioteca especializada en operaciones matemáticas.

Permite trabajar con:

- Matrices.
- Vectores.
- Álgebra.
- Estadística.
- Cálculos científicos.

---

# ¿Por qué utilizar módulos y bibliotecas?

Utilizar código ya desarrollado ofrece múltiples ventajas.

- Reduce el tiempo de programación.
- Evita duplicar código.
- Mejora la organización.
- Hace el código más fácil de mantener.
- Permite reutilizar soluciones ampliamente probadas.

---

# Aplicación en ciberseguridad

Los módulos y bibliotecas ayudan a automatizar numerosas tareas.

Ejemplos:

- Analizar registros.
- Buscar patrones en logs.
- Leer archivos CSV.
- Procesar directorios completos.
- Trabajar con fechas de eventos.
- Automatizar análisis de incidentes.
- Analizar páginas web.
- Realizar cálculos estadísticos.

---

# Buenas prácticas

- Utilizar primero la Biblioteca estándar de Python antes de instalar bibliotecas externas.
- Elegir módulos especializados para cada tarea.
- Reutilizar código existente en lugar de desarrollar soluciones desde cero.
- Mantener organizadas las dependencias del proyecto.

---

# Resumen

| Módulo / Biblioteca | Uso principal |
|---------------------|---------------|
| re | Expresiones regulares |
| csv | Archivos CSV |
| os | Sistema operativo |
| glob | Buscar archivos |
| time | Tiempo |
| datetime | Fechas y horas |
| Beautiful Soup | HTML |
| NumPy | Matemáticas y matrices |

---

# Conceptos clave

- Biblioteca
- Módulo
- Biblioteca estándar de Python
- Código reutilizable
- Dependencias
- Automatización
- `re`
- `csv`
- `os`
- `glob`
- `time`
- `datetime`
- Beautiful Soup
- NumPy
