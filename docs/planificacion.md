# Planificación

## User journey
El User Journey se encuentra en [UserJourney.md](UserJourney.md).

## Persona
### Daniel
Estudiante universitario de Granada que sale a correr varias veces
por semana. Sus horarios dependen de las clases y necesita conocer
las condiciones previstas del aire para una hora concreta.

### José
Tiene 35 años y sale a caminar habitualmente. Es sensible a la
contaminación y dispone de varias horas libres para realizar su
actividad. Necesita identificar qué hora presenta mejores condiciones
previstas sin tener que analizar manualmente cada contaminante.

## Historias de usuario
### HU001 - Consultar calidad del aire

Como estudiante que tiene una hora determinada para salir a correr,
quiero obtener una predicción de la calidad del aire para esa hora,
para saber si las condiciones serán favorables o desfavorables
y decidir si mantengo o aplazo mi actividad.
[HU001 en GitHub](https://github.com/danifc23/CalidadAireDeporte/issues/2)

### HU002 - Comparar franjas horarias

Como persona sensible a la contaminación que dispone de varias
horas para salir a caminar, quiero que se determine automáticamente
qué franja tendrá las condiciones más favorables, considerando
conjuntamente las predicciones de los distintos contaminantes,
para reducir mi exposición sin tener que interpretar y comparar
manualmente todos los valores.
[HU002 en GitHub](https://github.com/danifc23/CalidadAireDeporte/issues/3)

# Milestones

## Milestone 0 - Modelado del dominio de calidad del aire

Desarrollar un módulo de código que permita representar 
los datos necesarios para predecir la calidad del aire en Granada.

### Producto mínimamente viable:

Un módulo que modele las siguientes entidades:

- Medición: contaminante, concentración, estación y fecha/hora.
- Predicción: concentraciones estimadas de los contaminantes para una hora futura.
- Franja horaria: intervalo de tiempo en el que se puede realizar una actividad deportiva.

### Criterio de validación:

El módulo deberá permitir representar correctamente estas entidades, 
incluyendo situaciones en las que falten mediciones. Se comprobará mediante pruebas automatizadas.

Historias de usuario asociadas: HU001 y HU002.

## Milestone 1 - Predicción de la calidad del aire

Desarrollar una biblioteca que permita predecir la calidad del aire en Granada y 
determinar qué franjas horarias serán más favorables para practicar deporte al aire libre.

### Producto mínimamente viable:

Una biblioteca que, utilizando las entidades del Milestone 0, permita:

- Predecir la calidad del aire: estimar las concentraciones de contaminantes para una hora futura a partir de mediciones anteriores.
- Evaluar las condiciones: determinar si la calidad del aire prevista es favorable o desfavorable para practicar deporte.
- Seleccionar la mejor franja horaria: comparar las predicciones de diferentes horas e identificar aquella que presente mejores condiciones.

### Criterio de validación:

La biblioteca deberá generar predicciones y seleccionar las franjas horarias más favorables. 
Su funcionamiento se comprobará mediante pruebas automatizadas, contrastando las predicciones con mediciones históricas 
y verificando que la selección de horarios sigue los criterios establecidos.

Historias de usuario asociadas: HU001 y HU002.
