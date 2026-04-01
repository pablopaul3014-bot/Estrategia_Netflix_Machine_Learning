
📊 Optimización de Catálogo Netflix con Machine Learning
Netflix Catalogue Optimisation using Machine Learning

Autor / Author: Pablo Peralta Centini
Rol / Role: Desarrollo completo del modelo — EDA, feature engineering, entrenamiento, evaluación e interpretación
Período / Period: Septiembre – Diciembre 2025
Contexto / Context: Proyecto final del curso Data Science & Machine Learning — Coderhouse
Repo original del equipo / Original team repo: pabloper14/Estrategia_Netflix_Machine_Learning


🧠 Mi contribución en este proyecto / My Contribution
Este repositorio es un fork del proyecto grupal. El desarrollo del modelo de Machine Learning fue realizado íntegramente por mí, incluyendo:

Diseño y ejecución del pipeline de ML de punta a punta
Selección de algoritmos (Random Forest y Logistic Regression) y justificación técnica
Feature engineering sobre variables de texto y categóricas (TF-IDF, encoding)
Evaluación con validación cruzada k-fold y métrica AUC-ROC
Interpretación de resultados mediante SHAP Values
Redacción de conclusiones y recomendaciones estratégicas

This repository is a fork of a group project. The Machine Learning model development was carried out entirely by me, including pipeline design, algorithm selection, feature engineering, cross-validation, and SHAP-based interpretation.

🎯 Objetivo del Proyecto / Project Goal

Analizar el catálogo de Netflix y construir modelos predictivos de clasificación para identificar patrones en el contenido que permitan optimizar decisiones de adquisición y producción.
Analyse the Netflix catalogue and build classification models to identify content patterns that support acquisition and production decisions.

📂 Estructura del Repositorio / Repository Structure

├── ml_notebook_final_netflix.ipynb   # Notebook principal con todo el pipeline ML
├── netflix_proyectoFinal_pdf.pdf     # Informe final del proyecto
├── Cinema_Netflix_Estrategia.pptx    # Presentación ejecutiva de resultados
└── README.md

🔍 Metodología / Methodology
1. Análisis Exploratorio (EDA)

Exploración de distribuciones de géneros, países, duraciones y años de lanzamiento
Detección y tratamiento de valores nulos
Visualización de tendencias del catálogo por región y tipo de contenido

2. Feature Engineering

Vectorización de texto con TF-IDF sobre campos de descripción y géneros
Encoding de variables categóricas (país, tipo de contenido, rating)
Creación de variables derivadas (antigüedad del título, densidad de géneros)

3. Modelos Entrenados / Models Trained
Modelo                      AUC-ROC                    Observaciones
Logistic Regression        baseline                       Modelo de referencia, alta interpretabilidad
Random Forest              0.67                           Mejor performance, seleccionado como modelo final

Validación con k-fold cross-validation para evitar overfitting
Comparación de curvas ROC entre modelos


4. Interpretación con SHAP
Análisis de importancia de variables a nivel global (feature importance)
Explicación de predicciones individuales con SHAP values
Identificación de las variables con mayor impacto en la clasificación


📈 Resultados Clave / Key Results

AUC-ROC: 0.67 — el modelo supera al clasificador aleatorio (0.5) con capacidad discriminativa moderada
Los géneros y el país de producción resultaron las variables más predictivas según SHAP
El contenido producido en EE.UU., Reino Unido e India mostró los patrones más diferenciados
Random Forest superó a Logistic Regression en todas las métricas evaluadas
El análisis SHAP permitió pasar de un modelo "caja negra" a decisiones explicables


🚀 Tecnologías Utilizadas / Tech Stack
Python 3.10
Pandas / NumPy — manipulación y limpieza de datos
Scikit-learn — modelos ML, validación cruzada, métricas
SHAP — interpretabilidad del modelo
Matplotlib / Seaborn — visualización
TF-IDF (sklearn) — vectorización de texto
SQL — consultas sobre el dataset estructurado

▶️ Cómo reproducir este proyecto / How to Run
bash
# 1. Clonar el repositorio
git clone https://github.com/pablopaul3014-bot/Estrategia_Netflix_Machine_Learning.git
cd Estrategia_Netflix_Machine_Learning
# 2. Instalar dependencias
pip install pandas numpy scikit-learn shap matplotlib seaborn jupyter
# 3. Abrir el notebook
jupyter notebook ml_notebook_final_netflix.ipynb

💡 Aprendizajes / Learnings
La validación cruzada es esencial para evaluar modelos en datasets de tamaño moderado y evitar overfitting
SHAP convierte un modelo complejo en decisiones explicables — clave para contextos de negocio
Un AUC de 0.67 en datos reales no estructurados es un resultado válido y mejorable con más feature engineering
La combinación EDA → Feature Engineering → Modelado → Interpretación es el flujo real de un proyecto de DS


📬 Contacto / Contact
Pablo Peralta Centini
📍 Córdoba, Argentina
🔗 linkedin.com/in/pablo-peralta-centini
🐙 github.com/pablopaul3014-bot

Proyecto realizado con fines académicos y de desarrollo profesional en Data Science & Machine Learning.
Project developed for academic and professional growth in Data Science & Machine Learning.
