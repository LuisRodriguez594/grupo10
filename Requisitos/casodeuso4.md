# Modificar 

## **ID:004** 
## **Breve Descripcion:** _El sistema modificará a un alumno_  
## **Actores principales**: _Profesor,Ayudante,Coordinador_
---------------------------------------------------------

## **Precondiciones:** Debe existir el alumno en la base de datos

---------------------------------------------------------

**Flujo principal:** 
1. El caso de uso empieza cuando encuentra al alumno en la base de datos
2. El sistema abrirá una nueva ventana donde permitirá la modificacion de los datos del alumno

----------------------------------------------------------
**Postcondiciones:** Se modifican los datos del alumno en la base datos
----------------------------------------------------------

**Flujos alternativos:** 
_Si el alumno a modificar no existe mostrará un mensaje de error_
_Si al modificar no se cambia nada saltará una alerta de "Nada modificado"_
