# Machine-learning

En este repositorio se encuentran los links a los google colab donde desarrollé los proyectos de machine learning.


## Red Neuronal capaz de predecir la especie de un ave en base a su canto

Dado un dataset que contenía diferentes cantos de aves y su especie, entrené una red neuronal para que pueda distinguir las especies en base al canto. 

Lo primero que tuve que hacer fue transformar los audios a un formato de dato que la red neuronal pueda comprender.
Luego de investigar decidí que lo que mejor representaba a los audios eran los MFCC. Los MFCC (Mel Frequency Cepstral Coeﬃcients) son los coeﬁcientes para la representación del habla basados en la percepción auditiva humana.

Una vez convertidos los audios a MFCC, separé al dataset en train y test. Luego, entrené la red neuronal creada con keras con el dataset train y por último evalúe la red con el dataset de test obteniendo un los de 0.3318 y una accuracy de 0.9192.


**Link al colab de la red:** https://colab.research.google.com/drive/16G1rgort4CIEd8kfAvAh2-tWr5gr8Lb_?usp=sharing


## Modelo Random Forest capaz de predecir el fraude cometido en tarjetas de crédito:

Dado un dataset que contenía información sobre los fraudes cometidos con tarjeta de crédito, entrené un modelo Random Forest para predecir si una transacción realizada es un posible fraude.

Para comenzar tuve que seleccionar las features del dataset que usaría para entrenar mi modelo. Estas features fueron una mezcla entre las que consideré que eran más importantes y las obligatorias.  Además, para bajar las probabilidades de dejar una feature importante fuera del dataset decidí tomar algunas features de forma aleatoria.

El siguiente paso fue encondear las features no numéricas. Para esto utilicé 3 técnicas distintas de encoding: One hot encoding, CountVectorizer y Mean encoding.

Luego de encodear el dataset, este fue utilizado para entrenar al modelo. 

Finalmente, el modelo fue utilizado para predecir el resultado de un dataset de validación obteniendo 0.8184067598667024 puntos auc roc


**Link al colab de random forest:** https://colab.research.google.com/drive/1ZPoAiCQK-7pLubk8RK6rrLitpRgZNmW5?usp=sharing
