# Changelog

## [Sprint 3] - Ejercicio 01
### Agregado
  - Creación de la rama Sprint_3 a partir de Sprint_2.
  - Verificación de archivos requeridos del sprint anterior.
  - README.md con objetivo y contexto del Sprint 3.
  - CHAELOG.md con el historial de cambios.
  - gitignore

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

## [Sprint 3] - Ejercicio 07
### Agregado
- Implementación de consultas SQL sobre la base de datos transito.
- Obtención del Top 10 de patentes con mayor cantidad de multas.
- Identificación de multas sin evidencia asociada.
- Análisis de radares con mayor volumen de infracciones.
- Obtención del Top 10 de conductores reincidentes.
- Cálculo del porcentaje de multas confirmadas visualmente.

## [Sprint 3] - Ejercicio 08
### Agregado
- Carga del modelo OpenCLIP (ViT-B-32) para generación de embeddings.
- Creación de la base de datos vectorial ChromaDB `patente_vectorial`.
- Implementación de la función `vectorizar_imagen`.
- Poblado de la colección vectorial con embeddings de imágenes de evidencias.
- Vinculación entre la base relacional (SQLite) y la vectorial (ChromaDB).

## [Sprint 3] - Ejercicio 09
### Agregado
- Creación de la función buscar_patente_imagen.
- Integración de búsqueda de embeddings en ChromaDB.
- Consulta al ORM SQLAlchemy para retornar el historial del Vehículo asociado a la imagen.

## [Sprint 3] - Ejercicio 10
### Agregado
- Redacción de conclusión del trabajo integrador en README.md.
- Síntesis de resultados de todos los ejercicios del Sprint 3.

## [Sprint 3] - Ejercicio 10
### Agregado
- Redacción de conclusión del trabajo integrador en README.md.
- Síntesis de resultados de todos los ejercicios del Sprint 3.
