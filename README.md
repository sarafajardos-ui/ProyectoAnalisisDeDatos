# Análisis exploratorio y predictivo de fallas en la entrega de medicamentos
Este repositorio contiene el desarrollo del proyecto de analítica de datos enfocado en identificar, analizar y predecir fallas en la entrega de medicamentos para enfermedades 
crónicas en el departamento de **Cundinamarca (Colombia)**, a partir de registros de Peticiones, Quejas y Reclamos (PQR).

El proyecto aplica técnicas de **análisis exploratorio**, **modelos predictivos** y **explicabilidad** para apoyar la toma de decisiones en la priorización de casos con 
posible **riesgo vital**.

# Objetivo del proyecto

Aplicar técnicas de analítica de datos para identificar patrones, zonas críticas y variables asociadas al riesgo vital en fallas de entrega de medicamentos, y construir modelos 
predictivos que permitan **anticipar y priorizar** casos críticos dentro del sistema de salud.

# Descripción general

A partir de una base de datos oficial de PQR relacionadas con medicamentos:

- Se realiza limpieza y preparación de datos  
- Se ejecuta un análisis exploratorio (EDA)  
- Se construyen modelos predictivos:
  - Regresión logística
  - Random Forest
  - XGBoost
- Se comparan métricas de desempeño (Accuracy, F1-score, AUC)
- Se interpreta el modelo mediante **SHAP**

La variable objetivo es **riesgo_vida**, transformada a una variable binaria para clasificación.

# Contenido del repositorio

- `Análisis Exploratorio`  
  Notebook principal con todo el flujo de análisis:
  - Limpieza de datos  
  - Análisis exploratorio  
  - Modelado predictivo  
  - Evaluación de modelos  
  - Interpretabilidad (SHAP)
 
- `Presentación`
    - Pptx resumen del proyecto
    
- `Video`
    - Video resumen de la presentación    

- `README.md`  
  Documento descriptivo del proyecto (este archivo)

# Cómo ejecutar el notebook en Google Colab

## Opción 1: Desde GitHub (recomendado)

1. Abre el archivo `ACA2_AnalíticaTomaDecisiones.ipynb` en GitHub  
2. Haz clic en **Open in Colab** (si aparece)  
   - O copia la URL del notebook
3. Ve a https://colab.research.google.com
4. Selecciona **Archivo → Abrir cuaderno → GitHub**
5. Pega la URL del repositorio o del notebook y ábrelo

## Opción 2: Subiendo el archivo manualmente

1. Descarga el archivo `.ipynb` desde este repositorio
2. Ve a https://colab.research.google.com
3. Selecciona **Archivo → Subir cuaderno**
4. Carga el archivo descargado

## Requisitos

El notebook está diseñado para ejecutarse directamente en **Google Colab**, por lo que **no requiere instalación local**.

Librerías utilizadas (ya disponibles en Colab):

- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- xgboost  
- shap  

> En caso de ser necesario, el propio notebook incluye celdas para instalación automática.

## Resultados esperados

- Identificación de patrones en las PQR relacionadas con medicamentos
- Comparación de modelos predictivos para clasificación de riesgo vital
- Modelo con mejor desempeño basado en XGBoost
- Visualizaciones explicativas mediante SHAP para interpretar decisiones del modelo

## Consideraciones éticas

- Se utilizan únicamente **datos públicos y anonimizados**
- El modelo es una **herramienta de apoyo**, no sustituye la evaluación clínica
- Los resultados deben interpretarse como **asociaciones estadísticas**, no causalidad

## Autores

- Angélica María León  
- Sara María Fajardo  
- David Alexander Sabogal  

Especialización en Analítica de Datos  
Bogotá D.C., 2026

---

## Licencia

Este proyecto se desarrolla con fines **académicos**.
