# TP1 — Ciencia de Datos 2026
**UTN Santa Fe** | Entrega: 21/05/2026

## Descripción

Trabajo práctico de análisis y modelado sobre un dataset sintético de **mantenimiento predictivo industrial**. El objetivo es predecir fallas en equipos a partir de variables de operación, aplicando el pipeline completo de ciencia de datos: exploración, preprocesamiento y aprendizaje automático.

## Dataset

Archivo: `i40 (datos).csv` — 14.521 registros de equipos industriales.

| Columna | Descripción |
|---|---|
| `idx` | Índice del registro |
| `parent_device_id` | ID del equipo |
| `product_type` | Tipo de producto (L, M, H) |
| `air_temp` | Temperatura del aire [K] |
| `process_temp` | Temperatura de proceso [K] |
| `speed` | Velocidad de rotación [RPM] |
| `torque` | Torque [Nm] |
| `tool_wear` | Desgaste de herramienta [min] |
| `target` | Variable objetivo: `normal` / `failure` |

## Estructura del proyecto

```
TP1/
├── i40 (datos).csv          # Dataset original
├── eda_Final.ipynb         # Notebook con la solución completa
├── TP 1 (enunciado).pdf     # Enunciado oficial
├── README.md
└── Informe          # Informe oficial
```

## Contenido del notebook

### Parte 1 — Análisis Exploratorio (EDA)
- Vista general del dataset (shape, tipos, nulos, duplicados)
- Medidas de tendencia central (media, mediana, moda)
- Medidas de dispersión (desvío estándar, varianza, rango, IQR, CV)
- Forma de las distribuciones (asimetría, curtosis)
- Proporciones de variables categóricas
- Detección de outliers por criterio IQR
- Correlaciones entre variables
- Visualizaciones: histogramas, boxplots, KDE, scatter plots, heatmaps, violin plots, pairplot

### Parte 2 — Preprocesamiento y Modelos (pendiente)
- Tratamiento de valores erróneos/faltantes y outliers
- Codificación de variables categóricas
- Balance del dataset (dataset desbalanceado: ~6% fallas)
- Normalización
- Al menos 2 modelos de clasificación con búsqueda de hiperparámetros
- Al menos 1 modelo ensamblado
- Comparación de modelos con métricas (accuracy, precision, recall, F1, ROC-AUC)

## Paquetes utilizados

```
numpy  |  pandas  |  matplotlib  |  seaborn  |  scikit-learn
```

## Cómo ejecutar

Abrir `eda_Final.ipynb` en PyCharm Professional o JupyterLab y ejecutar todas las celdas.
