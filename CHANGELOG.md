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
<<<<<<< HEAD
=======
<<<<<<< HEAD
=======

  ## [Sprint 1] - Ejercicio 02
  ### Agregado
  - Dataset raw_speeding_fines.csv descargado y almacenado en urban_flow/data/raw
  - Exploracion inicial:
  - Se muestran las primeras 5 filas del dataset
  - Se analizan los tipos de datos
  - Se cuentan los valores nulos
  
  ## [Sprint 1] - Ejercicio 03
  ###
  - Limpieza y normalización de fechas, horas, ubicaciones y patentes
  - Eliminación de valores nulos y outliers
  - Cálculo de exceso de velocidad real y con tolerancia
  - Dataset guardado
  
  ## [Sprint 1] - Ejercicio 04
  - Creación de la clase FineAnalyzer
  - Implementación de métodos para ranking de patentes, horarios, excesos y ubicaciones
  
## [Sprint 1] - Punto 07
- Agregado análisis final y conclusión del TP
## [Sprint 2] - Ejercicio 03
### Agregado
Se realizo un procesamiento de las imágenes,  donde en cada punto llama a la
función que muestra las imágenes trabajadas en el punto anterior.
La cadena de trabajo es group_images → dict_grises → dict_blur → dict_canny
#  - Grises: desde las originales
#  - Blur: desde las grises ("en escala de grises")
#  - Canny: desde las suavizadas ("sobre las imágenes suavizadas")
>>>>>>> 547b7201d2afdb7b936f24c1f95d3638bac2154c

## [Sprint 2] - Ejercicio 02
### Agregado
- Listado de imágenes con nombre y tamaño en KB.
- Clasificación en grupos 'plates' y 'completes' por resolución promedio.
- Diccionario group_images guardado en data/interim/group_images.json.
- Función mostrar_muestra_imagenes para visualizar 8 imágenes aleatorias en tabla 2x4.

## [Sprint 2] - Ejercicio 02
### Agregado
- Listado de imágenes con nombre y tamaño en KB.
- Clasificación en grupos 'plates' y 'completes' por resolución promedio.
- Diccionario group_images guardado en data/interim/group_images.json.
- Función mostrar_muestra_imagenes para visualizar 8 imágenes aleatorias en tabla 2x4.
>>>>>>> d8058d2c09b353d41c8fda83c96ee8cc354a66d2

## [Sprint 2] - Ejercicio 02
### Agregado
- Listado de imágenes con nombre y tamaño en KB.
- Clasificación en grupos 'plates' y 'completes' por resolución promedio.
- Diccionario group_images guardado en data/interim/group_images.json.
- Función mostrar_muestra_imagenes para visualizar 8 imágenes aleatorias en tabla 2x4.

## [Sprint 2] - Ejercicio 02
### Agregado
- Listado de imágenes con nombre y tamaño en KB.
- Clasificación en grupos 'plates' y 'completes' por resolución promedio.
- Diccionario group_images guardado en data/interim/group_images.json.
- Función mostrar_muestra_imagenes para visualizar 8 imágenes aleatorias en tabla 2x4.

## [Sprint 2] - Ejercicio 03
### Agregado
Se realizo un procesamiento de las imágenes,  donde en cada punto llama a la
función que muestra las imágenes trabajadas en el punto anterior.
La cadena de trabajo es group_images → dict_grises → dict_blur → dict_canny
#  - Grises: desde las originales
#  - Blur: desde las grises ("en escala de grises")
#  - Canny: desde las suavizadas ("sobre las imágenes suavizadas")

## [Sprint 2] - Ejercicio 04
### Agregado
- Extracción de texto de patentes mediante OCR utilizando EasyOCR.
- Asociación de imágenes con registros del dataset histórico mediante Fuzzy Match con umbral de coincidencia del 80%.
- Incorporación de las columnas imagen, patente_imagen y ratio al dataset.
- Actualización del archivo data/interim/group_images.json con las patentes detectadas.
- Generación del dataset final data/processed/speeding_fines_image.csv.
