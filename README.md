![banner_tipster](https://github.com/cistelsa/Commerce_Data_Analysis_and_Recommendations/assets/17438992/5972fc1a-725d-43b7-9d7b-6cd76f0ad165)


# <h1 align=center> **COMMERCE DATA ALALYSIS AND RECOMMENDATIONS** <img src="5_Sources/Images/Icono_tipster_green.png" width="50px"/></h1>

## Tipster ![marca-version](https://img.shields.io/badge/Versi%C3%B3n-1.0.2-bluegreen?style=for-the-badge&logo=googlehome)
![marca-licencia](https://img.shields.io/badge/Licencia-MIT-green?style=for-the-badge&logo=apachespark)
![marca-lenguaje](https://img.shields.io/badge/Python-v3.10.10-yellowgreen?style=for-the-badge&logo=python)
![marca-status](https://img.shields.io/badge/Status-Project%20Advances%20Indefinitely-orangegreen?style=for-the-badge&logo=apachehadoop)
![marca-status](https://img.shields.io/badge/Authors-5-blue?style=for-the-badge&logo=azurepipelines)

-----

# <font color='#307A71'>**Tabla de Contenido**</font>

- [El Repositorio](#el-repositorio)
- [Autores](#autores)
- [Introducción](#introducción)
- [Entendimiento de la Situación Actual del Sector](#entendimiento-de-la-situación-actual-del-sector)
- [Alcance](#alcance)
- [Objetivos y Key Performance Indicators - KPI's](#objetivos-y-key-performance-indicators---kpis)
- [Stack Tecnologico - Pipeline](#stack-tecnológico---pipeline)
- [Metodología de Trabajo](#stack-tecnológico---pipeline)
- [Datos](#datos)
- [Modelo de Recomendación](#modelo-de-recomendacion)
-----


-----
# <font color='#307A71'>**El Repositorio**<a name="repo"></a></font>

En el repositorio se encuentran los siguientes archivos:

| **`Carpeta Principal`** | **`Subcarpeta`** | **`Descripción`** | **`Link`** |
|-------------------------|------------------|-------------------|------------|
|1_ETL                    |                  |Esta carpeta contiene los primeros archivos de ETL realizados al inicio del proyecto y los ETL de Normalización de Tablas producto de la automatización en Microsoft Fabric. |[1_ETL](1_ETL)    |
|1_ETL                    |APIs              |Subcarpeta con la API utilizada para la extracción de información HotelBeds.                |                  |
|2_Datasets               |                  |Carpeta raiz con los Datasets del proyecto.|[2_Datasets](2_Datasets)      |
|2_Datasets               |beta              |Subcarpeta con los Datasets en formato ".csv" originados luego del primer ETL aplicado.      |                  |
|2_Datasets               |launch            |Subcarpeta con los Datasets en formato ".csv" y ".zip" originados luego del proceso de "EDA" - Análisis Exploratorio de Datos.|                 |
|3_EDA                    |                  |Carpeta que contiene los notebooks con los "EDA" - Análisis Exploratorio de Datos, de los datasets de la empresa.|[3_EDA](3_EDA)           |
|4_Model_ML               |                  |Carpeta con los Notebooks de los Modelos de Machine Learning aplicados al proyecto.    |[4_Model_ML](4_Model_ML)                  |
|5_Sources                |                  |Carpeta de recursos web.|[5_Sources](5_Sources)       |
|5_Sources                |Images            |Subarpeta con las imágenes utilizadas en los archivos .md, .ipynb, web.|  |
|5_Sources                |Videos            |Subcarpeta con los videos utilizados en los archivos .md, .ipynb, web.|     |
|6_Documentation          |                  |Esta carpeta principal contiene información sobre material de apoyo o complementario necesario para el desarrollo del proyecto.|[6_Documentation](6_Documentation)            |
|6_Documentation          |Dictionaries      |Contiene los diccionarios de los Modelos de Entidad Relación de las Bases de Datos.|                   |
|6_Documentation          |KPI               |Contiene información sobre los KPI propuestos para el proyecto.|       |
|6_Documentation          |Presentations_Sprint|Contiene las presentaciones realizadas por cada sprint de avance entregado.|  |
|7_Dashboard              |                  |En esta carpeta se encuentra el Dashboard con las métricas de los KPI propuestos.|[7_Dashboard](7_Dashboard)              |
|8_Public                 |                  |Esta carpeta contiene los archivos para el deployment.|[8_Public](8_Public)|
|8_Public                 |static            |Información fija para fastapi, jinja2, uvicorn.       |       |
|8_Public                 |templates         |Plantilla para fastapi, jinja2, uvicorn.              |       |

-----


-----
# <font color='#307A71'>**Autores** <a name="autores"></a></font>

# <h1 align=center> <img src="5_Sources/Images/equipo.png" width="900px"/></h1>


|Nombre               | Rol                     | Correo                     | GitHub                                          | Linkedin|
|---------------------|-------------------------|----------------------------|-------------------------------------------------|---------|
|Leydy Lucena Peñaloza Rojas |Technical Project Managet, Data Engineer, Data Scientist |leydy.penaloza@gmail.com    |[leydypenaloza](https://github.com/leydypenaloza)    |[leydy-penaloza](www.linkedin.com/in/leydy-penaloza)|
|Edisson Camilo Ortiz López  |Data Analyst, Data Engineer, Visual Designer |eortiz@cistelsa.com   |[cistelsa](https://github.com/cistelsa)            |[camilo-ortiz-cistelsa](https://www.linkedin.com/in/camilo-ortiz-cistelsa)|
|Aldemar Bohorquez Rodriguez |Data Engineer, Data Scientist, Machine Learning Engineer|abr942010@gmail.com   |[aldemarbr94](https://github.com/aldemarbr94)            |[aldemar-bohorquez-rodriguez](https://www.linkedin.com/in/aldemar-bohorquez-rodriguez/)|
|Mayren Gabriela Silva Basto |Data Analyst, Data Engineer, Machine Learning Engineer  |mayrensilva95@gmail.com     |[MayrenS95](https://github.com/MayrenS95)        |[mayren-gabriela-silva-basto](https://www.linkedin.com/in/mayren-gabriela-silva-basto-67b645181/)|
|Yesica Milagros Leon Ccahuana |Data Analyst, Data Engineer, Data Scientist|agrostopo@gmail.com|[yesicamilagros](https://github.com/yesicamilagros)|[yesica-leon-ccahuana](https://www.linkedin.com/in/yesica-leon-ccahuana-1706a7216/)|

-----

-----
# <font color='#307A71'>**Introducción**<a name="introduccion"></a></font>


Como consultores de datos, centrados en el análisis del mercado del turismo estadounidense, presentamos a continuación el desarrollo de este proyecto. Nuestra misión es proporcionar a los clientes finales herramientas que les permitan mejorar sus campañas de marketing, tomar decisiones informadas sobre inversiones y ofrecer recomendaciones basadas en experiencias previas para sus usuarios.

El mercado del turismo en Estados Unidos es dinámico y competitivo. Nuestro proyecto aborda la necesidad de comprender mejor este mercado y aprovechar sus oportunidades; con este objetivo en mente, hemos desarrollado un conjunto de herramientas y análisis que ayudarán a nuestros clientes a optimizar sus estrategias.

En este repositorio, encontrará detalles sobre nuestra metodología, análisis de datos, modelos de machine learning y visualizaciones que respaldan nuestras recomendaciones. Esperamos que este proyecto brinde claridad y valor a nuestros clientes, mejorando la toma de decisiones y las experiencias de sus usuarios en el mercado del turismo norteamericano.

# <h1 align=center><img src="5_Sources/Images/pipeline_storytelling.gif" width="500px"/></h1>
-----

-----
# <font color='#307A71'>**Entendimiento de la Situación Actual del Sector**<a name="entendimiento"></a></font>

En la actualidad la opinión de los usuarios se ha convertido en un insumo importante para la toma de decisiones en las organizaciones. Sin importar el tamaño de las mismas, la experiencia que proporciona un producto y/o servicio se ha venido transformando con el paso del tiempo y el uso de las tecnologías, pues estas permiten el estar más interconectados, indistintamente del lugar en el que nos encontremos.

“El 52% de los usuarios a nivel global creen que las empresas deben tomar acciones para mejorar a partir del feedback de sus clientes”, según Microsoft. Las empresas son conscientes de lo anterior y del nivel de afectación que conlleva la facilidad con la que hoy día los usuarios comunican sus experiencias y como esto influye en las decisiones de posibles clientes, permitiendo el reaccionar, transformarse, anticiparse a diversas acciones del usuario, incluso fidelizar al mismo.

Por tanto, existen plataformas en la web que permiten recopilar esta información, como Yelp, que es una plataforma de reseñas de todo tipo de negocios, restaurantes, hoteles, servicios entre otros. Los usuarios utilizan el servicio y luego suben su reseña según la experiencia que han recibido; asimismo, Google posee una plataforma de reseñas de todo tipo de negocios, restaurantes, hoteles, servicios, entre otros integrada en su servicio de localización y mapas, Google Maps.

Sin embargo, toda esta información no es de utilidad sin el procesamiento y manejo adecuado, por ello, gracias al avance de la ciencia enfocada en el análisis de datos, se pueden usar herramientas que permiten identificar el estado actual, tendencias, pronósticos y supuestos en diversos escenarios, para finalmente tomar las decisiones pertinentes que permitan aumentar la satisfacción del cliente, posicionar la marca y utilidad de la organización.

-----

-----
# <font color='#307A71'>**Alcance**<a name="objetivos"></a></font>

* Se seleccionarán otras plataformas de información, además de Yelp y Google Maps, que contengan información pertinente y permitan complementar el proceso de ETL y EDA.
* Se usarán diversas herramientas tecnológicas, como Micfrosoft Fabric, para llevar a cabo el proceso de ETL y EDA.
* Se facilitará un dashboard y un sistema de recomendaciones del negocio a través de una API o aplicación.
-----

-----
# <font color='#307A71'>**Objetivos y Key Performance Indicators - KPI's**<a name="kpi"></a></font>

## **_♦Objetivo No 1:_**

Orientar nuestros esfuerzos hacia la mejora continua de la satisfacción del cliente en todos los aspectos de cada negocio; respaldada por la evaluación regular de indicadores clave como el Net Promoter Score (NPS) de los negocios por Estados y el Índice de Satisfacción del Cliente por negocio, con el propósito de fomentar relaciones a largo plazo y promover recomendaciones positivas.

<img src="5_Sources/Images/Objetivo_1.png" width="900px"/>

## **_♦Objetivo No 2:_**

Formular estrategias que promuevan un crecimiento sostenible y una expansión efectiva de la empresa, con un enfoque en el aumento constante de la Tasa de Retención de Clientes por Negocio y el comportamiento de la cantidad de clientes a los cuáles se les brinda el servicio, por negocio.

<img src="5_Sources/Images/Objetivo_2.png" width="900px"/>

## **_♦Objetivo No 3:_**

Optimizar la calidad y seguridad de servicios de nuestros clientes, garantizando información oportuna que les permita identificar cuando más del 30% de las observaciones sean negativas; y la calificación promedio de Salubridad y Seguridad de los Hoteles sea 3.5 o más.

<img src="5_Sources/Images/Objetivo_3.png" width="900px"/>


--------
# <font color='#307A71'>**Stack Tecnológico - Pipeline**<a name="pipeline"></a></font>

Son diversas herramientas las cuales nos van a ayudar a cumplir nuestros objetivos a nivel Técnico y Profesional, a continuación se detallan de la mejor forma:

<img src="5_Sources/Images/logo_fabric.png" width="25px"/><font color='##74A608'>**Microsoft Fabric:**</font> Es un todo en uno de data, se integran todas las herramientas para ETL, EDA y DA.
Se propuso esta herramienta con el fin de adelantarnos a la tendencia, ya que se encuentra en fase Beta y pronto saldrá la versión Oficial, viniendo de Microsoft y la inversión que ha realizado los ultimos años en herramientas de data posicionandose en segundo lugar, tendremos la mejor experiencia en un entorno muy Profesional y nos ayudará para futuros proyectos en diferentes empresas.

<img src="5_Sources/Images/python.png" width="30px"/><font color='##74A608'>**Phyton:**</font> Python es un lenguaje de programación versátil ampliamente utilizado en ciencia de datos. Con bibliotecas como Pandas y NumPy, permite el análisis y manipulación de datos. Su flexibilidad lo hace ideal para automatizar tareas, trabajar con SQL y conectarse a herramientas como Apache Spark Data Factory en este proyecto.

<img src="5_Sources/Images/logo_spark.jpeg" width="30px"/><font color='##74A608'>**Apache Spark:**</font> Hadoop y Spark nos ayuda para el procesamiento de grandes cantidades de datos en forma de nodos, paralelizando el trabajo y siendo más eficiente de acuerdo su configuración y el tipo de archivo que se use, lo podremos gestionar con Python o con SQL.

<img src="5_Sources/Images/logo_scikit.png" width="30px"/><font color='##74A608'>**Scikit Learn:**</font> Lo usaremos para crear nuestros modelos de ML, también con una herramienta "Experiment" la cual realizamos un seguimiento del desarrollo a los modelos de ML y validar las hipotesis.

<img src="5_Sources/Images/logo_powerbi.png" width="50px"/><font color='##74A608'>**Power Bi:**</font> Aprovecharemos esta herramienta para realizar, el analisis y la vizualización de datos creando un Dashboard muy profesional y en la web.

<img src="5_Sources/Images/logo_matplotlib.png" width="30px"/><font color='##74A608'>**MatPlotlib:**</font> Es indispensable para crear el mejor informe EDA para que nuestros clientes puedan acceder a él de la forma más legible e intuitivo, será necesario traer nuestros modelos de ML allí y exponerlos.

<img src="5_Sources/Images/logo_kusto.png" width="30px"/><font color='##74A608'>**Kusto (KQL):**</font> Muy posiblemente usaremos streaming de datos, no es algo seguro pero lo proponemos desde el inicio.

<img src="5_Sources/Images/logo_azure.png" width="30px"/><font color='##74A608'>**Microsoft Azure:**</font> Usaremos la nube de Microsoft para apoyarnos respecto a Bases de datos de SQL Server de ser necesarias, también para realizar el deploy de la aplicación para nuestros clientes a través de Fast API, usando Docker.

## **_♦ Pipeline_**

El diagrama de Pipeline tecnológico se encuentra a continuación:

<img src="5_Sources/Images/pipeline.gif" width="900px"/>

[def]: #stack-tecnológico---pipeline


Nuestra Aplicación ofrece a los clientes información precisa respecto a:

1. **Recomendaciones de ubicación para nuevos Hoteles:** hacemos uso de análisis de datos y modelos de machine learning para identificar las ubicaciones óptimas para nuevos hoteles de su cadena, considerando variables como la densidad de población, el turismo, la afluencia de viajeros, eventos locales y los precios de la propiedad raíz, maximizando así su éxito en el mercado.

2. **Recomendaciones para segmentación de Anuncios en Google y Redes Sociales:** Utilizamos análisis de datos y modelos de machine learning para recomendar estrategias de segmentación y palabras clave altamente efectivas en Google y redes sociales, considerando la demografía, el turismo, los viajeros y los eventos locales de ubicaciones específica, optimizando así su presencia en línea y aumentando la conversión.

3. **Outsourcig Logístico:** identificamos áreas de mejora a partir de opiniones y calificaciones negativas, impulsando una experiencia de hospedaje más satisfactoria.

Respecto a lo desarrollado definimos unos limites y lo que no podemos hacer, no podemos ofrecer el servicio al 100% del gremio ya que si son cadenas de Hoteles nuevas no tenemos un histórico de data para ofrecer el servicio.

https://github.com/cistelsa/Commerce_Data_Analysis_and_Recommendations/assets/17438992/fce4aa00-97e7-410e-b641-de1286028069

 *Musica de fondo creada por inteligencia artificial - [https://soundful.com/](https://soundful.com/)*
