# DATATHON ENTEL 2022 - Reto1
##  MODELO PREDICTIVO DE RENOVACIÓN DE EQUIPOS MÓVILES
------------
#### Nombre del grupo: Coinflip
#### Integrantes:
-  Jamil Jafet Moreno Grimaldo (líder)
-  Alberto De la Cruz Trauco
-  Cesar Antonio Junior Gonzales Montes 

------------
## Instalación
1. Instalar [XGBoost](https://xgboost.readthedocs.io/en/latest/install.html "XGBoost") y [H2O](https://docs.h2o.ai/h2o/latest-stable/h2o-docs/downloading.html "H2O")
```python
!pip install h2o
!pip install xgboost==1.2.0
```
1. Previamente instalar y actualizar java para usar H2O
```python
!apt-get install openjdk-8-jdk --yes
!apt-get update
```
1. Se usaran las siguientes librerias:
	1. Imblearn
	1. Sklearn
	1. Pandas
	1. Numpy
	1. Datetime

## Ejecución
1.  Ejecutar el notebook `preprocesamiento.ipynb` 
Este scrip importa el conjunto de datasets (8 archivos csv), genera un preprocesamiento para cada archivo y luego los une en un DataFrame y los guarda en un csv `dataprefinal.csv`.

2. Ejecutar el notebook `procesamiento.ipynb` 
Este scrip hace un procesamiento al DataFrame final, además de entrenar y validar mediante un XGBoost a nuestros datos para luego exportarnos un archivo csv en un formato listo para subir a Kaggle.

## Referencias
1.  Algoritmo  [XGBoost](https://github.com/PacktPublishing/Hands-On-Gradient-Boosting-with-XGBoost-and-Scikit-learn "XGBoost") y [documentación](https://xgboost.readthedocs.io/en/stable/ "documentación").
1. Algoritmo [H2O](https://docs.h2o.ai/h2o/latest-stable/h2o-docs/welcome.html "H2O").
