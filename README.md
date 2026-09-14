# Proyecto de análisis de entregas hortícolas a productores

## Descripción general

Este repositorio contiene el trabajo inicial de análisis y limpieza de una planilla de entregas de productos hortícolas a productores de la ciudad. El objetivo principal es transformar la información cruda en una estructura ordenada y normalizada para permitir su análisis, control y uso posterior en reportes o tableros.

La fuente original corresponde a la planilla "Entregas 2025", la cual presenta inconsistencias en la carga de datos, problemas de estructura y dificultades para estandarizar la información de manera uniforme.

## Objetivo del proyecto

- Revisar y evaluar la calidad de la información recibida.
- Identificar inconsistencias en la carga de datos.
- Normalizar nombres de productores, productos y estados de inscripción.
- Preparar una estructura de datos más simple y reutilizable para análisis.
- Generar una base de datos maestra o planilla central que permita trabajar con registros consistentes y con validaciones más claras.

## Problemas detectados en la fuente original

Durante la primera revisión de la planilla se identificaron varios puntos críticos:

- fallas en la estructura de carga de datos;
- inconsistencias en los valores cargados;
- dificultad para normalizar la información;
- nombres y apellidos de productores con registros que requieren una segunda revisión;
- variaciones en la forma de registrar productos entregados;
- ausencia de una estructura uniforme para la captura de información.

## Primer diagnóstico realizado

Como primera instancia, se trabajó con la identificación de valores únicos para los siguientes campos:

- nombres y apellidos de productores;
- productores inscriptos y no inscriptos;
- productos entregados.

Esto permitió detectar la cantidad de variaciones existentes y poner foco en los casos que necesitan limpieza manual o estandarización.

## Propuesta de mejora

Se propone realizar una segunda etapa de limpieza para luego construir una nueva planilla maestra con una estructura más simple y consistente. La idea es reducir la carga manual y evitar errores de normalización.

La nueva estructura sugerida es la siguiente:

- Fecha
- Productor / Institución
- Inscripto
- Producto
- Cantidad

Esta estructura permitirá trabajar con registros más claros y compatibles para análisis posterior. Además, se contempla el uso de tablas índice para administrar los valores que se utilizan en desplegables, con posibilidad de agregar o eliminar registros según corresponda.

## Estructura del repositorio

```text
.
├── README.md
├── avances.txt
├── datos/
│   └── (planillas y archivos de datos)
└── ...
```