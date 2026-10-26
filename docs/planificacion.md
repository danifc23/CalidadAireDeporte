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

### HU002 - Dificultad para elegir un horario con menor contaminación

Como persona sensible a la contaminación atmosférica que practica deporte al aire libre en Granada 
y dispone de flexibilidad horaria, desconozco qué momentos del día presentan condiciones 
más favorables para realizar mi actividad.
Los niveles de los distintos contaminantes varían a lo largo del día y no siempre evolucionan de 
la misma manera, por lo que resulta difícil identificar qué horario supone una menor exposición a la contaminación.
Esta situación dificulta elegir cuándo realizar mi actividad deportiva, ya que podría escoger un horario 
con niveles elevados de contaminación existiendo otras alternativas más favorables.
[HU002 en GitHub](https://github.com/danifc23/CalidadAireDeporte/issues/3)

# Milestones

## Milestone 0 - Modelado del problema.
### Objetivo

El contenido del paquete se determinará a partir del análisis del problema descrito en HU001.
A partir de esta historia de usuario se estudiarán los conceptos y las relaciones del dominio mediante issues, 
justificando las decisiones tomadas antes de representarlas en código.
En este milestone se trabajará únicamente en la modelización del problema, sin implementar todavía la lógica de negocio.

### Criterio de validación:

El producto se considerará válido cuando:
- Los problemas de modelado se hayan identificado a partir de HU001 y analizado mediante issues.
- Las entidades, objetos valor y sus relaciones estén justificadas mediante el análisis del dominio.
- El código represente el modelo obtenido mediante DDD, siguiendo las buenas prácticas del lenguaje elegido.
- El modelo permita representar un caso real de contaminación horaria y sirva como base para desarrollar posteriormente la lógica de negocio.
  
Historias de usuario asociadas: HU001.

## Milestone 1 - Primera versión con lógica de negocio
### Objetivo

Utilizar el modelo desarrollado en el Milestone 0 para implementar la lógica de negocio que permita predecir 
las condiciones de contaminación para una hora concreta y determinar si son favorables para practicar deporte, abordando HU001.

### Criterio de validación:

El producto se considerará válido cuando:
- La lógica implementada permita resolver el problema planteado en HU001 utilizando el modelo desarrollado anteriormente.
- Se hayan desarrollado pruebas automatizadas que comprueben el comportamiento esperado ante diferentes condiciones
  de contaminación, incluyendo casos con datos insuficientes.
- Las pruebas automatizadas se ejecuten correctamente y permitan comprobar que la lógica de negocio funciona según los requisitos establecidos.

Historias de usuario asociadas: HU001.
