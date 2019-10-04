# SAPCE SUIT
## EEH 
Son las siglas en inglés de (EMU Electrical Harnnesses), es el sistema que se encarga de administrar las funciones de los sensores biomédicos que esta compuesto por: los sensores de temperatura y sensor pulsoximetro; este módulo es controlado por un microcontrolador ATMEGA328P al que se le implementa un bootlader para Arduino, de manera que se pueda realizar desarrollos usando el IDE de Arduino.

Para que se pueda realizar el envío de información de la medición al microcontrolador se realiza mediante los distintos periféricos que lo componen, como se muestra en la siguiente tabla:

| Elemento | Referencia | Periférico |
| -------- | ----------|----------|
|Temperatura||ADCx|
|Pulsoximetría||I2C|


## LSS
Son las siglas en inglés de (Life Support Subsystem), en este apartado se implementa la electrónica asociada a este subsistema el cual se controla tanto los actuadores como son: los ventiladores, la bomba, y la linterna del casco, cómo tambien sensores como es el sensor de presión; este módulo es controlado por un microcontrolador ATMEGA328P al que se le implementa un bootlader para Arduino, de manera que se pueda realizar desarrollos usando el IDE de Arduino.
Para que se pueda realizar el envío de información de la medición y la devida actuación del microcontrolador se realiza mediante los distintos periféricos que lo componen, como se muestra en la siuguiente tabla:

| Elemento | Referencia | Periférico |
| -------- | ----------|----------|
|Ventilador||PWMx|
|Bomba||PWMx|
|Linterna||PWMx|
|Manómetro||ADCx|

# OBC
Son sigles en inglés de (On Board Computer) este sistema es básicamente la computadora que gestiona las funciones generales de los módulos; está desarrollado sobre una placa Raspberry PI 3B, que se divide en dos funciones principales que son: gestor de perifericos,y gestor de tareas internas.
## Gestor de periféricos
Se encarga de administrar los diferentes módulos por medio de una comunicación USB con los otros microcontroladores, enviando y recibiendo constantemente paquetes de datos en forma de JSON.
### EEH

### LSS

### Interfaz


## Gestor de tareas internas