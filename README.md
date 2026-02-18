# Actuadores Raspberry

El principal objetivo de está práctica es aprender a usar los actuadores Raspberry. Al inicio se crea un código en el que se muestra como podemos asignar los actuadores a los componentes que vamos a usar, así como definir si serán pines de entrada o de salida.

1º Parte:
Si se accede al historial de modificaciones del código se podrá encontrar el código usado en la primera parte de la práctica (código terminado) que funciona de la siguiente forma:

* Cuando se presione el botón por primera vez, se encenderá un led de color amarillo.
* Si se pulsa una segunda vez, se apagará el led de color amarillo y se encenderá un led de color rojo.
* Si se pulsa por tercera vez, se apagará el led de color rojo y se encenderá un zumbador durante 5 segundos. Pasados los 5 segundos, se mostrará un mensaje por pantalla preguntando por la clave para desactivar la
  alarma. Si el usuario introduce la clave correcta se mostrará por pantalla el mensaje “ALARMA DESACTIVADA”, pero si el usuario introduce una clave incorrecta, se mostrará el mensaje “AVISANDO A LA POLICÍA”.
* La clave correcta inicial es 1234, sin embargo, esta no es una clave válida y debe ser cambiada por el usuario. La nueva clave introducida debe contener 6 caracteres y al menos uno de ellos no debe ser              alfanumérico.
* Si salta la alarma antes de que la clave haya sido modificada, una vez desactivada la alarma, se debe pedir al usuario que modifique la clave.

2º Parte:
Si se vuelve a acceder al historal se podrá encontrar la segunda parte (Nueva práctica) en la que usando el código anterior como base se debe crear un nuevo código que funcione de la siguiente forma:

Si se pulsa el botón, se enciende un led amarillo, y se pregunta al usuario por una palabra clave, de la siguiente manera:

* Al iniciar el script, se debe crear el siguiente diccionario:
  contrasenas = {'color':'azul','flor':'amapola','animal':'perro','ciudad':'madrid','colegio':'salesianos'}
* Cuando se pulse el botón, se generará un número aleatorio, y se preguntará al usuario por el valor que coincide con la clave de la posición del número aleatorio. Por ejemplo, si el número es el 0, se              preguntará al usuario por un color, y si éste responde “azul”, la respuesta se considerará como correcta, en caso contrario, como incorrecta; si el número es el 3, se preguntará al usuario por un ciudad, y si     éste responde “madrid”, la respuesta se considerará como correcta, en caso contrario, como incorrecta.
* Si la respuesta es correcta, se apaga el led y se vuelve a comprobar si se pulsa el botón.
* Si la respuesta es incorrecta, se enciende un led rojo y se genera una llamada automática (a tu teléfono móvil) que al descolgar reproducirá el mensaje “se ha pulsado el botón y la contraseña es incorrecta”.
  Notas:
* Mientras no se pulse el botón, se imprimirá por pantalla “no hay movimiento”.
* Generar el comportamiento dentro de un bucle infinito.
* Se deben controlar las interrupciones por teclado.
