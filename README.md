# Sprint7-proyecto-final-telecom-analisis
El objetivo de este proyecto es analizar la base de usuarios y el historial de uso de ConnectaTel para identificar problemas de calidad en los datos, segmentar clientes según edad y nivel de uso, detectar patrones de comportamiento y generar recomendaciones estratégicas para optimizar la oferta comercial de planes.

A través de este análisis se busca responder preguntas clave sobre:
- Calidad y limpieza de datos
- Segmentación de clientes
- Patrones de llamadas y mensajería
- Detección de outliers
- Oportunidades de negocio y mejora de planes.
- Datasets Utilizados
- users_latam.csv
Contiene información demográfica y de registro de los usuarios
usage.csv
Contiene el historial de actividad de cada usuario
plans.csv
Contiene los planes actuales (precio, minutos incluidos, GB incluidos, costo por extra).

Etapas del Análisis Realizadas

Exploración inicial de datos
- Carga de datasets
- Revisión de estructura
- Resumen estadístico
- Exploración de variables categóricas

Limpieza y preparación de datos
- Detección de sentinels (`-999`, `?`)
- Corrección de fechas fuera de rango
- Conversión de columnas a formato fecha
- Manejo de valores nulos (MAR)

Transformación y creación de variables
- Creación de métricas agregadas por usuario:
  - cantidad de mensajes
  - cantidad de llamadas
  - minutos totales
- Segmentación por:
  - grupo de uso
  - grupo de edad

Análisis exploratorio (EDA)
- Histogramas
- Boxplots
- Distribuciones por tipo de plan
- Detección de outliers con IQR

Insights de negocio
- Identificación de segmentos valiosos
- Patrones de uso extremo
- Recomendaciones comerciales

Guía Rápida de Reproducción

Para replicar el análisis:
Cargar los datasets
Ejecutar limpieza de datos:
reemplazo de sentinels
corrección de fechas
validación de nulos
Generar tabla agregada por usuario
Unir datasets
Ejecutar análisis exploratorio
Crear segmentaciones
Revisar insights y conclusiones
