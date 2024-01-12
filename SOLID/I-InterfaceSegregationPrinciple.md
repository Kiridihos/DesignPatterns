# Interface Segregation Principle

Se deben desintegrar las interfaces "gruesas" hasta crear otras mas detallasadas y especificas. Los clientes deben implementar unicamente aquellos metodos que necesitan de verdad. De lo contrario, un cambio en una interfaz "Gruesa" descompondrpa incluso clientes que no utilizan metodos cambiados.

Para el siguiente diagrama encontramos que uno de los proveedores hace uso de varios de los servicios que se implementaron inicialmente para la empresa Amazon, sin embargo más adelante para la obtención de los servicios por parte de Dropbox, se encontró que no hace uso de todas las funciones de Amazon por lo que caemos en un error en el principio de segregación de interfaz

![](/SOLID/Images/InterfaceSegregationPrincipleWrong.png)


A continiación una implementación correcta sore el principio en el que se hace uso de varias interfaces mas sencillas o menos gruesas por lo que un nuevo proveedor puede implementar la interfaz que este a su necesidad.


![](/SOLID/Images/InterfaceSegregationPrincipleGood.png)

> Recordar que cuantas mas interfaces se creen, mas se complicara el codigo por lo que hay que mantener un equilibrio.