# 🎮 Análisis Actuarial y Modelado Predictivo: Mercado de Videojuegos

## 📌 Descripción del Proyecto
Este proyecto aplica metodologías actuariales, financieras y de Machine Learning para evaluar el riesgo y la rentabilidad en la industria del desarrollo de videojuegos. Utilizando el dataset `vgsales.csv`, el análisis trasciende la simple estadística descriptiva para ofrecer herramientas de toma de decisiones estratégicas basadas en flujos de caja esperados, probabilidades de supervivencia comercial y simulaciones de riesgo.

El objetivo central es proporcionar a desarrolladores y *publishers* un marco cuantitativo riguroso para la asignación de presupuestos, diversificación de portafolios y evaluación de viabilidad antes de comprometer capital.

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
3. **Modelado Predictivo:** Entrenamiento de un modelo **Random Forest Regressor** para pronosticar el volumen de ventas globales en función de decisiones de diseño (plataforma, género).
4. **Análisis de Supervivencia Comercial:** * Estimación **Kaplan-Meier** para calcular la probabilidad de que un título mantenga ventas superiores a 1M de copias a lo largo del tiempo.
   * Modelo de **Riesgos Proporcionales de Cox** para aislar el *Hazard Ratio* de géneros y plataformas.
5. **Evaluación de Riesgo y Sensibilidad:** Implementación de simulaciones de **Monte Carlo** para proyectar el Valor Actual Neto (VAN), incorporando volatilidad en costos de desarrollo y tasas de descuento.

## 📊 Insights Estratégicos y Conclusiones
* **Longevidad Comercial:** El análisis de supervivencia reveló que el género *Shooter* y las plataformas de sobremesa tienen una menor probabilidad de caída abrupta en ventas (Hazard Ratio < 1).
* **Gestión de Portafolio:** Se demostró matemáticamente que los géneros de *Action* y *Shooter* en consolas de última generación concentran la mayor rentabilidad potencial, mientras que los *Sports* funcionan como inversiones de menor volatilidad (menor Coeficiente de Variación).
* **Pensamiento Crítico (Stress Testing):** El análisis avanzado de sensibilidad permitió someter el modelo a pruebas de estrés, identificando límites en los supuestos de márgenes netos y tiempos de recuperación, validando la necesidad de escalar presupuestos dinámicamente según el éxito inicial del título.

## 🚀 Cómo ejecutar este proyecto
1. Clona este repositorio: `git clone https://github.com/TuUsuario/nombre-del-repo.git`
2. Instala las dependencias: `pip install pandas numpy numpy-financial scikit-learn lifelines matplotlib seaborn scipy`
3. Abre y ejecuta el notebook interactivo: `Proyecto_GARH_A2_Final.ipynb`
