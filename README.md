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
<td><img src="https://storage.googleapis.com/kagglesdsdata/datasets/1447507/2394131/Validation/Validation/Healthy/9be41b823d13e3c6.jpg?X-Goog-Algorithm=GOOG4-RSA-SHA256&amp;X-Goog-Credential=databundle-worker-v2%40kaggle-161607.iam.gserviceaccount.com%2F20221230%2Fauto%2Fstorage%2Fgoog4_request&amp;X-Goog-Date=20221230T105820Z&amp;X-Goog-Expires=345600&amp;X-Goog-SignedHeaders=host&amp;X-Goog-Signature=0d568204f117448a8fc7c902e8094928d1af624e43cddcdcb86a8a51c12ca619058f7421eea009fac150ebab3532bc1503bd0a7c2670134c309b84365a0c7a0d038b826318df260ff32e10a226a9e075860f33a39277504dd77cbb433868071e4854ba826423e5f284b7a67e1ad2435d2706bca19d6f4b9ab67817a8617b2a98727368aae4a8617c91748b906b3a5a77174962ab196ea2b583aa8fe94e2b9fb1a58db415cd7f5abf6fd980f1810672c162771e331a7801c7b61d90665437b098eb38a2974d43cac99344b3a696a00e56a59b96db6919a9acb9458544bf00f8d5956a89f57858aba12355ccad06f33d8367372786ad1c90dca414318e32d9834b" alt="Healthy" width="240" height="167" /></td>
<td><img src="https://storage.googleapis.com/kagglesdsdata/datasets/1447507/2394131/Validation/Validation/Powdery/8f6737815b2cd234.jpg?X-Goog-Algorithm=GOOG4-RSA-SHA256&amp;X-Goog-Credential=databundle-worker-v2%40kaggle-161607.iam.gserviceaccount.com%2F20221230%2Fauto%2Fstorage%2Fgoog4_request&amp;X-Goog-Date=20221230T110139Z&amp;X-Goog-Expires=345600&amp;X-Goog-SignedHeaders=host&amp;X-Goog-Signature=37f5aeec6b32c9d36f8b89b8d3d5b9a102fbfe16c7c6f14cddd115bfd9d7c1abfcf1667f85d1a57dc71484360f18e584cbd49e0b6e84afe8b96a93f4096149d7b9c875822ad8fc76bae54cc08f745540ec15978e4c7183deb2a1326ad2290a7d798e56072ce7e0df84ea8c1598399a970e0e5976ed82647fdeab13791498c5ba206cf543196f24035ce4f16b657c753c99ce5eb8b4045b5cf0540f406472e6f7fe526dc05e74e105825662f32f3dcbc6fae70502eda612615d9dda0810e1e8301b5e29cf9cef3711ddfeed7e5a29c991e60e8470384ce8cdccfc7628da2803d2b8ab4048a061be08542c4b0c14cb913df999270130090228bd763872328a029b" alt="Powdery" width="240" height="167" /></td>
<td><img src="https://storage.googleapis.com/kagglesdsdata/datasets/1447507/2394131/Validation/Validation/Rust/920e33d67f8b01b3.jpg?X-Goog-Algorithm=GOOG4-RSA-SHA256&amp;X-Goog-Credential=databundle-worker-v2%40kaggle-161607.iam.gserviceaccount.com%2F20221230%2Fauto%2Fstorage%2Fgoog4_request&amp;X-Goog-Date=20221230T110231Z&amp;X-Goog-Expires=345600&amp;X-Goog-SignedHeaders=host&amp;X-Goog-Signature=59b6867e7a5531207948a39ca4524172a7030f918cfb99ea4b4177b12be088f7edc36d27077c61918ac6742c13044fee9d3c8942476597ab4b6e5e3b45faeb73e6ea0d4b31312a23dbc749a2263b7b0a38df6a04ca4a7eb0f7cb0a28743a989c45cc6c845a1c6ac4d6b96c7cc1c71e40820e25400baf3b4e8e710fe7a01d085500c26e067837f9684cea61be69d7388623e0af1ead5aa780464c98285f0965763ef3e75b1430b67ac564525afd2c7611a9bb8516af18493310ef7996449502ce593f7f78eb1518c782967e06cb7e6255da33e4d26fed84a585dbeef1e3f4d15737b5c8022a2e121281c19e72891bfc6d7876200866233196874c20aece419ca3" alt="Rust" width="240" height="167" /></td>
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
| [02 - Conjunto de Datos](https://colab.research.google.com/github/JLopez86/plant_disease/blob/main/01_Introduccion.ipynb)
| [03 - Redes Neuronales Convolucionales](https://colab.research.google.com/github/JLopez86/plant_disease/blob/main/01_Introduccion.ipynb)
| [04 - Transferencia de Aprendizaje](https://colab.research.google.com/github/JLopez86/plant_disease/blob/main/01_Introduccion.ipynb)
| [Conclusión](https://colab.research.google.com/github/JLopez86/plant_disease/blob/main/01_Introduccion.ipynb)
