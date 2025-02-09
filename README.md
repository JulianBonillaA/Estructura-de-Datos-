# Departamento de Ventas

Este es un programa en Python que simula el manejo de ventas de diferentes departamentos a lo largo de los meses del año. El programa permite insertar, buscar, eliminar ventas y mostrar una tabla con todas las ventas registradas.

## Funcionalidades

- **Insertar venta**: Permite ingresar un monto de ventas para un departamento específico en un mes específico.
- **Buscar venta**: Permite consultar el monto de ventas registrado para un departamento y mes seleccionados.
- **Eliminar venta**: Permite eliminar una venta (poniendo el monto a 0.0) para un departamento y mes seleccionados.
- **Mostrar tabla de ventas**: Muestra una tabla con todas las ventas registradas, organizada por departamentos y meses.

## Estructura de Datos

- **Meses**: Un arreglo que contiene los 12 meses del año.
- **Departamentos**: Un arreglo con los departamentos disponibles ("Ropa", "Deportes", "Juguetería").
- **Ventas**: Una matriz (arreglo bidimensional) donde se almacenan las ventas de cada departamento para cada mes. Cada fila representa un departamento y cada columna representa un mes.

## Requisitos

- Python 3.x
- No se requieren dependencias externas.

## Cómo usar el programa

1. **Ejecutar el programa**:
   - Para ejecutar el programa, solo debes ejecutar el archivo `departamentos.py` en tu terminal o entorno de desarrollo.

2. **Interacción**:
   - Al ejecutar el programa, se te presentará un menú de opciones. Puedes seleccionar una de las siguientes opciones:
     - **1. Insertar venta**: Permite ingresar un monto de venta para un departamento y mes específicos.
     - **2. Buscar venta**: Permite consultar una venta registrada.
     - **3. Eliminar venta**: Permite eliminar (poner a 0) una venta.
     - **4. Mostrar tabla de ventas**: Muestra todas las ventas registradas en una tabla organizada por departamento y mes.
     - **5. Salir**: Termina el programa.

3. **Ejemplo de interacción**:

   ```text
   --- Menú de opciones ---
   1. Insertar venta
   2. Buscar venta
   3. Eliminar venta
   4. Mostrar tabla de ventas
   5. Salir
   Seleccione una opción: 1
   
   Departamentos disponibles: Ropa, Deportes, Juguetería
   Ingrese el departamento: Ropa
   
   Meses disponibles: Enero, Febrero, Marzo, ...
   Ingrese el mes: Enero
   
   Ingrese el monto de ventas: 500.0
   Venta de 500.0 insertada en Ropa para el mes de Enero.

