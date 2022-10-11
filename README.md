# Project_modulo3.Francisco-Villalobos-


EDA📌

Unificamos todos los Data Set de los diamantes hasta conseguir tener el dataset con todas las features a tener en cuenta para el precio del diamanta.

Una vez unificados estos Data Set, procedemos a realizar el Eda, donde observamos que las features más relacionadas con el precio son las features X, Y e Z, teniendo en cuenta esto, multiplicamos estas features y nos da el volumen del diamante. 

El precio del diamante tiene relacación con el volumen, por lo tanto, cuanto más caro es el diamante, es porque su tamaño es mayor.

Las otras features que encontramos en el Data set, tienen menos incidencia sobre el precio del diamante, estas features son: la ciudad, el color, la claridad, y el corte.


Best Model 💻

Predicciones_Model_1

El mejor RMSE en Kaggle: 568,131 / Notebook: 597,081
Descripción del modelo:

Paso 1: Creamos la nueva vfeature Volumen, multiplicado las features relacionadas con el tamaño.

Paso 2: Separamos el precio del resto de features.

Paso 3: Separamos las features, "carat	depth	table	x	y	z	total"

Paso 4: Escalamos las features numéricas utilizando el StandardScaler, y lo pasamos de nuevo a Dataframe.

Paso 5: Convertirmos las features cualitativas a numericas para posteriormente escalarlas de nuevo con el StandardScaler.

Paso 5: Convertirmos las features cualitativas a numericas para ello, le damos peso o valores a estas features. Posteriormente las escalamos con StandardScaler.

Paso 6: Una vez que tenemos nuestros Dataframes los unimos con un merge y entrenamos el modelo sobre ese Dataframe.

Paso 7: Para entrenarlo aplicamos al Dataframe el train_test_split para poder poder trabajar con el X_train y aplicarlo a X_test.

Paso 8: Aplicamos el RandomForestRegressor, el modelo que mejor RMSE nos ha dado. Para los parámetros hemos utilizado parámtros tipo.

Paso 9: Posteriormente aplicamos el mismo trabajo el al dataset para el que queremos predecir.


Predicciones_Model_2


El mejor RMSE en notebook: 571,44/Kaggle: 568,42

Descripción del modelo:



Paso 1: Creamos la nueva vfeature Volumen, multiplicado las features relacionadas con el tamaño.

Paso 2: Separamos el precio del resto de features.

Paso 3: Escalamos las variables númericas, con StandardScaler.

Paso 2: Convertimos las variables categóricas a numéricas, utilizando LabelEncoder()

Paso 3: Escalamos las variables una vez convertidas a numéricas

Paso 6: Una vez que tenemos nuestros Dataframes los unimos con un merge y entrenamos el modelo sobre ese Dataframe.

Paso 7: Para entrenarlo aplicamos al Dataframe el train_test_split para poder poder trabajar con el X_train y aplicarlo a X_test.

Paso 8: Aplicamos el RandomForestRegressor, el modelo que mejor RMSE nos ha dado. Para los parámetros hemos utilizado parámtros tipo.

Paso 9: Posteriormente aplicamos el mismo trabajo el al dataset para el que queremos predecir.



Analysis ✒️


Despues de la realización de multiples anális, que cuanto más datos mejor, es decir, el modelo aprende las features y de este modo puede predecir mejor los precios de los diamantes en función de dichas features. 


Entrenando el modelo con diferentes métodos como: (linear-regression, Random_forest, Catboosting)
He elegido el andmForest nos da el RMSE más bajo, y la preddición se ajusta más a nuestra necesidad debido a nuestras features.



Librery 📚

import numpy as np
import pandas as pd
from sklearn.preprocessing import RobustScaler, StandardScaler
from sklearn.preprocessing import OneHotEncoder, OrdinalEncoder
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.linear_model import LinearRegression
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import roc_auc_score
from sklearn.preprocessing import LabelEncoder
from sklearn.metrics import mean_squared_error
from sklearn.preprocessing import MinMaxScaler
from sklearn.ensemble import RandomForestClassifier
from sklearn.ensemble import RandomForestRegressor


Folder structure 💾
└── PROJECT_M3
    ├──Predicciones_Model_1
    ├──Predicciones_Model_1
    ├──DataSet
    ├── Link.txt
    ├── README.md
    ├── .ipynb_checkpoints
    ├── .DS_Store


Contact info  💌 

    ├── Email: fco.villalobos.perez@gmail.com
    ├── Móvil: 659.895.049

![image](https://user-images.githubusercontent.com/102686594/194706870-bcc596f0-b06f-40ca-9931-01b5ee0b8cbb.png)

