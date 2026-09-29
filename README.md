# Proyecto Final de Data Science — Oil & Gas

## Equipo 11

- Juan Pablo Buenanueva
- Nehuen Riquelme
- Agustin Araneda

## Tema

Análisis exploratorio y futura predicción del desempeño productivo de pozos gasíferos shale de Vaca Muerta.

## Dataset

El proyecto utiliza el dataset público **“Producción de Pozos de Gas y Petróleo No Convencional”**, publicado por la Secretaría de Energía de la Nación en Datos Argentina.

Fuente:
https://www.datos.gob.ar/dataset/produccion-de-petroleo-y-gas-por-pozo

El dataset original contiene información mensual por pozo sobre producción de petróleo, gas y agua, junto con variables técnicas, geográficas y operativas.

## Objetivo

Analizar el comportamiento productivo de pozos no convencionales y evaluar, en etapas posteriores del proyecto, si la información disponible durante los primeros meses de producción permite predecir su desempeño futuro.

A partir del análisis exploratorio se definió como universo de trabajo:

**Cuenca Neuquina → pozos gasíferos → shale → formación Vaca Muerta.**

## Segunda pre-entrega — Análisis Exploratorio de Datos

En esta etapa se realizaron tareas de exploración, validación y transformación utilizando Pandas:

- inspección de estructura, dimensiones y tipos de datos;
- validación de granularidad y duplicados;
- análisis de cobertura temporal y geográfica;
- evaluación de valores faltantes, ceros, negativos y valores extremos;
- análisis de las variables productivas;
- comparación entre recursos shale y tight;
- análisis de historia productiva por pozo;
- construcción de variables temporales relativas al inicio productivo;
- definición y justificación del universo analítico final.

También se realizaron visualizaciones con Pandas para analizar distribuciones, evolución temporal y comportamiento productivo.

## Dataset analítico

Como resultado del EDA se generó un dataset reducido para las próximas etapas del proyecto:

`data/gas_shale_vaca_muerta.csv.gz`

El archivo contiene aproximadamente:

- 46.280 registros;
- 867 pozos;
- producción mensual de pozos gasíferos shale de Vaca Muerta.

El uso de este dataset permite reducir significativamente el volumen de datos y trabajar con una población más homogénea desde el punto de vista productivo.

## Estructura del repositorio

```text
proyecto-final-data-science-oil-gas/
│
├── README.md
├── data/
│   └── gas_shale_vaca_muerta.csv.gz
│
└── notebooks/
    └── 01_validacion_eda_inicial.ipynb