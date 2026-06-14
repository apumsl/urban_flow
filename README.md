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
