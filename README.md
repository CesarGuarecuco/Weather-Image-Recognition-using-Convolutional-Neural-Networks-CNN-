# Weather Image Recognition using Convolutional Neural Networks (CNN)

### Descripción del modelo
Este repositorio contiene el código y los recursos necesarios para entrenar y evaluar un modelo de red neuronal convolucional (CNN) destinado a la clasificación de imágenes según diferentes condiciones meteorológicas. El proyecto utiliza un dataset de imágenes del tiempo, que incluye categorías como soleado, lluvioso, nevado, nublado, entre otros.

### Dataset
El dataset utilizado en este proyecto proviene de Kaggle y se llama "Weather Image Recognition". Contiene imágenes organizadas en carpetas según la categoría meteorológica correspondiente. El dataset está dividido en dos conjuntos principales:

 ##### Train: Usado para entrenar el modelo.
 ##### Test: Usado para evaluar el rendimiento del modelo

 ### Transformaciones de Datos
Para mejorar la capacidad del modelo para generalizar a nuevos datos, se aplican diversas técnicas de aumento de datos (data augmentation) al conjunto de entrenamiento:

##### Redimensionado de imágenes a 64x64 píxeles.
##### Rotación aleatoria.
##### Recorte aleatorio con diferentes escalas.
##### Normalización de los valores de los píxeles.

### Modelo de Red Convolucional
El modelo CNN está construido utilizando PyTorch y consta de las siguientes capas:

Tres capas convolucionales seguidas de capas de pooling.
##### Dos capas completamente conectadas.
##### Función de activación ReLU.
##### Softmax para la salida de clasificación.
      
### Entrenamiento y Evaluación
El modelo se entrena usando el optimizador Adam y la función de pérdida de entropía cruzada. Durante el entrenamiento, se mide la pérdida y la precisión para monitorizar el rendimiento del modelo. Los resultados se evalúan en el conjunto de prueba después del entrenamiento.
