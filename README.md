# Clasificación de enfermedades en platas
Desarrollo de un modelo clasificador de enfermedades en plantas (Healthy, Rust, Powdery) con aprendizaje profundo a través de redes neuronales convolucionales y transferencia de aprendizaje.
## Introducción
...
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
<td><img src="https://storage.googleapis.com/kagglesdsdata/datasets/1447507/2394131/Test/Test/Healthy/8df452e2e38c0b6e.jpg?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=databundle-worker-v2%40kaggle-161607.iam.gserviceaccount.com%2F20230110%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20230110T091822Z&X-Goog-Expires=345600&X-Goog-SignedHeaders=host&X-Goog-Signature=7d3226d301f09d4ab968647f4dec0f05ae95bc980f78315efdf7d6e3b03ef078617a93e1d3055b26382caa80bd0c8db557fb8a9f29ccda7a98b9ea5f170f1af032a8b4b2639375a64713c8f21f126e4bdbb3d2d0cc56623c78ae5f873ed34f1d0d29e7a6b79f48ef0bc3ea45f061d6e943a06994033f39c6cb9f5b94c77ab123d5d4214e83f1465be419c45d93d33284de82aae2c2303e6a0f5ca03dcf69cc9d4a8ea61342f782dfca70d175e66001f846d1fc104856abe3dd8de8bd62b57ab61fd98c72aca89173b4bc4dc06995d34353d0908df6846f67569ea3ce64b8d23318739f5deb28dccac1cad488cba567414f960afb551c6dc5d996dc7a1e3df54f" alt="Healthy" width="240" height="167" /></td>
<td><img src="https://storage.googleapis.com/kagglesdsdata/datasets/1447507/2394131/Test/Test/Powdery/81f43097df3940d7.jpg?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=databundle-worker-v2%40kaggle-161607.iam.gserviceaccount.com%2F20230111%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20230111T212258Z&X-Goog-Expires=345600&X-Goog-SignedHeaders=host&X-Goog-Signature=929bb647eb059fab125a2b0cad47e3703a125007a4d64b61776a99be44df22727f12b9d75554555c2b80e166a2be9c2f4a932808c42df64471d6379437570ccaf91d2a06ecf3ebc0a68ddc865d6300b60cc6292f2e40b73fc6fb73a44ccf6b389086ca09ceff79f86f1f3bea1254ff2ff28a130fa7554cb1d4276e573ec45b8ffcf119a64292030867a4b810dfc77a5c6eaa487fa56af191ee00ca4a3368882b94bf39b7f84e39f0cb24bf4312131c3cad7ee0a39a433355376de14a64cc91013727f302578cba15c6ded7233f7091da14ef8a8a9c51d5b9c592e82e432d452398078821390ec54f9153be883c145f87f7c95187cfbe0a7b61b60a92ba06e532" alt="Powdery" width="240" height="167" /></td>
<td><img src="https://storage.googleapis.com/kagglesdsdata/datasets/1447507/2394131/Test/Test/Rust/831abdc76c05e23d.jpg?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=databundle-worker-v2%40kaggle-161607.iam.gserviceaccount.com%2F20230110%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20230110T091830Z&X-Goog-Expires=345600&X-Goog-SignedHeaders=host&X-Goog-Signature=4cdfb609c02da2a3c57a57e98e907d78791f2febbc59c47a97b4b0476e36d1e2ad38b3cc8c95556ea346526c8618ae3a434f69148acfb5ab5aa2f5a40ef27ab6e513c3c9249bb497bcecfd84256174c4199bf6b9bd8fe73673a87b07eab60765bcfecc8974733f0b93ed6fdc9923ea9176ea36d000a8a8251a04745fe285b3ec765db2d9393fd74a87d66ba40ec285924e9b13a1f04b6e6feef087750722f40da2bd3a8b616aab50597d94196661ee706740a8699d99b03c3fed4558942b2d792a7138b63b025d54f3390c798ed6698e9ea1da260a22b7420ed07259244a349c63859c37003ad1ffcffe4ade6c9fa68f889f8bd0bc1fed05f6248165d23e2e0c" alt="Rust" width="240" height="167" /></td>
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
| [02 - Conjunto de Datos](https://colab.research.google.com/github/JLopez86/fastbook/blob/master/02_Conjunto_de_datos.ipynb)
| [03 - Redes Neuronales Convolucionales](https://colab.research.google.com/github/JLopez86/fastbook/blob/master/03_Red_Neuronal_Convolucional.ipynb)
| [04 - Transferencia de Aprendizaje](https://colab.research.google.com/github/JLopez86/fastbook/blob/master/04_Transfer_Learning.ipynb)
| [Conclusión](https://#)
