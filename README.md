# Evaluación 2 - Regresión: Modelado Predictivo de Ingresos Recurrentes (MRR)

**Asignatura:** Inteligencia Artificial (620454) **Semestre:** 2026-2

## Descripción de la Evaluación

Este repositorio contiene el desarrollo de la Evaluación 2, cuyo objetivo es construir un modelo de Regresión Lineal que estime el Ingreso Mensual Recurrente del próximo trimestre (`mrr_proximo_trimestre`) de los 30.000 clientes B2B de SaaSFlow, a partir del dataset "clientes_mrr_dataset.csv". El notebook se organiza en cuatro fases: diagnóstico y calidad de datos (nulos, tipos de dato inconsistentes, sesgos y valores atípicos mediante regla IQR y boxplots), limpieza y transformación (imputación por mediana y moda, antigüedad del cliente en días, codificación ordinal y One-Hot, mapeo numérico y escalado), construcción del modelo (división entrenamiento/prueba 80/20 y regresión lineal) y evaluación e interpretación de métricas. Todo el preprocesamiento se implementó con Pipelines y Column Transformers, incluyendo un transformador propio para la antigüedad, de modo que ningún estadístico se aprende fuera del conjunto de entrenamiento (sin fuga de datos).

El modelo obtuvo un R² de 0,924 y un MAE de 68,32 USD por cliente sobre el conjunto de prueba, validado además con una línea base, validación cruzada de 5 particiones, análisis del error por segmento y análisis de residuos. Los resultados se tradujeron a lenguaje de negocio y a recomendaciones para el equipo de Customer Success en una presentación ejecutiva de 4 diapositivas.

## Integrantes del Grupo

- **Cristóbal Soto Vidal** - [cristobal.soto2301@alumnos.ubiobio.cl](mailto:cristobal.soto2301@alumnos.ubiobio.cl)
- **Martín Romero Álvarez** - [martin.romero2301@alumnos.ubiobio.cl](mailto:martin.romero2301@alumnos.ubiobio.cl)
- **Benjamín Paredes Aguayo** - [benjamin.paredes2301@alumnos.ubiobio.cl](mailto:benjamin.paredes2301@alumnos.ubiobio.cl)
- **Darío Silva Pedreros** - [dario.silva2301@alumnos.ubiobio.cl](mailto:dario.silva2301@alumnos.ubiobio.cl)

## Estructura del Repositorio

El notebook ejecutable (`EV2_IA.ipynb`), el dataset (`clientes_mrr_dataset.csv`) y la presentación solicitada (`Presentacion_EV2_IA.pptx`) se encuentran dentro del directorio "E2-Regresión".
