# Ejercicios

Antes de empezar asegúrate de haber leído las indicaciones para trabajar con BaseX, la herramienta recomendada para hacer la tarea:

* [Indicaciones](./Indicaciones_BaseX.pdf) para usar e instalar [BaseX](https://basex.org)
* En esta tarea se utilizan los ficheros [impresoras.xml](./../data/impresoras.xml) y [artistas.xml](./../data/artistas.xml).
* Completa **cada consulta en su correspondiente fichero** numerado (ya están creados e indexados en este documento por cada consulta).

1. A partir del fichero `artistas.xml`, escribe consultas XQuery que devuelvan:

    1. Nombre y país de todos los artistas. ([consulta](./../queries/consulta1.1.xq))
    2. El nombre (sin etiquetas) de los artistas que nacieron antes de 1500. ([consulta](./../queries/consulta1.2.xq))
    3. Nombre de los artistas para los que no hay año de fallecimiento. ([consulta](./../queries/consulta1.3.xq))
    4. Una lista HTML con el nombre de los artistas nacidos en España. ([consulta](./../queries/consulta1.4.xq))
    5. El número de artistas nacidos antes de 1600. ([consulta](./../queries/consulta1.5.xq))

2. A partir del fichero `impresoras.xml`, escribe consultas XQuery que devuelvan:

    1. Modelo de las impresoras de tipo “láser”. ([consulta](./../queries/consulta2.1.xq))
    2. Marca y modelo de las impresoras con más de un tamaño . ([consulta](./../queries/consulta2.2.xq))
    3. Marca y modelo de las impresoras con tamaño A3 (pueden tener otros). ([consulta](./../queries/consulta2.3.xq))
    4. Marca y modelo de las impresoras con tamaño A3 como único tamaño . ([consulta](./../queries/consulta2.4.xq))
    5. Modelo de las impresoras en red. ([consulta](./../queries/consulta2.5.xq))
