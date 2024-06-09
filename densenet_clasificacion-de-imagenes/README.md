# DenseNet

El código proporcionado realiza el reconocimiento de objetos en imágenes utilizando la red neuronal convolucional (CNN) DenseNet-201 pre-entrenada en el conjunto de datos ImageNet. A continuación, se describe brevemente cada parte del código:

1. **Instalación de Dependencias**: 
   - Se instalan las bibliotecas necesarias, incluyendo PyTorch, torchvision y Ultralytics, que son utilizadas para cargar y ejecutar el modelo YOLO (You Only Look Once) para detección de objetos.

2. **Carga de Imágenes**:
   - Se cargan seis imágenes de archivos en formato JPEG y se almacenan en las variables `img1`, `img2`, `img3`, `img4`, `img5`, y `img6`.

3. **Conversión a RGB**:
   - Las imágenes cargadas en formato BGR se convierten a formato RGB utilizando OpenCV para su visualización adecuada.

4. **Visualización de Imágenes**:
   - Se muestran las imágenes cargadas en una cuadrícula de subtramas utilizando Matplotlib para su visualización.

5. **Carga del Modelo DenseNet**:
   - Se carga el modelo DenseNet-201 pre-entrenado utilizando OpenCV y el framework Caffe. Se cargan tanto los archivos del modelo (`DenseNet_201.caffemodel`) como el archivo de configuración (`DenseNet_201.prototxt`).

6. **Definición de Función Clasificadora**:
   - Se define la función `Clasificador_denset` que toma una imagen y la imagen en formato RGB como entrada, y realiza la clasificación utilizando el modelo DenseNet cargado. La función devuelve la imagen RGB con la etiqueta de clase y la puntuación máxima superpuestas.

7. **Clasificación y Visualización**:
   - Se clasifican las imágenes 1, 2, 3 y 4 utilizando la función `Clasificador_denset`, y se muestra cada imagen clasificada utilizando Matplotlib.
