---
layout: post
title: Limpieza y analisis de datos
author: Adrian E. Vazquez Icedo
date: '2019-12-12 22:18:00 +0530'
category: guides
summary: Limpieza y analisis de datos, accidentes de tránsito CDMX.
thumbnail: lim.jpg
permalink: /blog/Limpieza-y-analisis-de-los-datos.
---

La ciudad de México es una de las ciudades mas pobladas del mundo donde la vialidad automovilistica provoca grandes problemas.

El objetivo de este analizis es poder prevenir accidentes viales y disminuir las consecuencias que estos pueden tener con base a las fechas, horas, localizacion y delegaciones donde sucedieron accidentes en los ultimos 4 años en la ciudad de México.

Estos datos fueron recopilados del portal de datos de la ciudad de México:[Datos CDMX][datos-cdmx].

Primero cargamos los datos en el archivo "incidentes-viales-c5-csv", el cual contiene 1206191 registros con 18 parametros que nos permitaran realizar algunos analisis. 

![limp](/assets/img/d1.png)

![limp](/assets/img/d2.png)


Ahora es necesario eliminar valores nulos para quedarnos con puros registros con datos completos.

![limp](/assets/img/data.png)           ![limp](/assets/img/dataN.png)            ![limp](/assets/img/dC.png)

Para terminar de limpiar la informacion sera necesario quedarse unicamente con registros que fueron validados por el c5, esto permitira sacar informacion confiable basada en datos que han sido validados. 

![limp](/assets/img/T_A.png)

El c5 considera "reales" los registros con codigo de cierre afirmativos e informaticos. Con lo cual nos quedarian 544076 registros.

![limp](/assets/img/dV.png)

![limp](/assets/img/delegacion.png)

![limp](/assets/img/delegacion2.png)


[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
[datos-cdmx]: https://datos.cdmx.gob.mx/explore/dataset/incidentes-viales-c5/table/
[lim-jpg]: lim.jpg