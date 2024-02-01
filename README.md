<center><h1>IBM SkillsBuild Europa - Análisis de datos</h1></center>
Requisitos

* Conocimientos de Python, Power BI o Tableau.
* Comprensión de la limpieza de datos.
* Comprensión de la visualización de datos.



#### Nivel de ejercicio: Intermedio


# Objetivo:


En este proyecto, se realiza el análisis de datos sobre un conjunto de datos abiertos procedentes de Airbnb. Algunas de las tareas incluyen:

- limpieza de datos,
- transformación de datos y
- visualización de datos.



## Resumen sobre los datos de Airbnb:


Los criterios principales de la gente cuando visita lugares nuevos son contar con alojamiento y comida a precios razonables. Airbnb (Air-Bed-Breakfast) es un mercado en línea creado para satisfacer esta necesidad, pues permite a la gente alquilar sus casas durante plazos cortos. Estos servicios se ofrecen a un precio relativamente inferior al de los hoteles y en diversas ubicaciones geográficas. Además, personas de todo el mundo prefieren el servicio hogareño y económico.



## Fuente de los datos


Puedes obtener el <i>dataset</i> para realizar este proyecto en el siguiente enlace: https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata


# Contenido del dataset
El conjunto de datos utilizado en este proyecto consiste en información de Airbnb en Estados Unidos. Este <i>dataset</i> contiene información sobre los alojamientos, tal como el barrio, el tipo de habitación, el precio, la disponibilidad, las opiniones, los gastos de servicio, la política de cancelación y las normas de uso de la casa. Mas concretamente, este <i>dataset</i> abarca los siguientes parámetros:

1. **id** = Identificador único de Airbnb para el anuncio.
2. **Name** = Nombre del anuncio.
3. **host id** = Identificador único de Airbnb para el anfitrión.
4. **host_identity_verified** = Identidad del anfitrión.
5. **host name = Nombre del anfitrión**. Generalmente, solo se incluye el nombre (o nombres).
6. **neighbourhood group** = Grupo de barrios.
7. **neighbourhood** = Barrio
8. **lat** = Utiliza la proyección del Sistema Geodésico Mundial (WGS84) para la latitud.
9. **long** = Utiliza la proyección del Sistema Geodésico Mundial (WGS84) para la longitud.
10. **country** = País.
11. **country code** = Código de país.
12. **Instant_bookable** = Un indicador de listado comercial. Indica si el huésped puede reservar automáticamente el anuncio sin necesidad de que el anfitrión apruebe la solicitud de reserva.
13. **cancellation_policy** = Política de cancelación.
14. **room type** = Tipo de habitación. Los anfitriones de Airbnb pueden ofrecer casas/apartamentos enteros, habitaciones privadas, compartidas y, más recientemente, habitaciones de hotel. Dependiendo del tipo de habitación y la actividad, un anuncio residencial de Airbnb podría parecerse más a un hotel, perturbar a los vecinos, restar viviendas disponibles e incluso ser ilegal.
15. **Construction year** = Año de construcción de la propiedad.
16. **price** = Precio (costo de la habitación por noche).
17. **service fee** = Tarifa de servicio.
18. **minimum nights** = Noches mínimas (número mínimo de noches requeridas para reservar el anuncio).
19. **number of reviews** = Número de revisiones (cantidad de revisiones que tiene el anuncio).
20. **last review**  = Última revisión (fecha de la última/más reciente revisión).
21. **reviews per month** = Revisiones por mes (número de revisiones que ha recibido el anuncio a lo largo de su vida útil).
22. **review rate number** = Número de tasa de revisión.
23. **calculated host listings count** = Recuento calculado de fichas de anfitriones.
24. **availability 365** = Disponibilidad del anuncio en los próximos x días según lo determinado por el calendario.
25. **house_rules**. Reglas de la casa.
26. **license** = Número de licencia/permiso/registro.


## Tarea 1: Carga de datos 

1. Lee el fichero csv y cárgarlo en un <i>dataframe</i> de pandas.
2. Visualiza las cinco primeras filas de tu <i>dataframe</i>.
3. Visualize los tipos de datos de las columnas.

## Tarea 2: Limpieza de datos 


1. Elimina las columnas no deseadas del <i>dataframe</i>, entre ellas se incluyen `host id`, `id`, `country` y `country code`.
2. Indica la razón por la cual se han eliminado estas columnas para tu análisis de datos.
3. Compueba si hay valores nulos y muestra el recuento en orden ascendente. **Si faltan valores, imputa los valores como consideres.**
4. Comprueba si hay valores duplicados y elimínalos.
5. Muestra el número total de registros antes y después de eliminar los duplicados.


## Tarea 3: Transformación de datos 

- Cambia el nombre de la columna `availability 365` a `days_booked`.
- Convierte todos los nombres de columna a minúsculas y sustituye los espacios en los nombres de columna por un guión bajo "_".
- Elimina el signo de dólares y la coma de las columnas `price` y `service_fee`. Si es necesario, convierte estas dos columnas al tipo de datos adecuado.

## Tarea 4: Análisis exploratorio de datos

- Enumera los tipos de habitaciones disponibles en el <i>dataset</i>.
- ¿Qué tipo de habitación tiene la política de cancelación más estricta?
- Enumera el precio medio por barrio y señala cuál es el conjunto de barrios más caro para alquilar.

## Tarea 5: Visualización de datos (Cualquier herramienta)

* Enumerar los distintos tipos de habitaciones disponibles en Airnb
* Qué tipo de habitación se adhiere a una política de cancelación más estricta.
* Enumere los precios por grupo de barrios y mencione también cuál es el grupo de barrios más caro para los alquileres.
* Enumere los 10 barrios más caros por orden creciente de precio con la ayuda de un gráfico de barras horizontales. ¿Cuál es el barrio más barato?
* Enumere los barrios que ofrecen alquileres a corto plazo de menos de 10 días. Ilustrar con un gráfico de barras
* Enumere los precios con respecto al tipo de habitación utilizando un gráfico de barras y exponga también sus inferencias.
* Cree un gráfico circular que muestre la distribución de los días reservados para cada grupo de barrios.
* ¿El precio del servicio y el precio de la habitación tienen un impacto mutuo? Ilustre esta relación con un gráfico de dispersión e indique sus inferencias
* Utilizando un gráfico lineal muestre en qué año tuvo lugar la máxima construcción de habitaciones.
* Con la ayuda de gráficos de caja ilustra lo siguiente
* Efecto del número de tasa de revisión en el precio
* Efecto de la identidad del host verificada en el precio
---


  



