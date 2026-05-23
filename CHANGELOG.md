# Changelog

## [Sprint 1] - Ejercicio 01
### Agregado
- Inicialización del repositorio remoto en GitHub via API
- Colaboradores agregados al repositorio
- Estructura de directorios del proyecto
- README.md con objetivo y contexto del Sprint 1
- CHANGELOG.md
- .gitignore

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