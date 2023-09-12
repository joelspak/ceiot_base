# Ejercicio CiberKillChain - Ataque

 * Alumno: Joel Spak
 * Link al trabajo práctico: https://docs.google.com/document/d/1h9-l0jWH3PkarOiJRDv6Zb0b7ReHZj9A1A210QfYUMQ/edit?usp=sharing

### Ejercicio aplicado al proyecto de monitoreo de consumo doméstico de energía eléctrica
Objetivo del ataque: robar una joya de la casa de una persona en específico, que ha alardeado en sus redes sociales de haber adquirido un moderno sistema de monitoreo de consumo de energía eléctrica.

* Reconnaissance
  -  obtengo información sobre el servidor de la aplicación, comunicándome con los dueños de la aplicación e intentando obtener la mayor cantidad de detalles.
  -  intento obtener información sobre el host de la víctima para utilizarla durante el ataque (T1592) y sobre su topología de red para obtener datos (T1590).

* Weaponization
  - intento adquirir acceso a la red del usuario (T1650).
  - puedo codear un virus para filtrarlo en la red.
  
* Delivery
  - Envío el virus a través de correos electrónicos al usuario.
  - me hago pasar por la aplicación de medición de energía en ese correo electrónico.
  
* Exploit
  - el usuario cae en la trampa por confiar en la aplicacion y entra al correo
  
* Installation  
  - el virus se mete en la red del usuario y puedo comenzar a extraer información

* Command & Control
  - ejecuto las consultas a la base de datos del usuario y usar la aplicación
  - creo un data set del consumo de energía eléctrica del usuario

* Actions on Objectives
  - uso la información del usuario para establecer un criterio de cuando atacar y poder entrar, acorde al monitoreo de consumo. Registro que el bajo consumo no sea por una falla eléctrica en la cuadra, esto lo puedo hacer acercándome a la cuadra sin levantar sospecha de forma sigilosa y observar si hay energía (viendo la iluminación por ejemplo)
  
  

