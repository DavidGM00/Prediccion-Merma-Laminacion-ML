# Prediccion-Merma-Laminacion-ML
Proyecto final de Machine Learning para predecir pérdidas de material en empaques flexibles.
# Predicción de Merma en el Proceso de Laminación mediante Machine Learning

**Autor:** David Guerra, Ingeniero Industrial  
**Institución:** Facultad de Ingeniería - Universidad de San Carlos de Guatemala  
**Curso:** Introducción a Data Science y Machine Learning  

## Objetivo del Proyecto
El área de laminación de la planta de empaques flexibles actualmente calcula la asignación de materiales utilizando tablas estáticas basadas en porcentajes globales. El objetivo de este proyecto es reemplazar este enfoque empírico con un modelo dinámico de Machine Learning (**Random Forest Regressor**) capaz de predecir los kilogramos exactos de merma basándose en las variables reales de cada orden de producción (máquina, material, gramaje, ancho y peso).

## Tecnologías Utilizadas
* **Lenguaje:** Python
* **Librerías de Datos:** Pandas, NumPy
* **Visualización:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (Random Forest, GridSearchCV, StandardScaler)

## Resultados Clave
1. **Viabilidad Técnica:** Se demostró mediante la Importancia de Variables (*Feature Importance*) que el tamaño de la orden no es el único factor determinante de la merma, validando la necesidad de un modelo multivariable.
2. **Evaluación del Modelo:** Tras mitigar el sobreajuste (*overfitting*) con *Hyperparameter Tuning*, el modelo obtuvo un Error Absoluto Medio (MAE) en validación de **11.03 kg**. 
3. **Diagnóstico y Propuesta:** El margen de error y un $R^2$ de 0.20 en el conjunto de prueba diagnostican claramente una insuficiencia en el volumen de datos históricos (213 registros). Como propuesta de ingeniería, se estableció como prioridad estandarizar la recolección masiva de datos en planta antes de desplegar una calculadora predictiva en el ERP.

## Estructura del Repositorio
* `Proyecto_Final_DavidGuerra.ipynb`: Cuaderno principal de Jupyter con todo el marco teórico, Análisis Exploratorio (EDA), Ingeniería de Características y el entrenamiento del modelo.
* `train.csv` / `test.csv`: Conjuntos de datos extraídos del histórico de producción.

## Cómo visualizar el proyecto
Para revisar el análisis completo, el código ejecutado y las conclusiones detalladas, haz clic en el archivo `.ipynb` ubicado en este repositorio.
