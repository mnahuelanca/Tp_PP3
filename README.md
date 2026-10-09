# Proyecto de análisis de entregas hortícolas a productores

Trabajo práctico de PP3 — Análisis y Exploración de Datos, centrado en los registros de entregas hortícolas a productores e instituciones de Río Grande, Tierra del Fuego.

## Descripción general

El proyecto aborda la revisión y reorganización de información proveniente de la Dirección de Desarrollo Agroproductivo.

A partir de la planilla original de entregas 2025, se realizó un diagnóstico de los problemas de carga y se desarrolló una planilla maestra para registrar las entregas de 2026 con una estructura uniforme.

Actualmente se cuenta con la versión final de la planilla de esta etapa y una primera versión del dashboard, disponible en PDF. La finalización de la estructura de la planilla no implica el cierre de la carga de datos del año.

## Objetivo

Organizar los registros de entregas para facilitar su carga, consulta y análisis, y aportar información útil para el seguimiento de la actividad agroproductiva local.

Los principales usuarios son el personal administrativo y técnico del área, que utiliza la información para el control operativo y la elaboración de informes de temporada productiva.

## Evolución del trabajo

### Diagnóstico inicial

La revisión de la fuente 2025 permitió identificar:

- Variaciones en los nombres de productores y productos.
- Registros de productos y cantidades combinados como texto.
- Información distribuida en distintas hojas y períodos.
- Dificultades para consolidar y analizar las entregas.

Como primera instancia, se identificaron los valores únicos de productores, estados de inscripción y productos entregados para detectar casos que requerían revisión y estandarización.

### Planilla final 2026

Se desarrolló una nueva estructura que separa los registros de entregas de los catálogos de productores y productos.

La planilla contiene las siguientes hojas:

| Hoja | Función |
| --- | --- |
| ENTREGAS | Registro de fecha, destinatario, producto, cantidad y observaciones. |
| PRODUCTORES | Catálogo con identificador, apellido, nombre, estado de inscripción y un campo para dirección o coordenadas. |
| PRODUCTOS | Catálogo con identificador, nombre, categoría, unidad de medida y observaciones. |
| INICIO | Acceso al dashboard mediante un enlace. |

La hoja ENTREGAS contiene estos campos:

- Nº Entrega
- Fecha
- Productor / Institución
- Apellido y Nombre
- ¿Está Inscripto?
- Producto
- Cantidad
- Observaciones

La selección de productores y productos se realiza mediante listas desplegables. El nombre y el estado de inscripción se recuperan mediante fórmulas desde el catálogo de productores.

Cada fila registra un producto de una entrega; una misma entrega puede abarcar varias filas.

## Dashboard inicial

El archivo [Dash2026.pdf](Dash2026.pdf) contiene la primera versión del dashboard, organizada en dos páginas.

Actualmente presenta:

- Total de bandejas entregadas.
- Comparación de cantidades por producto.
- Distribución según el estado de inscripción.
- Comparación de cantidades por productor.

El PDF es una captura estática del dashboard. Los controles visibles en sus páginas no permiten filtrar el documento. La hoja INICIO de la planilla contiene un enlace al dashboard en línea, cuyo acceso depende de los permisos del informe.

Esta versión se ampliará en próximos avances con más información y nuevas páginas de análisis.

## Archivos del repositorio

| Archivo | Descripción |
| --- | --- |
| [ENTREGAS_HORTICOLAS_2026.xlsx](ENTREGAS_HORTICOLAS_2026.xlsx) | Planilla final de esta etapa. |
| [Dash2026.pdf](Dash2026.pdf) | Exportación del dashboard inicial. |
| [ENTREGAS2025Google.xlsx](datos/ENTREGAS2025Google.xlsx) | Fuente utilizada para el diagnóstico inicial. |

## Estructura del repositorio

```text
.
├── README.md
├── .gitignore
├── ENTREGAS_HORTICOLAS_2026.xlsx
├── Dash2026.pdf
└── datos/
    └── ENTREGAS2025Google.xlsx
```

## Próximos avances

- Incorporar nuevas páginas y análisis al dashboard.
- Ampliar la información presentada.
- Actualizar el PDF con cada avance relevante.
- Mantener la documentación alineada con los archivos disponibles.
