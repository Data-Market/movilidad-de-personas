# Dataset de Movilidad de Personas

<a href="https://datamarket.es">
  <img src="https://datamarket.es/static/core/img/banners/movilidad-de-personas-banner.png">
</a>

## Descripción

Datos sobre la __movilidad de personas en toda España__. Desplazamientos entre localidades y entre distritos con matriz de más de 2500 puntos de origen y destino. Este dataset ha sido creado enriqueciendo y limpiando los datos en bruto proporcionados por el Ministerio de Transportes, Movilidad y Agenda Urbana, en base al posicionamiento de teléfonos móviles.

Las características de este dataset son las siguientes:

* __Frecuencia de actualización__: diariamente, con un lag de 1-2 días
* __Volumen estimado__: 3-5 millones de registros cada día
* __Histórico__: disponible desde Febrero de 2020 en adelante

El dataset completo se puede adquirir en [DataMarket](https://datamarket.es/#movilidad-de-personas-dataset), plataforma de referencia de datos externos en España. 

Este repositorio contiene los siguientes recursos:

* La documentación completa del dataset.
* Una muestra representativa del mismo disponible para su evaluación y uso gratuito.

## Muestra

La muestra se encuentra disponible para descarga en el siguiente [link](https://github.com/Data-Market/movilidad-de-personas/blob/main/movilidad-de-personas-sample.csv).

## Documentación

A continuación se muestran las columnas de las que consta el dataset en el formato __nombre_columna__: __ejemplo_columna__, donde ejemplo_columna representa posibles valores que se pueden encontrar en dicha columna.

| nombre | tipo | descripción | ejemplo |
|--------|------|-------------|---------|
| date | datetime | Fecha en la cual se inicia un desplazamiento. | 2020-12-08 |
| day | int | Día en el que se inicia el desplazamiento. | 8 |
| destination_activity | str | Actividad que motiva el desplazamiento. | trabajo |
| destination_autonomous_region_name | str | Nombre de la Comunidad Autónoma de destino. | Comunitat Valenciana |
| destination_district_mitma_id | int | ID del lugar en el cual termina un desplazamiento. Correspondiente a un distrito para ciudades grandes, municipios para ciudades medianas o agrupación de municipios en el caso de ser pequeños. | 12138 |
| destination_district_name | str | Nombre del distrito de la ciudad al que pertenece el área del final del recorrido. Sólo está disponible para las ciudades de más de 500.000 habitantes. | None |
| destination_lat_centroid | geo | Latitud del centroide del punto final del desplazamiento. | 38.234478 |
| destination_lon_centroid | geo | Longitud del centroide del punto final del desplazamiento. | -0.814353 |
| destination_province_name | str | Nombre de la provincia de destino del desplazamiento. | Alicante/Alacant |
| destination_town_name | str | Nombre del municipio de destino del desplazamiento. En el caso de localidades pequeñas, puede incluir el nombre de varios pueblos de la región, separados por coma. | Crevillent |
| distance_km_interval | str | Intervalo de distancia (en kms) en el que se agrupan los desplazamientos. | 10-50 |
| home_province_name | str | Provincia de residencia de las personas que están realizando un determinado desplazamiento. | Valencia | 
| hour | int | Hora de inicio del desplazamiento. | 22 |
| month | int | Mes en el que se produce el desplazamiento. | 12 |
| n_trips | int | Número de desplazamientos de distancia comprendida en el intervalo "distance_km_interval" que comienzan a la hora "hour". | 19.558 |
| origin_activity | str | Actividad que se deja de efectuar debido al desplazamiento. | Casa |
| origin_autonomous_region_name | str | Nombre de la Comunidad Autónoma donde se inicia el desplazamiento. | Comunitat Valenciana |
| origin_district_mitma_id | int | ID del lugar en el cual comienza un desplazamiento. Correspondiente a un distrito para ciudades grandes, municipios para ciudades medianas o agrupación de municipios en el caso de ser pequeños. | 03059 |
| origin_district_name | str | Nombre del distrito de la ciudad al que pertenece el área del origen del recorrido. Sólo está disponible para las ciudades de más de 500.000 habitantes.ora de inicio del desplazamiento. | None |
| origin_lat_centroid | geo | Latitud del centroide del punto inicio del desplazamiento. | 38.209278 |
| origin_lon_centroid | geo | Longitud del centroide del punto inicio del desplazamiento. | -0.884140 |
| origin_province_name | str | Nombre de la provincia de origen del desplazamiento. | Alicante/Alacant |
| origin_town_name | str |  Nombre de la localidad donde se inicia el desplazamiento. En el caso de localidades pequeñas, puede incluir el nombre de varios pueblos de la región, separados por coma. | Albatera, San Isidro |
| total_km_traveled | float | Suma de los kms totales de los viajes realizados con inicio "hour" en el día "date" para dicha combinación de origen, destino y tipología de desplazamiento. | 205.856 |
| year | int | Año en el que se realiza el desplazamiento. | 2020 |
