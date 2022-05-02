# Prediccion  de  la satisfaccion de niños y abuelos
Este trabajo toma pretende a partir de los datos obtenidos de la Encuesta de Calidad de Vida del DANE formular una aplicación que permita predecir la satisfacción de los niños y abuelos, para esto primero se hace un análisis descriptivo.

Como podemos ver en el siguiente grafico la edad por si misma no es un factor determinante para la satisfacción, sin embargo nos muestra que las personas menores de 15 años no responden la encuesta.

![](https://github.com/ancgarciamo/Prediccion-de-la-satisfaccion-de-ni-os-y-abuelos-/blob/main/Imagenes/Satisfaccion%20y%20edad.PNG)
 
Para asignarle una satisfacción a las personas que no contestaron se obtuvo la probabilidad de las personas que si contestaron, y con una función aleatoria en proporción a esa probabilidad se asigno una satisfacción a las personas menores de 15 años ya que ahí se encuentra una de nuestras poblaciones objetivo.
Además a los niños se les clasificara siendo mayores de 3 años y menores de 13 años ya que desde los 4 años es que se desarrolla su yo propio , lo cual les permitiría responder la encuesta y hasta los 12 años , ya que esa es la edad antes de la adolescencia según el Instituto de bienestar familiar.

![](https://github.com/ancgarciamo/Prediccion-de-la-satisfaccion-de-ni-os-y-abuelos-/blob/main/Imagenes/probabilidad.PNG)

Para la población de abuelos se tomo en cuenta información de 2 articulos el cual uno exponía que la edad media del primer hijo es a los 22 años  y que el 40% de los hogares no tienen hijos ,así que tomamos 60% de los datos de las personas mayores de 44 años para la población de abuelos.

### Modelos
Para los modelos para predecir la satisfacción se escogieron con la excepción de Edad y Salud distintas variables para cada modelo
#### Para el modelo de los Abuelos
Se escogieron las variables  de:
- Edad
- Estado Civil 
- Sensacion de seguridad
- Condicion del Hogar
- Tenencia de bienes principales
- Tenencia de bienes Secundarios
- Salud
- Servicios Básicos

#### Para el modelo de los Niños
Se escogieron las variables
- Edad
- Ocupacion
- Sabe leer y escribir
- Uso de dispositivos electronicos diferentes al celular
- Uso de Internet
- Uso de Celular
- Numero de actividades de ocio en internet
- Numero de actividades de ocio en celulares
- Salud

Para los abuelos se tomo variables simples como el estado civil , como se siente de salud, sensacion de seguridad ,los servicios basicos que posee, cuantos bienes posee en el hogar , separandolos por bienes fundamentales y bienes menos necesarios.

Para los niños se tomo en que se ocupan , si saben leer o escribir , el uso de dispositivos electronicos separados por el celular y los demas , ademas de las actividades de ocio en internet y en un celular.

Las variables se unen en una sola base de datos , una para cada modelo y a estas se les aplica el metodo de los vecinos mas cercanos.
Con una aplicacion en RShiny se montan los modelos y se ejecutan en una interfaz.
### Resultados 
Con los modelos montados , en la interfaz podemos ver como de acuerdo a las opciones que se escojan , la aplicacion intenta predecir la satisfaccion del usuario.

![](https://github.com/ancgarciamo/Prediccion-de-la-satisfaccion-de-ni-os-y-abuelos-/blob/main/Imagenes/aplicacion.PNG)

### Video Promocional
El video se podra ver en la siguiente direccion:



### Aplicacion Web
En la siguiente aplicacion podra consultar en la siguiente direccion:
https://ancgarciamo.shinyapps.io/Prediccion_de_Satisfaccion/

### Bibliografia
- [Shiny](https://shiny.rstudio.com/)
- [Stack overflow](https://stackoverflow.com/)
- https://www.icbf.gov.co/cargues/avance/docs/concepto_icbf_0027891_2010.htm
- https://www.ceupe.com/blog/etapas-de-desarrollo-de-la-conciencia.html
- https://www.eugin.com.co/eugin-presenta-la-primera-encuesta-internacional-sobre-fertilidad-edad-para-tener-hijos-donacion-de-ovulos/
- https://www.eltiempo.com/vida/educacion/crece-tendencia-de-parejas-jovenes-a-no-tener-hijos-465196
- https://faros.hsjdbcn.org/es/articulo/beneficios-tiempo-ocio-desarrollo-infantil
- https://www.publico.es/psicologia-y-mente/biblioterapia-leer-nos-hace-mas-felices/
