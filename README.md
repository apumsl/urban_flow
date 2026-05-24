# Urban Flow

## Sprint 2

## Objetivo
Partiendo de los datos procesados y analizados en el Sprint 1,
El objetivo actual es desarrollar un sistema que determine
¿Qué multas tienen evidencia visual válida?


## Introducción y Contexto del nuevo problema
Los radares urbanos generan registros administrativos de multas
de forma automática y las cámaras asociadas registran la
evidencia visual que acompaña y valida de forma visual la infracción.
Sin embargo se plantean los siguientes puntos a tener en consideración:
- No todas las multas tienen una imagen asociada.
- No todas las imágenes corresponden a una infracción.
- Puede haber errores de detección.
- Se utiliza el Dataset de imágenes de la siguiente URL:
https://github.com/HAD141/datasets/raw/refs/heads/main/TrabajosPracticos/urban_flow/urban_flow_plates.zip


## Ejercicio 06 - Conclusiones del Trabajo Práctico

### Relación entre imágenes y datos

#### Sobre el dataset de imágenes
El dataset original contiene 106 imágenes en una sola carpeta. En el Ejercicio 02
clasificamos las imágenes en dos grupos según el nombre del archivo:

- plates (87 imágenes): archivos que contienen la palabra "patente" en su nombre,
  correspondiendo a recortes directos de patentes, con mayor claridad y definición.
- completes (19 imágenes): el resto de las imágenes, correspondiendo a fotografías
  completas del vehículo, donde la patente ocupa una porción menor del encuadre,
  dificultando la detección OCR.

#### Sobre el proceso de OCR y matching
El proceso de extracción mediante EasyOCR presentó limitaciones significativas:

- Solo 23 de las 106 imágenes lograron un match exitoso contra el dataset
  histórico, representando aproximadamente un 21,7% de efectividad.
- Las 83 imágenes restantes (78,3%) no pudieron ser vinculadas a ninguna multa,
  lo que evidencia las dificultades del OCR sobre imágenes del mundo real.

Las principales causas de error identificadas fueron:

- Diversidad de formatos de patentes (distintos países y estándares).
- Ausencia de GPU, lo que limitó la capacidad del modelo EasyOCR.
- Ruido visual en las imágenes (ángulos, iluminación y resolución variable).
- Imágenes de tipo "completes", donde la patente ocupa una pequeña porción
  de la imagen.

#### Sobre la relación con el dataset histórico
Las métricas obtenidas sobre el dataset final permitieron evaluar el nivel de
integración entre las multas registradas y las imágenes procesadas.

- El dataset final contiene 1713 multas registradas.
- Solo 23 multas pudieron vincularse exitosamente a una imagen, mientras que
  1690 multas no poseen evidencia fotográfica asociada.
- Se identificaron 83 imágenes sin coincidencia dentro del dataset histórico,
  evidenciando las limitaciones del proceso de matching implementado.
- Del total de 430 multas impagas registradas, únicamente 7 cuentan con una
  imagen asociada.

#### Conclusión general
El sistema demuestra que la validación visual de infracciones es un problema
complejo. La baja tasa de matching refleja que un enfoque basado únicamente
en OCR directo no resulta suficiente para alcanzar niveles de precisión
adecuados en un entorno real. Sería necesario incorporar técnicas de
preprocesamiento de imágenes, modelos especializados en reconocimiento de
patentes y mejores condiciones de captura.

A pesar de estas limitaciones, el trabajo permitió integrar información de
multas e imágenes en un único dataset consolidado, generando métricas objetivas
que establecen una base sólida para futuras mejoras.
