# Movilidad de Personas

Datos sobre la movilidad de personas en las diferentes ciudades de España. Este dataset se puede adquirir en [Data Market](https://datamarket.es/#movilidad-de-personas-dataset), plataforma de referencia de datos externos en España. Puede consultar nuestro catálogo de datos en la siguiente url: [datamarket.es](https://datamarket.es/)

A continuación se muestran las columnas de las que consta el dataset en el formato __nombre_columna__: __ejemplo_columna__, donde ejemplo_columna representa posibles valores que se pueden encontrar en dicha columna.

| nombre               | tipo     | descripción                                                                                                                               | ejemplo                                                                                                                          |
|----------------------|----------|-------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
| date                 | datetime | Día en el cual se inicia un recorrido de un determinado civil desde su origen a su destino.                                               | 2020-12-08                                                                                                                       |
| origin_id            | int      | Punto de origen del recorrido de un civil.                                                                                                | 4625016                                                                                                                          |
| origin_lat           | geo      | Punto del centroide para latitud el cual representa una de las coordenadas geográficas del origen del recorrido de un determinado civil.  | 39.46975                                                                                                                         |
| origin_lon           | geo      | Punto del centroide para longitud el cual representa una de las coordenadas geográficas del origen del recorrido de un determinado civil. | -0.37739                                                                                                                         |
| origin_activity      | str      | Tipo de lugar del que parte cada civil para llegar al destino.                                                                            | Casa                                                                                                                             |
| destination_id       | int      | Lugar en el cual un civil termina su recorrido.                                                                                           | 12138                                                                                                                            |
| destination_lat      | geo      | Punto del centroide para latitud el cual representa una de las coordenadas geográficas del final del recorrido de un determinado civil.   | 39.98567                                                                                                                         |
| destination_lon      | geo      | Punto del centroide para longitud el cual representa una de las coordenadas geográficas del final del recorrido de un determinado civil.  | -0.04935                                                                                                                         |
| destination_activity | str      | Tipo de lugar en el que se encuentra un determinado civil después de terminar su recorrido.                                               | Otros                                                                                                                            |
| origin_polygon       | geo      | Área de superficie de origen de un determinado civil representado mediante coordenadas geográficas en UTM.                                | POLYGON ((724170.8735999996 4374062.2238, 724237.2073999997 4373941.599300001, 724016.7068999996 4373802.0811, 723941.3515999996 |
| destination_polygon  | geo      | Área de superficie del destino de un determinado civil representado mediante coordenadas geográficas en UTM.                              | POLYGON ((794152.4726999998 4484794.095699999, 794045.5981999999 4484669.313499999, 793923.5981999999 4484595.315199999, 793735. |
| province             | str      | Residencia de las personas que están realizando un determinado recorrido.                                                                 | Valencia                                                                                                                         |
| age                  | int      | Edad del civil que realiza un recorrido.                                                                                                  | None                                                                                                                             |
| hour_of_day          | int      | Hora de inicio del recorrido de un civil.                                                                                                 | 16                                                                                                                               |
| distance             | str      | Distancia entre el origen y el final del recorrido realizado por un civil.                                                                | 010-050                                                                                                                          |
| n_trips              | int      | Número de viajes que realiza una persona en un recorrido.                                                                                 | 7706                                                                                                                             |
| trips_km             | int      | Distancia en km desde el origen al final del recorrido de una persona.                                                                    | 310253                                                                                                                           |
