# Liskov Substitutión Principle
Este principio es un grupo de comprobaciones que ayudan a predecir si una subclase permanece compatible con el código que pudo funcionar con objetos de la superclase. Este concepto es fundamental al desarrollar bibliotecas y frameworks, pro que otras personas utilizarán tus clases y no podrás acceder directamente ni cambiar su código.


Diagrama de una implementación incorrecta, ya que la clase padre lleva un método que presentara fallos para archivos que son de solo lectura. Método save();

![](/Images/LiskovSubstitutionWrong.png)


Una correcta implementación del principio se evidencia a continuación en la que se realiza la asociación de una clase para los documentos de escritura y a esta clase si se le implementa el metodo de save();



![](/Images/LiskovSubstitutionGood.png)



**Solución**

El problema se resuelve tras hacer a la clase de documentos de solo lectura la clase base de la jerarquía.

Puedes resolver el problema rediseñando la jerarquía de clases: una subclase debe extender el comportamiento de una superclase, por lo tanto, el documento de solo lectura se convierte en la clase base de la jerarquía. El documento de escritura es ahora una subclase que extiende la clase base y añade el comportamiento de guardar.