# Predicción de Abandono de Clientes en Servicios de Streaming: Netflix (Netflix Churn Prediction)

Este proyecto implementa un modelo de aprendizaje automático basado en **Árboles de Decisión para Clasificación** para predecir la probabilidad de que un usuario cancele su suscripción (*churn*) en una plataforma de streaming. El modelo analiza variables financieras, geográficas y de patrones de uso.

El proyecto está diseñado para ejecutarse de forma nativa y directa en **Google Colab** sin necesidad de configuraciones locales.

---

## Características del Proyecto

* **Carga Dinámica de Datos:** El código fuente importa automáticamente el dataset `netflix_churn.csv` directamente desde este repositorio de GitHub (vía URL Raw), eliminando la necesidad de subir archivos de forma manual a la sesión.
* **Entrenamiento y Visualización:** Procesa los datos, entrena un clasificador de árbol de decisión con una profundidad de 3 niveles (por defecto, puede ser modificado) y grafica el árbol resultante para una fácil interpretación teórica ("modelo de caja blanca").
* **Formulario de Inferencia Interactiva:** Cuenta con un sistema interactivo basado en controles "sliders" y menús desplegables para simular el comportamiento de nuevos clientes y obtener predicciones de riesgo en tiempo real.

---

## Estructura del Repositorio

* `netflix_churn.csv`: Conjunto de datos simulado con registros de usuarios de streaming (Créditos a Abdul Wadood. Obtenido en Kaggle: https://www.kaggle.com/datasets/abdulwadood11220/netflix-customer-churn-dataset)).
* `Netflix_Churn.ipynb`: Cuaderno de Jupyter (Google Colab) con el código fuente del proyecto estructurado y documentado.
* `README.md`: Documentación del repositorio (este archivo).

---

## Dependencias Utilizadas

El entorno de Google Colab cuenta con todas las dependencias preinstaladas de manera nativa. Las librerías utilizadas en el desarrollo son:

* `pandas`: Manipulación y preprocesamiento de datos.
* `numpy`: Operaciones matriciales.
* `scikit-learn`: División de datos (`train_test_split`), entrenamiento del clasificador (`DecisionTreeClassifier`) y graficado del árbol (`plot_tree`).
* `matplotlib`: Renderizado de gráficos en pantalla.

---

## Instrucciones de Ejecución (Google Colab)

Para ejecutar y probar la aplicación interactiva, puedes elegir cualquiera de las siguientes opciones:

### Opción 1: Ejecución Directa en Google Colab (Recomendada - Sin Descargas)
1. Haz clic en el siguiente enlace para abrir la libreta interactiva directamente en la nube:  
   **[Abrir proyecto en Google Colab]([[TU_ENLACE_DE_COMPARTIR_DE_COLAB](https://colab.research.google.com/drive/1b2HbNq-wsXAfwmAnGgXuzeAwZbF1-xkQ?usp=sharing)])**
2. Una vez abierto en Colab, ejecuta cada celda de forma secuencial de arriba hacia abajo haciendo clic en el botón de "Play" de cada celda.
3. Modifica los parámetros en la última celda para interactuar con el sistema de inferencia.

### Opción 2: Ejecución Manual subiendo el archivo .ipynb
1. Descarga el archivo `Netflix_Churn.ipynb` de este repositorio.
2. Abre [Google Colab](https://colab.research.google.com/).
3. Clic en **Subir** (Upload) y arrastra el archivo `.ipynb` que acabas de descargar.
4. Ejecuta cada una de las celdas en orden secuencial haciendo clic en el botón de "Play" de cada celda.
