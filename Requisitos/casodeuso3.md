# Buscar Alumno

## **ID:003** 
## **Breve Descripcion:** _El sistema buscará un alumno_  
## **Actores principales**: _Alumno_
---------------------------------------------------------

## **Precondiciones:** El alumno debe existir en la base de datos

---------------------------------------------------------

**Flujo principal:** 
1. El caso de uso empieza cuando existe el alumno en la base de datos
2. El sistema encontrará ha dicho alumno y mostrará los datos de este
3. El sistema accederá directamente a mostrar alumno una vez lo ha encontrado
4. Se buscará al alumno por dni o por email del mismo

----------------------------------------------------------
**Postcondiciones:** Se muestra por pantalla los datos de dicho alumno unicamente
----------------------------------------------------------

**Flujos alternativos:** 
_Si el alumno no existe, mostrará un mensaje de error_
