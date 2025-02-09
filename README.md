## Métodos del Programa

El programa utiliza varias funciones para realizar las operaciones necesarias con las ventas. A continuación se explican cada uno de los métodos implementados:

### 1. `insertar_venta()`

**Descripción**:  
Esta función permite al usuario insertar una venta en el sistema. El proceso es interactivo y solicita al usuario el departamento, el mes y el monto de la venta.

**Pasos**:
- Muestra los departamentos disponibles (Ropa, Deportes, Juguetería).
- Pide al usuario que seleccione un departamento.
- Muestra los meses disponibles (Enero, Febrero, ..., Diciembre).
- Pide al usuario que seleccione un mes.
- Solicita el monto de la venta.
- Almacena el monto de la venta en la matriz `ventas`, usando los índices del departamento y del mes.

**Funcionamiento**:
- El valor ingresado se guarda en la matriz `ventas` en la posición correspondiente (usando índices para el departamento y el mes).
- Si el departamento o mes no son válidos, la función muestra un mensaje de error.

### 2. `buscar_venta()`

**Descripción**:  
Este método permite al usuario buscar el monto de ventas registrado para un departamento y un mes específicos.

**Pasos**:
- Muestra los departamentos disponibles.
- Solicita al usuario que seleccione un departamento.
- Muestra los meses disponibles.
- Solicita al usuario que seleccione un mes.
- Recupera y muestra el monto de la venta en el departamento y mes seleccionados.

**Funcionamiento**:
- Utiliza los índices de los arreglos `departamentos` y `meses` para acceder a la matriz `ventas` y obtener el valor correspondiente de la venta.
- Si el departamento o mes no son válidos, la función muestra un mensaje de error.

### 3. `eliminar_venta()`

**Descripción**:  
Permite al usuario eliminar una venta registrada, lo que equivale a poner el monto de ventas a 0.0 para un departamento y mes seleccionados.

**Pasos**:
- Muestra los departamentos disponibles.
- Solicita al usuario que seleccione un departamento.
- Muestra los meses disponibles.
- Solicita al usuario que seleccione un mes.
- Establece el monto de ventas en la matriz `ventas` para esa combinación de departamento y mes a `0.0`.

**Funcionamiento**:
- Al igual que en `insertar_venta()`, utiliza los índices para acceder y modificar la matriz `ventas`. El valor de la venta se actualiza a `0.0`, eliminando así la venta registrada previamente.

### 4. `mostrar_tabla()`

**Descripción**:  
Este método muestra una tabla con todas las ventas registradas, organizada por departamentos y meses.

**Pasos**:
- Muestra un encabezado con los nombres de los meses.
- Luego, recorre cada departamento y muestra el monto de venta correspondiente a cada mes para ese departamento.
  
**Funcionamiento**:
- Utiliza dos bucles: el primero recorre los departamentos y el segundo recorre los meses.
- Los valores se extraen de la matriz `ventas` y se presentan en formato tabular.
- Los valores se alinean para que la tabla sea clara y fácil de leer.

