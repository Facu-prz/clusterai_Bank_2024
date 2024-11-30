# clusterai_Bank_2024
ClusterAI - Análisis de Subscripciones Bancarias

### **Introducción**
Este repositorio contiene un análisis exploratorio de datos (EDA) y un pipeline de machine learning (ML) diseñado para predecir la probabilidad de que un cliente bancario se suscriba a una campaña de marketing. El objetivo principal es ayudar al banco a optimizar sus recursos y esfuerzos, segmentando de manera más precisa su público objetivo.

### **Estructura del Proyecto**
1. **EDA (Exploratory Data Analysis):**
   - Análisis estadístico y visualización de datos.
   - Identificación y tratamiento de valores nulos.
   - Análisis de variables categóricas y numéricas con histogramas y gráficos de distribución segmentados por la variable objetivo.
   - Creación de variables dummies para variables categóricas relevantes.
   - Matriz de correlación con un heatmap para identificar relaciones clave entre variables.


2. **Pipeline de Machine Learning:**
   - Implementación de un pipeline en Python utilizando:
     - **Pandas y Numpy:** Para la manipulación de datos.
     - **Matplotlib y Seaborn:** Para la generación de visualizaciones.
     - **Scikit-learn:** Para la implementación de modelos como Logistic Regression y SVC, además de reducción de dimensionalidad con PCA.
     - **TensorFlow:** Para la evaluación de redes neuronales.
   - Balanceo de clases mediante redistribución de la variable objetivo ('Subscription').
   - Comparación de modelos y métricas como Accuracy, AUC-ROC y matriz de confusión.

### **Resultados**
- **Logistic Regression** fue el modelo más efectivo, alcanzando un **accuracy de 0,815** y un **AUC de 0,86**.
- Se exploró la reducción de dimensionalidad con **PCA**, pero los resultados no mejoraron debido a la dispersión de información en las componentes principales.
- El desbalance inicial de la variable objetivo fue corregido para reducir los falsos negativos, priorizando la identificación correcta de clientes potenciales.

### **Referencias**
VanderPlas, J. (n.d.). Python Data Science Handbook. Recuperado de https://jakevdp.github.io/PythonDataScienceHandbook/
James, G., Witten, D., Hastie, T., & Tibshirani, R. (2013). An Introduction to Statistical Learning: With Applications in R. Recuperado de https://www.statlearning.com/
Murphy, K. P. (2022). Probabilistic Machine Learning: An Introduction. Recuperado de https://probml.github.io/pml-book/book1.html
Goodfellow, I., Bengio, Y., & Courville, A. (2016). Deep Learning. Recuperado de https://www.deeplearningbook.org/
Hastie, T., Tibshirani, R., & Friedman, J. (2009). The Elements of Statistical Learning: Data Mining, Inference, and Prediction (2nd ed.). New York: Springer.
Géron, A. (2019). Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow (2nd ed.). O'Reilly Media.
Bishop, C. M. (2006). Pattern Recognition and Machine Learning. New York: Springer.

