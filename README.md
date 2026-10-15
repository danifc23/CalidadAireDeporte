# Calidad Aire Deporte

## Problema

Practico deporte al aire libre en Granada, sobre todo salir a correr.
Cuando corro, respiro más cantidad de aire y me preocupa que el aire
que estoy respirando no sea de buenas condiciones. 
Además, he notado que cuando las condiciones del aire son peores, mi rendimiento durante la
actividad también es peor.
Normalmente puedo salir
por la mañana, por la tarde o por la noche, dependiendo del horario que tenga ese día.

El problema es que, cuando tengo que decidir cuándo salir a correr, no
sé qué condiciones de calidad del aire hay en las diferentes franjas
horarias. Actualmente no tengo esa información para poder tenerla en
cuenta al elegir cuándo realizar la actividad.


## Datos ambientales

Para abordar el problema se utilizarán datos reales de calidad del aire
publicados por la Junta de Andalucía.

[fuente de datos de la Junta](https://www.juntadeandalucia.es/medioambiente/atmosfera/informes_siva/cuantitativo/2026/)

Estos datos se van actualizando por cada día que pasa.
La fuente proporciona un fichero de datos para cada día. Los ficheros siguen el formato GR_AAAAMMDD.csv, donde GR identifica Granada y AAAAMMDD indica la fecha de las mediciones.

Los datos utilizados contienen mediciones horarias de calidad del aire
y permiten relacionar las concentraciones de los contaminantes con una
hora concreta.

Para el estudio se utilizarán los datos correspondientes a la estación
GRANADA - NORTE.

Los datos disponibles incluyen mediciones de PM10, PM2.5, NO2, O3 y SO2.
Para este problema se tendrán en cuenta PM10, PM2.5, NO2 y SO2.

Los datos contienen información de fecha y hora junto con las
mediciones de los contaminantes, lo que permite analizar las condiciones
del aire en diferentes franjas horarias.

## Qué se necesita analizar

La logica a seguir es comparar las diferentes franjas horarias teniendo en cuenta
conjuntamente los contaminantes disponibles.

Los cuatro contaminantes tendrán la misma importancia. Una concentración
baja será favorable y una concentración especialmente alta penalizará
la valoración de esa franja.

Cuando no exista un dato para un contaminante en una determinada hora,
ese contaminante no se tendrá en cuenta en la valoración de esa hora.

La valoración de una franja se obtendrá a partir de los contaminantes
que tengan datos disponibles, de forma que se puedan comparar las
diferentes horas del día.

La franja con una valoración más favorable será la considerada como mejor para realizar la actividad.

## Documentación

configuración [configuracion del repositorio](docs/configuracion.md)

## Juego de rol

![Tarjeta del juego de rol con mi problema](tarjetaRol.jpeg)

## Tarjeta Validacion

![Tarjeta de Validación](tarjetaValidacion.jpeg)

## Configuración

La configuración inicial del proyecto se realizará mediante las herramientas y servicios necesarios para su desarrollo y posterior despliegue en la nube.
