# AeroCVer Risk Predictor ✈️🦉

Sistema de inteligencia artificial para la predicción de riesgos de daños por impactos de aves (Bird Strikes) en la industria aeronáutica.

## 🚀 Estado del Proyecto
**Prototipo Funcional (MVP)**: El sistema es capaz de procesar datos históricos de la FAA/NTSB y predecir la probabilidad de daño físico en una aeronave tras un impacto con fauna.

## 📊 Resultados del Modelo Actual
- **Algoritmo**: Random Forest Classifier.
- **ROC-AUC**: 0.77 (Capacidad de discriminación sólida para un primer prototipo).
- **Dataset**: +25,000 registros de incidentes reales.

## 🛠️ Estructura del Proyecto
- `data/raw`: Dataset original `Bird_strikes.csv`.
- `data/processed`: Contiene el preprocesador (`preprocessor_ohe.pkl`) y el modelo entrenado (`rf_damage_model.pkl`).
- `notebooks`: 
    - `01_exploracion_datos_publicos.ipynb`: Análisis visual y estadístico.
    - `02_preprocesamiento_base.ipynb`: Limpieza, manejo de nulos y encoding.
    - `04_modelos_clasificacion_basica.ipynb`: Entrenamiento y función de inferencia.

## ⚙️ Requisitos e Instalación
Para ejecutar este proyecto, necesitas Python 3.x y las siguientes librerías:
```bash
pip install scikit-learn pandas matplotlib seaborn joblib