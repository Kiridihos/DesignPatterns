# Dependency Inversion Principle

Las clases de alto nivel no deben depender de las clases de bajo nivel. 
Ni alto nivel ni bajo nivel pueden depender de abstracciones.
Las abstracciones no denen depender de detalles.
Los detalles no pueden depender de abstracciones.

> Las clases de **Bajo nivel** implementan operaciones básicas, como trabajar con el disco, transferir datos por red, conectar con una base de datos, etc.

> Las Clases de **Alto Nivel** contienen la lógica de negocio compleja que ordena a las clases de bajo nivel que hagan algo

Este principio suele ir de la mano del principio de abierto/cerrado: se pueden extender clases de bajo nivel para utilizarlas con distintas clases de logica de negocio sin descomponer l¿clases existentes.

Aca observamos una mala implementación del principio en la que una clase de alto nivel depende de una clase de bajo nivel.

> ![](/Images/DependencyInversionPrincipleWrong.png)

En la siguiente imagen observamos una correcta impelmentación del principio en la que la clase de alto nivel, deja la dependencia con una clase de bajo nivel.

> ![](/Images/DependencyInversionPrincipleGood.png)
