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
### HU001 - Incertidumbre sobre la contaminación al practicar deporte

Como persona que practica deporte al aire libre en Granada y dispone de horarios limitados, 
desconozco qué condiciones de contaminación atmosférica habrá durante mi actividad.
La concentración de contaminantes varía según la hora y el día, por lo que puedo acabar 
realizando ejercicio en condiciones desfavorables sin saberlo previamente.
Esta incertidumbre dificulta decidir si salir a practicar deporte, 
ya que podría exponerme a niveles elevados de contaminación atmosférica que afecten a 
las condiciones en las que realizo mi actividad.
[HU001 en GitHub](https://github.com/danifc23/CalidadAireDeporte/issues/2)

### HU002 - Comparar franjas horarias

Como persona sensible a la contaminación atmosférica que practica deporte al aire libre en Granada 
y dispone de flexibilidad horaria, desconozco qué momentos del día presentan condiciones 
más favorables para realizar mi actividad.
Los niveles de los distintos contaminantes varían a lo largo del día y no siempre evolucionan de 
la misma manera, por lo que resulta difícil identificar qué horario supone una menor exposición a la contaminación.
Esta situación dificulta elegir cuándo realizar mi actividad deportiva, ya que podría escoger un horario 
con niveles elevados de contaminación existiendo otras alternativas más favorables.
[HU002 en GitHub](https://github.com/danifc23/CalidadAireDeporte/issues/3)

# Milestones

## Milestone 0 - Primera versión interna del proyecto
### Producto mínimamente viable:

Una primera versión de una biblioteca de código organizada en un paquete 
que pueda ser utilizado por otros módulos del proyecto.

El contenido del paquete se determinará mediante el análisis del problema planteado en la 
historia de usuario, identificando sus conceptos y relaciones antes de comenzar a programar.

### Criterio de validación:

El producto se considerará válido cuando:
- El código desarrollado esté justificado por el análisis del problema descrito en HU001.
- Se pueda comprobar el proceso de análisis y diseño seguido, relacionando las decisiones tomadas con los issues y commits correspondientes.
- El código esté correctamente organizado y supere las comprobaciones de sintaxis o compilación correspondientes al lenguaje utilizado.
  
Historias de usuario asociadas: HU001 y HU002.

## Milestone 1 - Primera versión con lógica de negocio
### Producto mínimamente viable:

Una nueva versión de la biblioteca desarrollada en el Milestone 0, empaquetada 
de forma que pueda ser utilizada por otros componentes del proyecto.

Esta versión incorporará la lógica de negocio necesaria para avanzar en la resolución del problema 
descrito en HU001. Su contenido se determinará a partir del análisis del problema y 
de los resultados obtenidos en el milestone anterior.

### Criterio de validación:

El producto se considerará válido cuando:
- La lógica de negocio implementada esté justificada por los problemas descritos en HU001
  y los issues derivados de ella.
- Se pueda comprobar el proceso de desarrollo seguido mediante los issues y commits correspondientes.
- La biblioteca pueda utilizarse desde otros módulos del proyecto.
- Se hayan desarrollado y superado pruebas automatizadas que comprueben el comportamiento implementado
  frente a los casos derivados de la historia de usuario.

Historias de usuario asociadas: HU001 y HU002.
