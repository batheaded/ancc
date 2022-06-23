# Informe del Proyecto

Análisis de desnudos en el cine cubano, como evaluación de la asignatura de Aprendizaje de Máquina y Periodismo de Datos. Se apunta a lograr un trabajo para mostrar y contextualizar el uso del desnudo en el cine cubano, usando modelos de detección de desnudos.

## Introducción  

Se realizó una evaluación del estado del arte para llevar a cabo la detección desnudos y luego detección de rostros y la similitud de rostros.

Para evaluar el estado del arte se utilizaron las herramientas [Papers With Code](https://paperswithcode.com/) y [Google Scholar](https://scholar.google.com/).

Para la detección de rostros y la similitud de rostros se utilizó la biblioteca [Deepface](https://github.com/serengil/deepface).

En detección de rostros:

- [OpenCV](https://github.com/opencv/opencv)
- [RetinaFace](https://github.com/serengil/retinaface)

En similitud de rostros:

- [VGG-Face](https://www.robots.ox.ac.uk/~vgg/software/vgg_face/)

## Preparación

Partiendo de archivos de videos de filmes, se preparan los datos para comenzar a procesarlos y adaptarlos a la entrada del modelo. Utilizando el módulo ```VideoCapture``` de ```openCV```, teniendo la captura del video podemos quedarnos con cada uno de los frames, pero para facilitar el trabajo nos quedamos con un solo frame por cada segundo de duración del filme.

## Modelos

### OpenCV

OpenCV (Open Source Computer Vision Library) es una biblioteca open source de Machine Learning y Computer Vision. OpenCV se creó para proporcionar una infraestructura común para las aplicaciones de visión por computadora. Esta bajo una licencia BSD, lo que hace que OpenCV facilite que las empresas y organizaciones utilicen y modifiquen el código.

### RetinaFace

RetinaFace es un modelo de detección de rostro de vanguardia basado en deep learning para Python que viene con puntos de referencia faciales. Su rendimiento de detección es sorprendente y sobre salta en imágenes con varias personas, incluso entre la multitud.

### VGG-Face

VGG-Face esta basado en el aprendizaje de extremo a extremo (end-to-end) utilizando una red neuronal convolucional (CNN) y en la disponibilidad de conjuntos de datos de entrenamiento a gran escala.