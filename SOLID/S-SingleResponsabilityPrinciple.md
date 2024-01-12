# Single Resonsability Principle
El principal objetivo es reducir la complejidad, buscando que cada clase sea responsable de una unica parte de la funcionalidad proporcionada por el software.

**Aca no se aplica el principio de unica responsabilidad**
```java
public class Employee {
	private String name = "Diego";
	public String getName() {
		return name;
	}
    public void printTimeSheetReport(){
        System.out.println("Imprimiendo Reporte");
    }
}
```
***
***
**Así deberia aplicarse el principio**
```java
public class Employee {	
	private String name = "Diego";
	public String getName() {
		return name;
	}
}
```

```java
public class TimeSheetReport {
    public void print() {
    	Employee employee = new Employee();
    	System.out.println(employee.getName());
    }
}
```
