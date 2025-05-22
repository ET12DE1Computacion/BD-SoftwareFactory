## Software Factory - Guía Stored Procedure/Function

1) Realizar la función llamada `CostoProyecto` que reciba como parámetro unIdProyecto, la función tiene que devolver el costo del proyecto `Sumatoria del producto del costo base de la tecnología por la complejidad del requerimiento`.
2) Realizar el SP 'EmpleadosAptos' que reciba como parámetro unIdRequerimiento, el SP tiene que devolver nombre, apellido y calificación de los empleados que tengan al menos, la calificación que requiere el requerimiento (`Requerimiento.complejidad`). Ordenar empleados por calificación de mayor a menor y luego por fecha de contratación, comenzando por los más antiguos.

  ```sql
  CALL EmpleadosAptos(1);
  ```
  | Nombre    | Apellido| Calificación |
  | :---:     | :---:   | :---:        |
  | Beymar    | León    | 8            |
  | Arturo    | Cruz    | 8            |
  | Alexis    | Noguera | 6            |

3) Realizar el SP `AltaTecnologia` que reciba por parámetro el nombre de una tecnología y un parámetro de salida donde asigne el valor _autoincremental_ que haya asignado la BD. Van a tener que usar la función sin parametro [`LAST_INSERT_ID()`](https://www.w3schools.com/sql/func_mysql_last_insert_id.asp) que devuelve el ultimo valor que genero la BD para una clave autoincremental.

  ```sql
  CALL AltaTecnologia('Go', @salida);
  SELECT '@salida 'El valor de Salida'
  ```
  | El valor de Salida  |
  | :---:               |
  | 14                  |
  
4) 

[<< VOLVER](../05%20AGBD/README.md)