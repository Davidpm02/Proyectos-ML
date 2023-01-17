# Proyectos-SAGEMAKER #
Este repositorio subire los principales proyectos que haré con AWS Sagemaker, explicando los detalles de cada uno.



## Modelo de prediccion de salario de emepleados ##
Se trata de un modelo de machine learning de aprendizaje supervisado.

### COMMIT-1 ###

Subo el cuaderno de Jupyter Notebook junto con el archivo csv que uso como datos de entrada y salida.

### COMMIT-2 ###

He avanzado en el cuaderno de Jupyter hasta la parte previa a la prueba del modelo con Sagemaker.

Para empezar, he importado todas las librerias necesarias, ademas de los datos que utilizaremos de entrada (archivo csv).
Acto seguido, ha hecho uso de la libreria matplotlip para poder visualizar los datos de entrada y salida del csv.

He hecho uso de pandas para crear un array correspondiente a la columna de las X del dataframe (datos de entrada y salida del csv), y otro array
correspondiente a la columna y del dataframe.
Tras esto, he hecho uso de la libreria sk-learn para separar el array anterior en datos de entrenamiento y testeo (X_train,X_test---y_train,y_test),
y mezclar los valores de los datos (no queremos que el modelo memorice ningun tipo de secuencia en los valores de entrenamiento).

   - Separamos los datos en datos de entrenamiento y testeo porque el modelo NO DEBE HABER VISTO ninguno de los datos de testeo al momento de entrenar.

Por ultimo, he utilixado de nuevo sk-learn para predecir los valores correspondientes a X_train, y ha predicho los valores que supuestamente encajarian 
en la columna de las y.

### COMMIT-3 ###

Despues de probar el rendimiento de nuestro modelo, es hora de entrenarlo. Para ello, los datos de entreda se deben pasar a un formato con el que Sagemaker pueda trabajar con ellos. Ademas, se han seteado los hiperparametros para el entrenamiento.

Al terminar el entrenamiento, el resultado se almacena en una nueva subcarpeta (output).








