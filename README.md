# Analisis de retención de usuarios de un gimnasio

Uno de los problemas más comunes que enfrentan los gimnasios es la perdida de clientes, así que en este proyecto analizo el comportamiento de los usuarios, mediante los datos analiticos presentados, busco predecir la perdida de usuarios del siguiente mes, utilizando machine learning para un caso de clasificación binaria, donde pruebo dos métodos 1) Regresión logistica y 2) bosque aleatorio, evaluando sus resultados y tomando la decisión de cual utilizar. 
A su vez, creo cluster para clasificar a los usuarios de acuerdo a su comportamiento y posteriormente calcular la tasa de cancelación de cada una de los clusters, obteniendo como resultado un perfil de usuario objetivo que suele cancelar su suscripción el proximo mes.

## Herramientas y tipo de proyecto

![Static Badge](https://img.shields.io/badge/sklearn-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/pandas-blue?style=for-the-badge&logo=pandas)
 | ![Static Badge](https://img.shields.io/badge/matplotlib.pyplot-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/seaborn-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/machine%20learning-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/clustering-blue?style=for-the-badge)
 | ![Static Badge](https://img.shields.io/badge/ETL-blue?style=for-the-badge)| 

## Metodología
**Preprocesamiento de datos:**   
Se estandarizaron los nombres de las columnas, se verificaron y limpiaron los valores ausentes y duplicados.

**Analisis Exploratorio de datos (EDA):**  
- Se analizaron los patrones de los usuarios que cancelaron y los que permanecen.
- Se realizo un mapa de calor para definir las caracteristicas con mayor colerración para los usuarios que cancelaron.

**Modelado predictivo:**  
Para predecir la cancelación de los usuarios del proximo mes, se entrearon dos modelos, regresión logística y bosque aleatorio. y se evaluaron para elegir el mejor modelo. Obteniendo una presición de 85% y 84% respectivamente  

**Clustering:**  
Se crea una matriz de distancias para obtener el valor de grupos para k-means y generar nuestros grupos de segmentación.

## Preguntas clave
-¿Cuál es la probabilidad de perdida (para el próximo mes) para cada cliente?  
-¿Cual es el perfil de usuarios que suele cancelar?  
-¿Que factores impactan la pérdida?   

## Conclusiones y recomendaciones

Al crear grupos mediante clúster logramos obtener grupos interesantes, tomando como punto de partida el grupo con mayor tasa de cancelación, obtuvimos que el grupo 2 que representa el 20.5% de la población total posicionándose como el segundo grupo más grande, lo cual representa una gran oportunidad, el análisis arrojo que el 100% de los usuarios del grupo 2 se encuentran cerca de las instalaciones, el 67.6% no cuenta con un partner y el rango de edad va de los 25 a 30 años, por lo que se puede ofrecer descuentos a esos usuarios dentro de ese rango de edad, en los horarios de menos flujo de personas, así mejorando nuestra ocupación de las instalaciones y incrementando la retención de usuarios de este grupo. Se sugiere realizar un estudio A/B, donde el grupo B sea un grupo seleccionado de los usuarios de este clúster y probando la estrategia de retención de los usuarios mencionada anteriormente. Esto se puede llevar a cabo mediante una campaña de marketing por mensajes de texto, ya que se cuenta con el 90% de los números de teléfono de los usuarios. 

Propuestas:
- Campañas de marketing por telefono: El 90% de los usuarios proporcionaron su número para contacto, conviritiendose en un excelente canal de comunicación.
- Realizar una prueba A/B con una campaña personalizada para usuarios de 25 a 30 años con promoción en horarios con menos flujo para incrementar la retención y el uso de las instalaciones.
- Fomentar las actividades grupales en los usuarios más jovenes ya que los usuarios que participan en estas actividades suelen renovar su suscripción.


