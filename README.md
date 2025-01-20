1) Título
    El proyecto de computer vision consisten en un detector de letras del alfabeto LSA argentino, el antes mencionado es el alfabeto homologado por el CAS(confederación argentina de sordos)
2) Requisitos previos
   Se deben instalas las siguientes técnologias:
     * Pytorch
     * Pandas
     * Numpy
3) Estructura del proyecto
   3.1 El dataset utilizado para este proyecto fue creado por los integrantes del proyectos(Matias Guzmán y Gonzalo Maunas), en base a las señas proporcionadas por el alfabeto, cada uno repitio las mismas
       5 veces. Para realizar las anotaciones se utilizo la herramienta de Software libre VGG Image Annotator
   3.2 El modelo utilizado en el proyecto es FasterRCNN , ya que el mismo es un modelo lo suficientemente escueto para poder entrenarlo en COLAB
4) Entrenamiento
   Durante el entrenamiento se realizo la carga y el guardado de los pesos del modelo para poder optimizar los recursos del entorno de desarrollo. Para realizar la carga de los pesos se tuvo encuenta el accuracy
   de entrenamiento si el mismo resultaba ser mejor que "best_accuracy" se guardaban los nuevos pesos generados por el modelo.
