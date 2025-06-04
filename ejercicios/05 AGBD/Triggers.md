## Software Factory - Guía Triggers

1. Antes de hacer un Insert en Tarea, si la calificación del empleado es menor a la complejidad del requerimiento no se tiene que permitir el Insert y se tiene que mostrar la leyenda `"Calificación insuficiente"`.
1. Realizar un trigger para que al ingresar un Empleado, le asigne por defecto experiencia en todas las tecnologías disponibles con calificación igual a _CERO_ (revisar ultima diapo de `"09 Consultas SQL - Insert - Delete - Update"`).
1. Al asignarle una tarea a un Empleado (_INSERT_ en Tarea), no se puede asignar una fecha de inicio anterior a la contratación del empleado; en ese caso, cancelar la operación y emitir la leyenda `"No se puede asignar esta fecha de inicio"`.
1. Al agregar un un _Requerimiento_, en caso de que no exista al menos un empleado que posea al menos el nivel de _calificación_ necesario para la _complejidad_ del _Requerimiento_ en cuestión, se tiene que cancelar la operación y mostrar la leyenda `'Requerimiento no alcanzable'` 

[<< VOLVER](../05%20AGBD/README.md)