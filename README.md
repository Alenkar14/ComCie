# 🎮 Análisis Actuarial y Modelado Predictivo: Mercado de Videojuegos

## 📌 Descripción del Proyecto
Este proyecto aplica metodologías actuariales, financieras y de Machine Learning para evaluar el riesgo y la rentabilidad en la industria del desarrollo de videojuegos. Utilizando el dataset `vgsales.csv`, el análisis trasciende la simple estadística descriptiva para ofrecer herramientas de toma de decisiones estratégicas basadas en flujos de caja esperados, probabilidades de supervivencia comercial y simulaciones de riesgo.

El objetivo central es proporcionar a desarrolladores y *publishers* un marco cuantitativo riguroso para la asignación de presupuestos, diversificación de portafolios y evaluación de viabilidad antes de comprometer capital.

📄 **Nota:** Puedes consultar la metodología matemática a detalle y el código formateado en el Reporte Técnico PDF adjunto en este repositorio.

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python
* **Manipulación de Datos:** Pandas, NumPy
* **Modelado Financiero:** Numpy-Financial (Cálculo de VAN/NPV y ROI)
* **Machine Learning:** Scikit-learn (Random Forest Regressor, K-Means Clustering, SimpleImputer)
* **Análisis de Supervivencia:** Lifelines (Kaplan-Meier, Cox Proportional Hazards)
* **Visualización:** Matplotlib, Seaborn

## ⚙️ Metodología y Pipeline Analítico
1. **Saneamiento e Imputación:** Tratamiento de valores atípicos y nulos utilizando imputación por mediana para garantizar la robustez frente a la distribución asimétrica (positivamente sesgada) de la industria de los videojuegos.
2. **Segmentación de Mercado (Clustering):** Aplicación de **K-Means** para identificar 4 perfiles comerciales distintos (Éxito Global, Nicho Americano, Nicho Japonés, Mercado Emergente).
3. **Modelado Predictivo:** Entrenamiento de un modelo
