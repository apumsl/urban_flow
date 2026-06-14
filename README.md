# Urban Flow

## Sprint 3

## Objetivo
Partiendo de los datos procesados en el Sprint 2,
el objetivo es integrar dos tecnologías de persistencia complementarias:
una base de datos relacional (SQLite con SQLAlchemy) y una base de datos
vectorial (ChromaDB con OpenCLIP) para vincular multas de tránsito
con evidencia fotográfica mediante búsqueda por similitud visual.

## Introducción y Contexto del nuevo problema
El sistema Urban Flow creció en volumen de datos y complejidad.
Los registros de multas e imágenes de patentes requieren una
arquitectura de datos más robusta que permita:
- Persistir el modelo de dominio en una base de datos relacional.
- Almacenar representaciones vectoriales de imágenes de patentes.
- Vincular ambas bases para identificar vehículos a partir de una imagen.
- Mantener trazabilidad del proceso mediante Git y DVC.
## Conclusiones del Trabajo
### Sprint 3: Integración de Bases de Datos Relacionales y Vectoriales

El Sprint 3 cerró el ciclo de evolución del sistema Urban Flow incorporando dos
tecnologías de persistencia complementarias: una base de datos relacional
(SQLite con SQLAlchemy) y una base de datos vectorial (ChromaDB con OpenCLIP).

#### Gestión de versiones y datos binarios
Se configuró un remote local de DVC para desacoplar los archivos binarios del
historial de Git. Los cinco gráficos generados en el Sprint 1 fueron migrados
a DVC, manteniendo trazabilidad mediante archivos .dvc commiteados en Sprint_3.
Se identificó que el remote DVC del Sprint 2 no tenía binarios subidos, por lo
que las imágenes fueron re-descargadas desde el repositorio de datasets original.

#### Modelo de datos
Se diseñó un modelo lógico de cuatro entidades — Vehiculo, Multa, Radar y
Evidencia — y su implementación relacional con SQLAlchemy. El modelo refleja
las relaciones del dominio: 66 vehículos, muchos con más de 20 infracciones,
registradas por 4 radares, con evidencia fotográfica en 23 casos.

#### Base de datos relacional
Se migró el dataset speeding_fines_image.csv (1.713 registros) a transito.db,
resultando en 66 vehículos, 4 radares, 1.713 multas y 23 evidencias.
Las consultas SQL revelaron que WEFLYN lidera el ranking con 38 infracciones,
que el 98,66% de las multas carece de evidencia fotográfica, y que R01
en AV SIEMPRE VIVA es el radar más activo con 439 eventos registrados.

#### Base de datos vectorial
Se integró OpenCLIP (ViT-B-32) para generar embeddings de las 23 imágenes
de patentes, almacenados en ChromaDB con métrica coseno. La función
buscar_patente_imagen permite identificar un vehículo a partir de una imagen
y recuperar su historial completo desde la base relacional, validando la
integración end-to-end del sistema.

#### Limitaciones identificadas
El bajo porcentaje de evidencia fotográfica (1,34%) refleja una restricción
del dataset del Sprint 2. Las fechas inválidas del dataset original fueron
tratadas como 1932-01-01 según la convención establecida en el Sprint 1.
Se detectó además un registro con radar_id nulo en el dataset de origen,
presente en las consultas como valor nan.

#### Conclusión general
El trabajo integrador permitió aplicar progresivamente CRISP-DM, programación
orientada a objetos, ORM, versionado de datos y búsqueda semántica sobre un
caso realista de infracciones de tránsito. El sistema resultante identifica
vehículos infractores a partir de una imagen, consultando en tiempo real
dos fuentes de datos heterogéneas de forma transparente.
