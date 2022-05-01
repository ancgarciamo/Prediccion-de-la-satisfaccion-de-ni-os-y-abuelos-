# Prediccion  de  la satisfaccion de niños y abuelos
Este trabajo toma pretende a partir de los datos obtenidos de la Encuesta de Calidad de Vida del DANE formular una aplicación que permita predecir la satisfacción de los niños y abuelos, para esto primero se hace un análisis descriptivo.

Como podemos ver en el siguiente grafico la edad por si misma no es un factor determinante para la satisfacción, sin embargo nos muestra que las personas menores de 15 años no responden la encuesta.

 
Para asignarle una satisfacción a las personas que no contestaron se obtuvo la probabilidad de las personas que si contestaron, y con una función aleatoria en proporción a esa probabilidad se asigno una satisfacción a las personas menores de 15 años ya que ahí se encuentra una de nuestras poblaciones objetivo.
Además a los niños se les clasificara siendo mayores de 3 años y menores de 13 años ya que desde los 4 años es que se desarrolla su yo propio , lo cual les permitiría responder la encuesta y hasta los 12 años , ya que esa es la edad antes de la adolescencia según el Instituto de bienestar familiar.

 
Para la población de abuelos se tomo en cuenta información de 2 articulos el cual uno exponía que la edad media del primer hijo es a los 22 años  y que el 40% de los hogares no tienen hijos ,así que tomamos 60% de los datos de las personas mayores de 44 años para la población de abuelos.

###Modelos
Para los modelos para predecir la satisfacción se escogieron con la excepción de Edad y Salud distintas variables para cada modelo
Para el modelo de los Abuelos
Se escogieron las variables  de:
-Edad
-Estado Civil 
-Sensacion de seguridad
-Condicion del Hogar
-Tenencia de bienes principales
-Tenencia de bienes Secundarios
-Salud
-Servicios Básicos

Para el modelo de los Niños
Se escogieron las variables
-Edad
--Ocupacion

-Sabe leer y escribir

-Uso de dispositivos electronicos diferentes al celular

-Uso de Internet

-Uso de Celular

-Numero de actividades de ocio en internet

-Numero de actividades de ocio en celulares

-Salud




### Aplicacion Web
En la siguiente aplicacion podra 
https://ancgarciamo.shinyapps.io/Prediccion_de_Satisfaccion/

### Bibliografia
- [Shiny](https://shiny.rstudio.com/)
- [Stack overflow](https://stackoverflow.com/)
