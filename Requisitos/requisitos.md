**Aqui se expondrán los requisitos del programa que queremos realizar en la practica 2**
Tenemos un caso en el cual, un cliente (profesor) nos pide que realicemos una aplicación para que él mismo pueda gestionar una base de datos de los alumnos de su clase. El profesor nos explica todo lo que quiere que la aplicación realice:

**Requisitos del usuario**

1. Insertar alumnos en la base de datos: Insertar varios alumnos, a los que habrá que añadir un mínimo de datos que son:    
    1.1. DNI    
    1.2. Nombre     
    1.3. Apellidos    
  Además de estos, el cliente podrá añadir todos los campos que quiera, siendo el total de datos el siguiente:  
    1.4. Teléfono personal  
    1.5. E-mail corporativo (UCO)   
    1.6. Dirección postal   
    1.7. Curso más alto en el que está matriculado  
    1.8. Fecha de nacimiento    
    1.9. Número del equipo en el que está enrolado  
    1.10. Saber finalmente si es el líder o no de este equipo   

2. Mostrar alumnos: opción que nos enseñe todos los alumnos que existen en la base de datos.
  2.1. Añadiremos una funcionalidad que nos permita mostrar los alumnos de la base de datos completa y otra que nos permita mostrar los alumnos de un determinado grupo de trabajo.   
  2.2. Añadiremos una funcionalidad para que el cliente pueda hacer que se muestren todos los alumnos cuyos datos coincidan con los campos introducidos: curso, numero de equipo y líderes de los grupos, por ejemplo.   

3. Buscar alumno: opción que nos permita buscar a un alumno concreto, introduciendo los siguientes datos:       
    3.1. Apellidos  
    3.2. DNI        
  En el caso de crear conflicto por coincidencia de apellidos, si es el campo buscado, se mostrarán los alumnos que coincidan, y se permitirá realizar al cliente una segunda búsqueda en la que podrá introducir los campos completos/correctos.   
    3.3. Si la búsqueda fuera errónea, permitir una segunda búsqueda que permita la correcta introducción de datos.

4. Modificar alumno: Esta opción nos permitirá realizar una búsqueda igual que en la opción anterior, pero en este caso el cliente podrá modificar los datos del alumno buscado.  

5. Borrar alumno: realizará una búsqueda en la cual, si se da conflicto por coincidencia (como en el caso anterior), realizará una segunda búsqueda, para así asegurarnos de que solo se borra un solo alumno.  

6. Borrar base de datos: En el caso de que el cliente quiera borrar su base de datos, esta opción lo permitirá. Antes de realizar el borrado de la base de datos, se le preguntará al usuario si está completamente seguro de querer borrarla, ya que puede seleccionar esta opción por error y perder todo el trabajo que haya realizado hasta el momento.   

7. Ordenar base de datos: Esta función permitirá al usuario ordenar la base de datos de acuerdo a los campos que quiera introducir, como puede ser:   
  7.1. Ordenar por cursos
  7.2. Ordenar por edad
  7.3. Ordenar por número de grupo  
  7.4. Ordenar por apellidos  
  7.5. Ordenar por DNI  
  Además, después de ordenar la base de datos, la aplicación deberá mostrar la base para comprobar que se ordenó correctamente.

8. Salir de la aplicación.


**Requisitos del usuario**

Esta sección tratará los requisitos que el usuario demanda en la aplicación que deberemos crear.

* Los 8 puntos antes expuestos son lo que el cliente nos pide que hagamos, principalmente.  
* El usuario requiere que la aplicación sea en sistema Linux.
* El máximo de alumnos será de 150.
* Se realizará una copia de seguridad cada cierto tiempo del fichero que realicemos con la aplicación.
* En cada grupo de trabajo solo podrá haber un líder, por lo que necesitaremos controlar el error en caso de que coincidan dos en un solo grupo.

**Requisitos del sistema**

*Requisitos funcionales*

Servicios que proporcionará el sistema, además de especificar el comportamiento que debe tener el sistema ante determinadas entradas, y decir que no debe hacer.

* El sistema estará codificado con un lenguaje simple, para que tanto el cliente como cualquier persona que quisiera utilizarlo, pudiera hacerlo sin ningún tipo de problema.
* El usuario deberá de tener la posibilidad de insertar todos los alumnos que quiera, introduciendo unos campos de información mínimos, y pudiendo insertar los alumnos desde esos campos hasta el total (10).
* El usuario deberá ser capaz de leer en la pantalla todos los alumnos de la base de datos, así como pedir que se muestren por grupos, por ejemplo.
* El usuario será capaz de buscar alumnos según distintos campos, como puede ser el DNI y los apellidos de dichos alumnos. En caso de conflicto (antes descrito), el sistema realizará una segunda búsqueda para poder buscar correctamente algún alumno concreto.
* El sistema permitirá que el cliente sea capaz de hacer una búsqueda(igual que en el punto anterior), y que modifique los campos que desee.
* En este caso, la búsqueda se realiza de la misma forma pero, para evitar borrados innecesarios, se preguntará si se desea borrar antes de hacerlo, y además en caso de conflicto, igualmente se realizará una segunda búsqueda para evitar que se borrren varios alumnos de la base de datos.
* El usuario debe ser capaz de ordenar la base de datos según el campo que desee, ya sea por curso, DNI, orden alfabético, o por grupo de trabajo, por ejemplo.

*Requisitos no funcionales*

* El sistema debe permitir un borrado completo de la base de datos, ya que el cliente en algún momento puede llegar a necesitarlo.
* El sistema estará basado en Linux, y a su vez se cargará en un sistema binario, por su mayor facilidad para realizar una base de datos.
* El máximo de alumnos, es decir, el tamaño máximo de la base de datos será de 150 alumnos.
* Las funcionalidades del sistema deben responder adecuadamente, es decir, la inserción, modificación, borrado y búsqueda de alumnos se deberían de realizar en menos de un segundo desde que se introduce la información por teclado.
* El sistema operará adecuadamente, ya que este está adecuado a que lo utilice solamente el cliente.
* El sistema realizará una copia de seguridad cada 2 minutos, para que si la computadora sufre un corte de electricidad, por ejemplo, el progreso del cliente esté asegurado todo lo posible.
* La aplicación será sencilla de utilizar siempre, ya que no siempre los clientes tendrán conocimientos de informática. Dicho esto, el tiempo de aprendizaje para utilizar esta aplicación debe de ser muy muy corto.
* El sistema, al ejecutarse, estará bien comentado con los pasos que deba dar el cliente. Además debe tener una interfaz gráfica agradable.
*  La base de datos no ocupará mucho espacio, para que sea sencillo poder llevarla de una computadora a otra o así mismo poder llevarla copiada en sistemas de almacenamiento externo.
*
