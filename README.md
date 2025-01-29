1) Título
    Proyecto LSA-alfabeto el proyecto consiste en generar un modelo de inteligencia artificial que detecta las señas que representan cada una de las letras del alfabeto proporcionado por el CAS(Confederación Argentina de Sordos).

2) Requisitos previos y Dependencias
   Se deben instalas las siguientes técnologias:
     * Pytorch
     * Pandas
     * Numpy
     * Matplotlib
    El entorno de desarrollo utlizado en el desarrollo del proyecto fue COLAB. en su versión gratuita.

3) Datos utilizados en el proyecto.

    El dataset utilizado para el entrenamiento y testeo del modelo fue un dataset personalizado el cual fue creado con una herramienta open source VGG Image Anottation: https://www.robots.ox.ac.uk/~vgg/software/via/ . Esta herramienta nos permitio generar las etiquetas en un formato JSON, las misma se generan en el formato COCO.

    Ya que no se poseia una cantidad considerable de muestras de datos se implemento una función augmentation para aumentar la cantidad de datos, y asi lograr entrenar y testear el modelo de forma correcta.

4) El modelo utilizado

    El modelo utilizado para el entrenamiento fue FasterRCNN50, ya que el mismo no es demasiado pesado para poder ejecutarlo en versión gratuita de COLAB y permite lograr un excelente desempeño en la tarea de detección de objetos.

5) Entrenamiento
   Durante el entrenamiento se evaluo el modelo utilizando el acurracy del testeo, para verificar que el mismo este aprendiendo correctamente.
   
