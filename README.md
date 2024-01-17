# PI_02_DA_Siniestros_Viales
Analisis de los Siniestros Viales en la ciudad de Buenos Aires

![Static Badge](https://img.shields.io/badge/PowerBI-gray?style=flat&logo=powerbi)
![Static Badge](https://img.shields.io/badge/Python-gray?style=flat&logo=python)
![Static Badge](https://img.shields.io/badge/-Pandas-gray?style=flat&logo=pandas)
![Static Badge](https://img.shields.io/badge/-Matplotlib-gray?style=flat&logo=matplotlib)
![Static Badge](https://img.shields.io/badge/-Seaborn-gray?style=flat&logo=seaborn)
![Static Badge](https://img.shields.io/badge/-Jupyter_Notebook-gray?style=flat&logo=jupyter)
![Static Badge](https://img.shields.io/badge/Visual_Studio_Code-gray?style=flat&logo=visual%20studio%20code&logoColor=blue)


Para la elaboración de este proyecto simulamos ser un `Data Analist`.

El principal objetivo es mediante el analisis de la información poder ofrecer estadisticas con KPI's claves del comportamiento de siniestros viales en la ciudad de Buenos Aires. Haciendo uso de la información suministrada en la pagina: [BA Data Buenos Aires](https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales)

## Desarrollo

Para este proyecto se trabajó con la **Bases de Víctimas Fatales en Siniestros Viales** que se encuentra en formato de Excel y contiene dos pestañas de datos:

 * **HECHOS**: que contiene una fila de hecho con id único y las variables asociadas temporales, espaciales y participantes.

 * **VICTIMAS**: contiene una fila por cada víctima de los hechos y las variables: edad, sexo y modo de desplazamiento. Se vincula a los HECHOS mediante el id del hecho.
   
En este [PDF](https://drive.google.com/file/d/1ct4Y5PpQ7XkSegjyclxKNoYIyKa7GILO/view?usp=drive_link) se detallan todas las definiciones manejadas en los datos y en el desarrollo de este proyecto.
En las siguientes imagenes se detalla el diccionario de datos de las pestañas `HECHOS` `VICTIMAS`

![Diccionario HECHOS](/Image/Diccionario_Hechos.png)

![Diccionario HECHOS](/Image/Diccionario_Victimas.png)


## Analisis del Data Set

### ETL

Se realiza la extracción y limpieza de datos, identidicando los campos necesarios para la elaboracíon del proyecto validando y unificando los tipos de datos y nombres de las columnas de las hojas `HECHOS` `VICTIMAS` . Se eliminan los datos Nulos y Duplicados para finalmente unificar ambas hojas en un solo Data Set llamado [siniestros_ok](/Data/siniestros_ok.csv)

### EDA

Se realiza un Análisis exploratorio de los datos reviando que tipos de variables y comportamiento de la información podemos llegar a evaluar [EDA](/EDA.ipynb) para poder crear la visualización en Poer BI









