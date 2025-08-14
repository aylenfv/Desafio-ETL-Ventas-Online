# Desafio-ETL-Ventas-Online
Desafío 1 del curso "Pandas: transformación y manipulación de datos" de Alura latam.

## Objetivo
El objetivo de este proyecto es analizar los resultados de un evento con los clientes de una empresa de venta online. Se recopiló un conjunto de datos que contiene los clientes que más gastaron en productos durante los 5 días de ventas, que es la duración del evento. Este análisis identificará al cliente con la mayor compra esta semana, quien recibirá un premio de la tienda, y posteriormente, puede ayudar a la empresa a crear nuevas estrategias para atraer más clientes.

La base de datos utilizada en este análisis es ![datos_ventas_clientes](Desafio-ETL-Ventas-Online/data/datos_ventas_clientes.json).json y contiene información importante sobre los clientes, como el nombre registrado del cliente, el monto total pagado al momento de la compra y el día de la compra.

## Etapa 1
Sabiendo esta información, el desafío del proyecto 1: ventas online será abrir la base de datos con Pandas y aplicar json_normalize.

## Etapa 2

Leímos la base de datos en el desafío anterior, ahora podemos seguir adelante con la transformación de estos datos. Así, el nuevo desafío del proyecto 1 será dividido en algunas metas:

* Eliminar datos en listas dentro del DataFrame;
* Verificar tipos de datos;
* Identificar columnas numéricas;
* Transformar la columna numérica a tipo numérico.

## Etapa 3

Debido a una inestabilidad en el sitio web de la empresa, tuvimos problemas con los nombres de los clientes durante el guardado. Esto resultó en una columna de nombres de clientes con una combinación de letras, mayúsculas y minúsculas, números y otros caracteres.

Sabiendo esto, manipula los textos de la columna Cliente para que el resultado sean los nombres de los clientes en letras minúsculas, con ausencia de caracteres especiales o números.

## Etapa 4

En los pasos anteriores ya hemos trabajado con varios tipos de datos, ahora podemos trabajar con datos de tiempo.

En la columna Fecha de venta tenemos fechas en el formato 'día/mes/año' (dd/mm/AAAA). Transforme estos datos al tipo datetime y busque una forma de visualización de subconjunto que pueda contribuir al objetivo del contexto en el que se insertan los datos.