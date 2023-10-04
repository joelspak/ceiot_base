# Ejercicio CiberKillChain - Ataque

 * Alumno: Joel Spak
 * Link al trabajo práctico: https://docs.google.com/document/d/1h9-l0jWH3PkarOiJRDv6Zb0b7ReHZj9A1A210QfYUMQ/edit?usp=sharing

### Ejercicio aplicado al proyecto de monitoreo de consumo doméstico de energía eléctrica
Objetivo del ataque: robar una joya de la casa de una persona en específico, que ha alardeado en sus redes sociales de haber adquirido un moderno sistema de monitoreo de consumo de energía eléctrica.

* Reconnaissance
  -  obtengo información sobre el servidor de la aplicación, comunicándome con los dueños de la aplicación e intentando obtener la mayor cantidad de detalles.
  -  intento obtener información sobre el host de la víctima para utilizarla durante el ataque (T1592) y sobre su topología de red para obtener datos (T1590).

* Weaponization
  - podría intentar adquirir acceso a la red del usuario (T1650).
  - podría codear un virus para filtrarlo en la red del usuario.
  - podría armar un frontend similar al de la aplicación con el objetivo de extraer datos del usuario.
  - decido codear una app web con el mismo frontend de la aplicación, que solicite credenciales del usuario para acceder. Una vez colocadas, redirige a una página que dice que está todo ok y que las anomalías que se habían detectado fueron solucionadas.
  - armo un correo electrónico similar al que podría enviar la aplicación al detectar anomalías en el consumo eléctrico, con el objetivo de phishing, junto con la aplicación web copiada.
  
* Delivery
  - Envío el correo electrónico a la persona en cuestión.
  
* Exploit
  - el usuario cae en la trampa por confiar en que el correo proviene de la aplicación, y coloca sus credenciales en mi frontend. 
  
* Installation  
  - procedo a buscar vulnerabilidades en la aplicación para otorgarme un acceso nuevo y evitar perder el acceso en caso de que el usuario cambie sus credenciales.

* Command & Control
  - accedo a la aplicación con las credenciales del usuario.
  - ejecuto un script que permita leer el consumo y me notifique en caso de que baje de un cierto umbral que yo defina al ver como se comportan las curvas de consumo del usuario.

* Actions on Objectives
  - uso la información del usuario para establecer un criterio de cuando atacar y poder entrar, acorde al monitoreo de consumo. Debo asegurarme que el bajo consumo no sea por una falla eléctrica en el área, esto lo puedo hacer acercándome a la cuadra sin levantar sospecha de forma sigilosa y observar si hay energía eléctrica en la zona.
  
  

