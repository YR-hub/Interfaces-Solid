# SEGREGATION

Principio de segregación de interfaz: Los clientes no deben verse obligados a depender de interfaces que no utilizan. En lugar de tener una única interfaz monolítica para todos los métodos relacionados con los empleados, dividiremos la interfaz en interfaces más pequeñas y cohesivas.

Principio de inversión de dependencia: Los módulos de alto nivel no deben depender de los módulos de bajo nivel. Ambos deben depender de abstracciones. Crearemos una capa de abstracción entre la capa de negocios y la capa de acceso a la base de datos para invertir la dependencia.

# DEPENDENCIA

En el ejemplo anterior, hemos aplicado el principio de segregación de interfaz dividiendo la interfaz de empleados en interfaces más pequeñas y cohesivas (EmployeeReader y EmployeeWriter). Luego, creamos una interfaz combinada EmployeeRepository que extiende ambas interfaces.

También aplicamos el principio de inversión de dependencia al introducir la interfaz DatabaseConnection, que permite que la capa de negocios (EmployeeService) dependa de una abstracción en lugar de una implementación concreta. Esto nos permite cambiar fácilmente
