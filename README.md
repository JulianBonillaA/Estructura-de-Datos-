# Sistema de Gestión de Ventas en Python

Este proyecto es un programa en Python que simula la gestión de ventas en diferentes departamentos para cada mes del año. El usuario puede interactuar con el sistema para insertar, buscar, eliminar y mostrar las ventas, todo esto a través de un menú interactivo en la consola.

## Funcionalidades

El sistema permite las siguientes operaciones:

1. **Insertar ventas**: El usuario puede ingresar las ventas de un departamento para un mes específico.
2. **Buscar ventas**: El usuario puede consultar las ventas registradas para un departamento y mes específico.
3. **Eliminar ventas**: El usuario puede eliminar una venta (poniendo su monto a 0) para un departamento y mes específico.
4. **Mostrar la tabla de ventas**: El sistema muestra una tabla con todas las ventas registradas, organizada por departamentos y meses.
5. **Salir**: El usuario puede salir del programa.

## Estructura de Datos

- **Departamentos**: El sistema maneja tres departamentos predeterminados: *Ropa*, *Deportes*, *Juguetería*.
- **Meses**: El sistema maneja los 12 meses del año.
- **Ventas**: Las ventas se almacenan en un diccionario bidimensional, donde el primer nivel es el departamento y el segundo nivel es el mes. El valor es el monto de la venta.

## Métodos del Programa

A continuación, te explico cómo funciona cada uno de los métodos que componen el programa:

### `insertar_venta()`
Este método permite al usuario ingresar una nueva venta para un departamento y mes específicos. El flujo de ejecución es el siguiente:

1. El sistema solicita al usuario que seleccione un departamento.
2. Luego, se le solicita seleccionar un mes.
3. Finalmente, se pide ingresar el monto de la venta, que se guarda en la estructura de datos.

Si el monto no es válido (no se puede convertir a un número), se muestra un mensaje de error.

### `buscar_venta()`
Este método permite al usuario buscar el monto de una venta registrada para un departamento y mes específicos. El flujo de ejecución es el siguiente:

1. El sistema solicita al usuario que seleccione un departamento.
2. Luego, se le solicita seleccionar un mes.
3. El sistema muestra el monto de la venta para ese departamento y mes, o indica que no se ha registrado ninguna venta si el monto es `0.0`.

### `eliminar_venta()`
Este método permite eliminar una venta (es decir, poner su monto a `0.0`). El flujo de ejecución es el siguiente:

1. El sistema solicita al usuario que seleccione un departamento.
2. Luego, se le solicita seleccionar un mes.
3. El monto de la venta para ese departamento y mes se pone a `0.0`.

### `mostrar_tabla()`
Este método muestra una tabla con todas las ventas registradas. El flujo de ejecución es el siguiente:

1. Se muestra una tabla con los nombres de los meses como encabezado.
2. Para cada departamento, se muestra el monto de las ventas para cada mes. Si no se ha registrado una venta, se muestra `0.0`.

### `obtener_entrada()`
Este es un método auxiliar utilizado por otros métodos para pedir y validar la entrada del usuario. Se encarga de mostrar las opciones disponibles (departamentos o meses), y valida si la entrada proporcionada por el usuario es válida. Si la entrada no es válida, el método muestra un mensaje de error y devuelve `None`.

---
