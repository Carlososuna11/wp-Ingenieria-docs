# Centrar Detalles de un Registro del Pod

1. Este apartado explica como solucionar el espacio del lado izquierdo de todos registro de los pod.
<p align="center"> <img src="https://imgur.com/x7wxShD.png"> </p>

2. Primeo accedemos al “Administrador de Pods”, y buscamos el pod de noticias, tenemos que estar atentos al valor del campo “Nombre” del pod.
<p align="center"> <img src="https://imgur.com/uhkQtLf.png"> </p>

3. Accedemos a “Fragmentos de Código”, editamos el código de “Configuracion de body_class para Staff, Noticias y Representantes estudiantiles”.
<p align="center"> <img src="https://imgur.com/X56VT9b.png"> </p>

4. Vemos el código ingresado, y nos centramos en el condicional que posee la función “is_post_type”, en el grupo de disyunciones, se agrega otra condición con la función “is_post_type”, pasando como un parámetro de tipo string el nombre del pod.
<p align="center"> <img src="https://imgur.com/S3XZbQV.png"> </p>

5. Podemos ver que se ha solucionado el problema del margen del lado izquierdo.
<p align="center"> <img src="https://imgur.com/XEvMBJ9.png"> </p>
<p align="center"> <img src="https://imgur.com/FMYgmWJ.png"> </p>