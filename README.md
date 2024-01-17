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

![Diccionario HECHOS](/image/Diccionario_Victimas.png)
