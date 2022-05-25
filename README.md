# Prototipo "Melabot"
## "Melanoma, responsable del 80 por ciento de muertes por cáncer de piel" (*Gaceta UNAM* Jun 28, 2019)

Decidí hacer un Bot de asistencia para auxiliar a identificar si una persona pudiera tener un Melanoma mediante un "rápido test" de preguntas que se hicieron a partir de los síntomas y riesgos que suelen tener las personas de acuerdo a la edad y género. Es importante mencionar que esto no es un diagnóstico completo, por lo que no se asegura que sea 100% fiable y no sustituye el diagnostico de un médico especialista, sin embargo, podría ayudar a las personas a identificar si necesitan ayuda de un profesional, además de acercar sitios de información donde podrán saber más información acerca del padecimiento.

Este Bot lo hice con ayuda de los servicios de Azure Health Bot
Para ayudar al Bot, también decidí hacer uso de los servicios de Inteligencia artificial de Microsoft Custom Vision, la entrene con fotos de lunares y manchas que estaban relacionadas al desarrollo de cáncer de melanoma, con otras que eran saludables y finalmente con fotos de zonas de piel donde no se tuvieran ningún tipo de macha o lunar. Haciendo pruebas acertó en todos los casos presentados.
Publiqué la IA para poder probarlo en una API, tanto el Bot como la IA pueden ser implementados en una página de dominio público para su funcionamiento.



### Bot de asisitencia
El Bot lo hice solamente tomando en cuenta factores básicos, ya que no es mi área de conocimiento, pero me gustaría profundizar las preguntas para obtener un historial más detallado y técnico.
La IA siempre se le puede entrenar con más imágenes para que sea aún más precisa y arroje porcentajes más altos de probabilidad.

![Logo](/SS/1_Bot.PNG "Estructura del Bot")

Este es la estructura del contenido del Bot, donde se establece el contenido y el funcionamiento del Bot, posteriormente se hacen las rutas que tomara dependiendo las respuestas que el usuario proporcione. 
A continuación, se puede ver un ejemplo de cómo responde el Bot.

![Logo](/SS/1.3_Bot.PNG "Ejemplo de Bot")
![Logo](/SS/1.4_Bot.PNG "Ejemplo de Bot")
![Logo](/SS/1.5_Bot.PNG "Ejemplo de Bot")
![Logo](/SS/1.6_Bot.PNG "Ejemplo de Bot")
![Logo](/SS/1.7_Bot.PNG "Ejemplo de Bot")

### Inteligencia Artificial para imágenes 
Se entrenó la IA con múltiples fotos de lunares benignos y malignos para que fuera más precisa la identificación de los lunares.
Se hicieron muchas pruebas, todas las imágenes procesadas fueron acertadas por la IA.  

![Logo](/SS/2.3_QuickTest.PNG "Prueba de IA")

Se sube una imagen y la IA comprueba que el lunar de la imagen es “Benigno” por lo que se le considera que no tiene riesgo.

Se hizo la prueba en 3 personas quienes ya tenían un diagnostico previo de un médico especialista, las pruebas realizas dieron un diagnóstico exacto de acuerdo con el diagnóstico del especialista. 

![Logo](/SS/2.5_Test_1_AC.PNG "API")

:small_orange_diamond: Se puede hacer uso de una API para pasar la información obtenida de la IA y del Bot para concentrar todo dentro de una interfaz o una página web para uso del usuario final.
Todavía hay muchas cosas mejorables y espacio para perfeccionar, como lo podría ser:
* Creación de una página web para la consulta de la prueba
  * Front end y Back end 
  * Información adicional para el usuario final 
* Aumentar el entrenamiento de la IA
* Asesoramiento con un médico especialista para el mejoramiento del Bot
