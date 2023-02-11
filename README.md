# JAVA
### Primer proyecto de java en el que se han realizado las siguientes tareas:  
* 1.- Prepara un menú que seleccione la ejecución de los diferentes ejercicios que se piden a continuación. Este menú se debe realizar con un switch.  
* 2.- Crea un método para todos y cada uno de los siguientes ejercicios. El método debe incorporar el calificador de acceso “public static'' y tener un nombre adecuado a lo que se solicita.  
La llamada al método se debe realizar desde el switch codificado en el ejercicio anterior. Los métodos a codificar deben realizar lo siguiente:  
  * A.- Leer 5 números (con bucle por favor, no pongáis 5 scanner consecutivos) y mostrarlos en el mismo orden introducido. Los 5 números se deben almacenar en un array.  
  * B.- Leer 5 números y mostrarlos en orden inverso al introducido.  
  * C.- Leer 5 números por teclado y a continuación realizar la media de los números positivos, la media de los negativos y contar el número de ceros que se han introducido por teclado.  
  * D.- Reciba como parámetro un texto y devuelva la cantidad de caracteres que incorpora el texto.  
  * E.- Reciba como par*ámetro un texto y devuelva el texto invertido.  
  * F.- Reciba como parámetro un texto y lo devuelva sin espacios en blanco.  
  * G.- Reciba como parámetro dos cadenas y las devuelva concatenadas.  
  * H.- Reciba como parámetro una cadena y una vocal, el método sustituye todas las vocales de la cadena por la vocal que se ha pasado como parámetro (no devuelve nada).  
  * I.- Reciba como parámetro una cadena, y muestre el código ASCII de cada uno de los caracteres de la cadena (no devuelve nada el método).  
 
 ### Extras  
 El menú incluye simbolos ASCII para dibujar el logo de MENU y el de final, ADIOS, en colores.  
 ![Imagen programa](https://github.com/raquel36/JAVA/blob/master/EjercicioUno/img/vistaJava.jpg)  
 He conseguido hacer una limpieza de pantalla con código en ANSI, además, después de la limpieza, también he conseguido que la vista por pantalla se presente en la parte superior.  
 Las secuencias de escape ANSI son secuencias de caracteres especiales que se utilizan para controlar la forma en que se muestra la información en la consola. Estas secuencias son específicas del estándar ANSI (American National Standards Institute) y se utilizan en sistemas operativos basados en Unix y en consolas de Windows.  
Las secuencias de escape ANSI permiten hacer cosas como mover el cursor a una posición determinada, cambiar el color de texto y fondo, limpiar la pantalla y mucho más.  
 Otra cosa que he incluido es que cuando se inicia el menú, se ejecuta un bucle de 5 segundos de espera, mostrando por pantalla un punto por segundo antes de ejecutar el menú, esta función se activa trás cada opción del menú y permite ver el resultado del programa antes de que se vuelva a mostrás el menú.  
 ![video.mp4](https://user-images.githubusercontent.com/119154158/218282441-f2f4a071-8cb7-4a6c-aa77-cd745d7704d0.mp4)  
 El menú está dentro de un bucle que hasta que no se pulsa la letra S/s no se sale del menú.  
 
 ### Algunos problemas surgidos
 #### Problema
 Al realizar el bucle y cuando se ejecutaba alguna de las opciones del menú me salia un error, comó que no se habia introducido ninguna opción y se cerraba el programa automáticamente.  
 ##### Solución
 Resulta que en los metodos de cada clase incluia un scan.close, lo que me provocaba este error, al eliminarlo, ya no se producia el error. El problema era que el método Scanner se cerraba y provocaba el cierre del bucle principal.  
 
 ##### Problema
 Otro problema que me ha surgido con el Scanner es que en el bucle lo llamaba con la variable scan y en los metodos, también por lo que solo leia el tipo del primer scan, que era de tipo .next, y los de tipo .nextLine no los leia.  
 ##### Solución
 He cambiado el nombre de la llamada al método Scanner en los métodos de texto por "input".  
 
 ##### Problema
 Al subir el proyecto al repositorio de github, no me cargaba correctamente. Era porque lo habia sacado de la carpeta principal y lo habia dejado solo en la carpeta secundaria (package).  
 ##### Solución
 He creado una carpeta nueva y he incluido las carpetas del proyecto en ella.
 
 ### Webgrafia  
Contar carácteres en JAVA  
https://www.delftstack.com/es/howto/java/count-characters-in-a-string-java/  
Sistemas para leer Strings desde el teclado  
https://www.abrirllave.com/java/leer-una-variable-de-tipo-string-desde-el-teclado.php  
Como obtener el valor ASCII de una letra de diferentes formas  
https://parzibyte.me/blog/2020/08/18/java-obtener-valor-ascii-char/#:~:text=Para%20hacer%20esto%2C%20simplemente%20%E2%80%9Ccasteamos,a%20otro%2C%20manteniendo%20el%20valor.&text=En%20este%20caso%20la%20salida%20ser%C3%A1%20El%20valor%20ASCII%20es%3A%2064.  
Convertir string a caracter   
https://www.techiedelight.com/es/convert-string-char-java/  
Generador letras ASCII  
https://www.letrabonita.net/2018/01/primera-entrada.html  
https://es.rakko.tools/tools/68/  
ANSI CODE  
https://en.wikipedia.org/wiki/ANSI_escape_code  
  
