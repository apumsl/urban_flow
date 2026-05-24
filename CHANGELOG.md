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
