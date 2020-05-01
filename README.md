# covid19_mexico_data

Aquí se mantienen los datos 🗂️ de fuentes oficiales en formato reproducible para facilitar el análisis del progreso de COVID-19 en México 🦠🇲🇽. Análisis, series de tiempo y gráficas aquí: [marianarf/covid19_mexico_data](https://github.com/marianarf/covid19_mexico_data).

### Fuentes 📈📈📈

``'dge/'``
+ **Dirección General de Epidemiología** - Los archivos en esta carpeta contiene los reportes diarios referente a los casos asociados a COVID-19 publicados por la [Dirección General de Epidemiología](https://www.gob.mx/salud/documentos/datos-abiertos-152127) a partir de ``2020-04-12``. Los datos se obtienen mediante ``zip`` el día de su publicación, o accediendo la base de datos histórica, que contiene los archivos en formato ``csv``.
  + Notas
    + _2020-04-30_ - La base de datos ahora incluye la variable ``Identificador``, la cual es única y aleatoria para cada caso.
    + _2020-04-21_ - A partir de este reporte, puede ser que el campo que reporta más acertadamente dónde se realizó la prueba, es ``ENTIDAD_RES`` y no ``ENTIDAD_UM``.
    + _2020-04-12_ - El campo de ``ID_REGISTRO`` no es un identificador único.

``'geo/'``
+ **INEGI** - 
Los archivos en esta carpeta contienen los nombres y claves oficiales de las entidades y municipios en México delineadas a través del marco geoestadístico del [INEGI](https://www.inegi.org.mx/app/biblioteca/ficha.html?upc=889463142683).
	
``'ssa/'``
+ **Secretaría de Salud** - 
Los archivos en esta carpeta contienen ``csv`` procesador a partir de las publicaciones diarias sobre COVID-19 que la Secretaría de Salud (InDRE) mantuvo hasta el día ``2020-04-19`` en formato pdf. Estos archivos fueron convertidos `csv` usando servicios como [ZAMAR](https://www.zamzar.com) y [ILovePDF](https://www.ilovepdf.com) y manualmente tabulando los casos nuevos, que se indican como filas resaltadas en color azul, en los archivos ``pdf``. A partir del día``2020-04-19``, los reportes de datos oficiales de la SSA han sido descontinuados, y presumiblemente, fueron asimilados por la Dirección General de Epidemiología.
  + Notas
    + _2020-04-10_ - Los reportes del día ``2020-04-06`` y ``2020-04-07``, en el campo que indica la fecha de inicio de síntomas, contiene la mayor parte de las entradas en formato de número (ejemplo: **43912**, **43914** y **43916**).
    + _2020-04-09_ - A partir de `2020-04-06`, los nuevos casos se concatenan al final de los reportes pasado.
    + _2020-04-01_:  Cambia de forma significativa la estructura de sus datos y también elimina el campo `Origen`.

### Más información 🔍

Si eres reserarcher 👩‍🔬👨‍🔬📈 y quieres incepcionar a las meras, meras, fuentes, hay otros repos y sitios no oficiales que se han dedicado a mantener,  comentar y archivar los datos y las series de tiempo de fuentes oficiales:

* https://serendipia.digital/
* https://www.covid19in.mx/
* https://github.com/guzmart/covid19_mex/
