## *Comparación de Modelos Supervisados usando Validación Cruzada*

### *Objetivo*
*El propósito de este trabajo práctico es comparar el rendimiento de distintos modelos de regresión supervisada para predecir el salario individual, aplicando la técnica de validación cruzada como herramienta principal de evaluación.
El ejercicio busca desarrollar una comprensión crítica sobre cómo la estructura del modelo, la naturaleza de los datos y la métrica de evaluación influyen en la selección del modelo más adecuado.*

### *Datos*
*El conjunto de datos empleado corresponde a un dataset público de análisis salarial, obtenido desde Kaggle, este contiene información socioeconómica y laboral de distintos individuos.*
*Características principales:*
   - *Variable dependiente: Income (salario o ingreso individual)*
   - *Tipo de problema: Regresión supervisada*
   - *Observaciones: ~10.000 individuos*
   - *Variables explicativas: edad, género, educación, estado civil, experiencia laboral, entre otras.*

### *Modelos*
*Los modelos seleccionados fueron:*
   - *KNN (K-Nearest Neighbors)	Predice el salario promedio de los k individuos más similares; sensible a la escala de los datos.*
   - *Árbol de Decisión	Segmenta los datos en grupos homogéneos según variables explicativas.*
   - *Regresión Lineal	Modelo base que estima la relación lineal entre los factores socioeconómicos y el salario.*
   - *Random Forest	Ensamble de múltiples árboles que reduce la varianza y mejora la generalización.*

### *Validación cruzada*
*Se utilizó una validación cruzada de 5 particiones (K-Fold), la cual permite estimar el rendimiento promedio y su variabilidad entre distintas divisiones de los datos.*

### *Conclusiones*
   - *Random Forest fue el modelo más eficiente y estable, mostrando la mejor capacidad para capturar la relación entre variables laborales (educación, edad, experiencia, género, etc.) y el salario.*
   - *Regresión Lineal logró resultados razonables, aunque limitados por su estructura estrictamente lineal.*
   - *Árbol de Decisión tuvo un rendimiento variable, evidenciando la necesidad de ajustar parámetros de profundidad o usar técnicas de poda.*
   - *KNN fue el menos eficaz, probablemente debido a la escala y la distribución de los datos numéricos.*
*La validación cruzada permitió evaluar la estabilidad de los modelos y reducir el sesgo de una única división de entrenamiento y prueba.*


