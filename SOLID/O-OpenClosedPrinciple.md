# Open/Close Principle

Las clases deben estar abiertas a la extensión pero cerradas a la modificación.
Su idea fundamental es evitar que el codigo existente se descomponga cuando implementas nuevas funciones.
Se suele solcionar este problema aplicando polimorfismo

Ejemplo sin implementar el principio

Damos el caso de que tenemos un dashboard que tiene la funcion crear unos widget para un DashBoard y por otro lado tenemos la función que nos dibuja los widget en pantalla.
Una vez finalizada la implmenetación, nos llega un requerimiento para crear otro widget mas exclusivo para clientes premium. Lo incorrecto de acuerdo a este principio seria modificar la cfunció de widget para agregar este nuevo que es el gerencial.
Aca un ejemplo agregando este nuevo widget

![Imagen de unas nubes](/SOLID/Images/OpenClosedPrincipleWrong.png)

La solución ideal es generar nuevas clases que implementen dichas funcionalidades, para esto puedes extender las clases y agregar tus nuevas funcionalidades.

Aca la manera correcta de aplicar el principio

![Imagen de unas nubes](/SOLID/Images/OpenClosedPrincipleGood.png)