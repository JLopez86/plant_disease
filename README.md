# Clasificación de enfermedades en platas
Desarrollo de un modelo clasificador de enfermedades en plantas (Healthy, Rust, Powdery) con aprendizaje profundo a través de redes neuronales convolucionales y transferencia de aprendizaje.
## Introducción
El sector de producción de alimentos y más específicamente el de la agricultura puede verse afectado por la aparición de diversas enfermedades o anomalías en los cultivos que ponen en gran riesgo la seguridad alimentaria de la población mundial. Por lo tanto, la detección y clasificación con precisión de las anomalías presentes en las hojas de los cultivos es altamente necesaria para la toma de decisión en tiempo oportuno.  El objetivo central del presente reporte técnico fue modelar un algoritmo de aprendizaje profundo basado en redes neuronales convolucionales para la detección de enfermedades en hojas de plantas. La metodología empleada fue el desarrollo experimental de diversos modelos de aprendizaje profundo para en primer lugar, entrenar el modelo con los hiperparametros seleccionados como la cantidad de iteraciones, taza de aprendizaje, optimizadores, función de costos y la utilización de técnicas de transformación de datos y aprendizaje transferido sobre el conjunto de datos de enfermedades de plantas previamente recabados y etiquetados. Finalmente se expuso los resultados obtenidos en la predicción de imágenes de validación, constatándose que los mejores resultados fueron obtenidos por los modelos que utilizaron técnicas de aprendizaje transferido.
## Conjunto de datos
El conjunto de datos a utilizar se encuentra clasificada con tres etiquetas: <u>Healthy</u> (saludable), <u>Powdery</u> (polvorienta) y <u>Rust</u> (oxidada) que hacen referencia a las condiciones de la planta. 
<br>
<table border="0">
<thead>
<tr>
<td><b>Healthy</b> / Saludable</td>
<td><b>Powdery</b> / Polvorienta</td>
<td><b>Rust</b> / Oxidada</td>
</tr>
</thead>
<tbody>
<tr>
<td><img src="https://github.com/JLopez86/plant_disease/blob/main/00-IMG/saludable.jpg" alt="Healthy" width="240" height="167" /></td>
<td><img src="https://github.com/JLopez86/plant_disease/blob/main/00-IMG/polvorienta.jpg" alt="Powdery" width="240" height="167" /></td>
<td><img src="https://github.com/JLopez86/plant_disease/blob/main/00-IMG/oxidada.jpg" alt="Rust" width="240" height="167" /></td>
</tr>
</tbody>
</table><br>

**Cantidad de imágenes del conjunto de datos**

Hay un total de **1532** imágenes divididas en conjuntos de entrenamiento, prueba y validación. 

  - **1472** imagenes para entrenamiento y validación. <br>
  - **60** imágenes desconocidas por el modelo.

El conjunto de datos se encuentra disponible en la plataforma [Kaggle](https://www.kaggle.com/) y es posible acceder desde el siguiente [enlace](https://www.kaggle.com/datasets/rashikrahmanpritom/plant-disease-recognition-dataset).
## Colab
Es posible acceder a los distintos archivos de colab desde los siguientes enlaces: [Introducción](https://colab.research.google.com/github/JLopez86/plant_disease/blob/main/01_Introduccion.ipynb)
| [02 - Conjunto de Datos](https://colab.research.google.com/github/JLopez86/plant_disease/blob/main/02_Conjunto_de_datos.ipynb#scrollTo=g1FxZc-noIhN)
| [03 - Redes Neuronales Convolucionales](https://colab.research.google.com/github/JLopez86/plant_disease/blob/main/03_Red_Neuronal_Convolucional.ipynb)
| [04 - Transferencia de Aprendizaje](https://colab.research.google.com/github/JLopez86/plant_disease/blob/main/04_Transfer_Learning.ipynb)

