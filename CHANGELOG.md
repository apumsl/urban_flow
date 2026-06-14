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
