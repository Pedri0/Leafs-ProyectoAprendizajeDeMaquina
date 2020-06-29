# Leafs-ProyectoAprendizajeDeMaquina
 Proyecto de Clasificación de hojas suecas para la clase de Aprendizaje de Maquina

 Instrucciones:
 Debido a que los archivos de las imagenes provistas por la universidad Linkoping y las imagenes generadas tienen un peso mayor a 3 Gb no fue posible subirlas al Github. Sin embargo aqui proveo los links a google drive donde subi las imagenes.


 Imagenes  Originales (propiedad de linkoping U) (carpeta data): 

 Imagenes segmentadas en escala de gris (carpeta mascaras):
 
 Imagenes binarias (carpeta binarios):

 Imagenes de la clasificacion Online (carpeta validacion): 

Todas las carpetas (con el nombre como esta descrito) deben encontrarse en la misma ubicacion que las libretas de jupyter 

 El orden de ejecucion es como sigue:
 1 LeafsDoMasks (requiere de las imagenes originales, es decir la carpeta data)
 2 LeafsGetData (requiere de las imagenes segmentadas y binarias)
 3 SVM (requiere de los archivos .csv de Train y Test)
 4 OnlineClassification (requiere de las imagenes segmentadas y binarias)

 Los archivos .csv que se adjuntan en este git vienen por pares una para el conjunto de entrenamiento y otra para prueba.
Para prueba el archivo se llama texturaTestXyX.csv donde X X es un numero y representa la cantidad empleada de superpixeles por imagen. En el reporte .pdf se utiliza texturaTest10y10.csv ya que este valor fue el optimo en cuanto a recursos temporales
Para entrenamiento el archivo se llama texturaTrainXyX.csv donde X X es un numero y representa la cantidad empleada de superpixeles por imagen. En el reporte .pdf se utiliza texturaTrain10y10.csv ya que este valor fue el optimo en cuanto a recursos temporales

Requerimientos obligatorios:
Se encontro que para el calculo de superpixeles en un region de interes y no sobre toda la imagen se requiere instalar scikit-image en su version 0.17.2 o superior. Si no se cumple este requerimiento esta funcion truena.
