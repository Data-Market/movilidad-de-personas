# Dataset de Movilidad de Personas

<table align="center">
  <tbody>
    <tr align="center">
      <td width="33%">
        <a href="https://github.com/Data-Market/movilidad-de-personas">
          <img src="https://datamarket.es/media/images/movilidad-de-personas-image.png" style="max-width:100%;">
        </a>
      </td>
      <td width="33%">
        <a href="https://datamarket.es">
          <img src="https://datamarket.es/static/core/img/logo-og.png" style="max-width:100%;">
        </a>
      </td>
    </tr>
  </tbody>
</table>

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

| nombre               | tipo     | descripción                                                                                                                               | ejemplo                                                                                                                          |
|----------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
| date                 | datetime | Fecha en la cual se inicia un desplazamiento.                                               | 2020-12-08                                                                                                                       |
| origin_id            | int      | ID del lugar en el cual comienza un desplazamiento.                                                                                                | 4625016                                                                                                                          |
| origin_lat           | geo      | Latitud del centroide del punto final del desplazamiento.  | 39.46975                                                                                                                         |
| origin_lon           | geo      | Longitud del centroide del punto final del desplazamiento. | -0.37739                                                                                                                         |
| origin_activity      | str      | Actividad que se deja de efectuar debido al desplazamiento.                                                                            | Casa                                                                                                                             |
| destination_id       | int      | ID del lugar en el cual termina un desplazamiento.                                                                                           | 12138                                                                                                                            |
| destination_lat      | geo      | Latitud del centroide del punto final del desplazamiento.   | 39.98567                                                                                                                         |
| destination_lon      | geo      | Longitud del centroide del punto final del desplazamiento.  | -0.04935                                                                                                                         |
| destination_activity | str      | Actividad que motiva el desplazamiento.                                               | Otros                                                                                                                            |
| origin_polygon       | geo      | Área de superficie del origen de un determinado desplazamiento representado mediante coordenadas geográficas en UTM.                                | POLYGON ((724170.8735999996 4374062.2238, 724237.2073999997 4373941.599300001, 724016.7068999996 4373802.0811, 723941.3515999996... |
| destination_polygon  | geo      | Área de superficie del destino de un determinado desplazamiento representado mediante coordenadas geográficas en UTM.                              | POLYGON ((794152.4726999998 4484794.095699999, 794045.5981999999 4484669.313499999, 793923.5981999999 4484595.315199999, 793735... |
| province             | str      | Residencia de las personas que están realizando un determinado desplazamiento.                                                                 | Valencia                                                                                                                         |
| age                  | int      | Edad del civil que realiza un desplazamiento.                                                                                                 | None                                                                                                                             |
| hour_of_day          | int      | Hora de inicio del desplazamiento.                                                                                                 | 16                                                                                                                               |
| distance             | str      | Intervalo de distancia (en kms) en el que se agrupan los desplazamientos.                                                             | 010-050                                                                                                                          |
| n_trips              | int      | Número de desplazamientos de distancia comprendida en el intervalo "distance" que comienzan a la hora "hour_of_day".                                                                                 | 7706                                                                                                                             |
| trips_km             | int      | Suma de los kms totales de los viajes realizados con inicio "hour_of_day" en el día "date".                                                                   | 310253                                                                                                                           |
| year                 | int      | Año en el que se realiza el desplazamiento.                                                                                                                   | 2020                                                                                                                             |
| month                | int      | Mes en el que se produce el desplazamiento.                                                                                                                   | 12                                                                                                                               |
| day                  | int      | Día en el que se inicia el desplazamiento.                                                                                                                   | 8                                                                                                                                |
| hour                 | int      | Hora de inicio del desplazamiento.                                                                                                                           | 22                                                                                                                               |
