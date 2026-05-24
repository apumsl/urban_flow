# Changelog

## [Sprint 2] - Ejercicio 01
### Agregado
- Se clonó el repositorio remoto del TP1 en GitHub vía API.
- Se creó la rama Sprint_2 partiendo de Sprint_1.
- Se generó la estructura de directorios para las imágenes del proyecto.
- Se descargó el dataset comprimido de imágenes desde GitHub.
- Se descomprimieron las imágenes en urban_flow/data/raw/imgs.
- Se creó el archivo README.md.
- Se creó el archivo CHANGELOG.md.
- Se creó el archivo .gitignore.

## [Sprint 2] - Ejercicio 02
### Agregado
- Listado de imágenes con nombre y tamaño en KB.
- Clasificación de imágenes en los grupos plates y completes.
- Generación del diccionario group_images.
- Almacenamiento de group_images en data/interim/group_images.json.
- Implementación de la función mostrar_muestra_imagenes para visualizar imágenes aleatorias.

## [Sprint 2] - Ejercicio 03
### Agregado
- Procesamiento de imágenes en escala de grises.
- Aplicación de filtro Blur para suavizado.
- Detección de bordes mediante algoritmo Canny.
- Generación de los diccionarios dict_grises, dict_blur y dict_canny.
- Visualización de resultados en cada etapa del procesamiento.

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
