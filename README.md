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

Principalmente evaluamos la variable de victimas por siniestros por Año, Mes y dia concluyendo lo siguiente:

* Evidenciamos que el año com mas victimas fue el 2018 con 160 casos, mientras que el menor año es el 2020 tal vez por el confinamiento que hubo por el Covid_19
* Evidenciamos que el mes con mayor cantidad de victimas es Diciembre, tal vez influya que es mes de vacaciones y es cuando mas se movilizan las personas en sus vehiculos
* Evidenciamos que el dia del mes con mas victimas es el dia 20 con un total de 33 Victimas

![Victimas por Año](/Image/Cantidad_de_victimas_por_año.png)

![Victimas por Mes](/Image/Cantidad_de_victimas_por_mes.png)

![Victimas por Día](/Image/Cantidad_de_victimas_por_dia.png)

Luego evaluamos la edad promedio de las vistimas:

![Victimas por Año](/Image/Edad_promedio_victimas.png)

Finalmente la distribución de las victimas por genero, evidenciando que los hombres tienen un mayor % 

![Distribución de Victimas por Género](/Image/Distribución_de_victimas_por_genero.png)


## KPI's   :chart_with_downwards_trend:  :hourglass:  :eyes:

**Tablero de Control**

![DashBoard](/Image/DashBoard.png)

- *Reducir en un 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior*.
  
  Definimos a la **tasa de homicidios en siniestros viales** como el número de víctimas fatales en accidentes de tránsito por cada 100,000 habitantes en un área geográfica durante un período de tiempo específico.
  Su fórmula es: (Número de homicidios en siniestros viales / Población total) * 100,000

 ![Disminución 10% tasa de Homicidiosi](/Image/-10%_kpi.png)

  
- *Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior*.
  
  Definimos a la **cantidad de accidentes mortales de motociclistas en siniestros viales** como el número absoluto de accidentes fatales en los que estuvieron involucradas víctimas que viajaban en moto en un determinado periodo temporal.
  Su fórmula para medir la evolución de los accidentes mortales con víctimas en moto es: (Número de accidentes mortales con víctimas en moto en el año anterior - Número de accidentes mortales con víctimas en moto en el año actual) / (Número de accidentes mortales con víctimas en moto en el año anterior) * 100
  
 ![Disminución del 7% Accidentes en Motocicleta](/Image/-7%_kpi.png)

##### Concluciones Dash Board 🚧

Realizando el análisis total del dataset y creacion del DashBoar concluimos que dentro de la ciudad de Buenos Aires los siniestros en vehiculos desde el año 2016 al 2018 aumentaron pero del 2019 al 2021 han logrado disminuir, esto podria mejorar si se hicieran continuamente charlas de concientizacion a los conductoeres.










