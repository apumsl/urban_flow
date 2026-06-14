# Changelog

## [Sprint 2] - Ejercicio 01
### Agregado
- Se clono el repositorio remoto del TP1 en GitHub via API
- Se crea la rama Sprint_2 partiendo del Sprint_1
- Estructura de directorios para las imagenes del proyecto
- Se descarga dataset zipeado de imágenes desde github
- Se descomprime el dataset en urban_flow/data/raw/imgs
- README.md con objetivo y contexto del Sprint 2
- CHANGELOG.md
- .gitignore

## [Sprint 2] - Ejercicio 02
### Agregado
- Listado de imágenes con nombre y tamaño en KB.
- Clasificación en grupos 'plates' y 'completes' por resolución promedio.
- Diccionario group_images guardado en data/interim/group_images.json.
- Función mostrar_muestra_imagenes para visualizar 8 imágenes aleatorias en tabla 2x4.

## [Sprint 2] - Ejercicio 03
### Agregado
- Procesamiento de imágenes en escala de grises.
- Aplicación de filtro Blur.
- Detección de bordes mediante Canny.
- Generación de los diccionarios dict_grises, dict_blur y dict_canny.

## [Sprint 2] - Ejercicio 04
### Agregado
- Extracción de texto de patentes mediante OCR utilizando EasyOCR.
- Asociación de imágenes con registros del dataset histórico mediante Fuzzy Match con umbral de coincidencia del 80%.
- Incorporación de las columnas imagen, patente_imagen y ratio al dataset.
- Actualización del archivo data/interim/group_images.json con las patentes detectadas.
- Generación del dataset final data/processed/speeding_fines_image.csv.

## [Sprint 2] - Ejercicio 05
### Agregado
- Cálculo de métricas finales sobre el dataset procesado.
- Verificación de registros con imagen asociada.
- Análisis de multas con y sin imagen.
- Generación de conclusiones finales del Sprint 2.
- Limpieza del archivo CHANGELOG.md.

## [Sprint 2] - Ejercicio 06
### Agregado
- Análisis final de los resultados obtenidos.
- Elaboración de conclusiones del Trabajo Práctico.

## [Sprint 3] - Ejercicio 02
### Agregado
- Creación del directorio /content/remote_dvc para simular un remote local de DVC.
- Configuración del remote DVC local.
- Migración de los archivos binarios de gráficos desde Git hacia DVC.
- Generación de los archivos de seguimiento .dvc para cada imagen.

## [Sprint 3] - Ejercicio 03
### Agregado
- Diseño del modelo lógico basado en speeding_fines_image.csv.
- Creación de la entidad Vehiculo.
- Creación de la entidad Multa.
- Creación de la entidad Radar.
- Creación de la entidad Evidencia.
- Definición de relaciones entre las entidades.
- Implementación de métodos __repr__ para mejorar la legibilidad.

## [Sprint 3] - Ejercicio 04
### Agregado
- Implementación de la función procesar_fila_csv.
- Mapeo de filas del archivo speeding_fines_image.csv a objetos del modelo lógico.
- Creación automática de instancias Vehiculo, Radar y Evidencia.
- Asociación de las entidades mediante relaciones del dominio.
- Generación de objetos Multa a partir de los registros del dataset.
- Validación del funcionamiento mediante casos de prueba.

## [Sprint 3] - Ejercicio 05
### Agregado
- Diseño del modelo relacional con SQLAlchemy.
- Definición de claves primarias.
- Implementación de claves foráneas.
- Definición de relaciones entre tablas.
- Implementación de métodos __repr__.

## [Sprint 3] - Ejercicio 06
### Agregado
- Creación de la base de datos SQLite transito.db.
- Creación automática de tablas mediante SQLAlchemy.
- Migración de datos desde speeding_fines_image.csv.
- Inserción de registros de Vehiculo, Radar, Multa y Evidencia.
- Validación de la cantidad de registros insertados.
