### EJERCICIO DE ESTRUCTURAS ###

Este archivo README describe las estructuras de datos necesarias para el ejercicio y los enunciados de los ejercicios que hayq ue hacer

A continuación, se detallan las estructuras que debes implementar: EJER

1. **`inventario` (lista de diccionarios):**  
    Una estructura para almacenar los productos en el inventario. Cada producto debe ser representado como un diccionario con las siguientes claves: `'nombre'`, `'precio'`, y `'cantidad'`. Al principio, deberá ser una lista vacía.  
    Ejemplo de cómo debería ser:  
    ```python
    [
         {'nombre': 'Camisa', 'precio': 20, 'cantidad': 40},
         {'nombre': 'Pantalón', 'precio': 30, 'cantidad': 30}
    ]
    ```

2. **`clientes` (diccionario):**  
    Una estructura para llevar un registro de los clientes de la tienda. Cada cliente debe ser representado como un diccionario con las siguientes claves: `'nombre'` y `'email'`. Al inicio, deberá ser un diccionario vacío. Además, cada cliente debe tener un historial de compras.  
    Ejemplo de cómo debería ser:  
    ```python
    {
         'Cliente1': {'email': 'cliente1@email.com', 'compras': []},
         'Cliente2': {'email': 'cliente2@email.com', 'compras': []}
    }
    ```

3. **`ventas_totales` (float):**  
    Una variable para llevar un registro de las ventas totales de la tienda. Inicialízala con el valor `0`.

### Uso del README ###

Este archivo sirve como guía para implementar las estructuras de datos necesarias en el ejercicio. Sigue las instrucciones para crear y manejar las estructuras mencionadas. Asegúrate de inicializar correctamente cada una de ellas antes de comenzar a trabajar en las funcionalidades adicionales.

#### EJERCICIOS DE EVALUACIÓN PARA EL MÓDULO 1 ###

1. `agregar_producto(nombre, precio, cantidad)`: Esta función agrega un
producto al inventario o actualiza su cantidad si ya existe. Debe recibir el
nombre, precio y cantidad del producto como parámetros.
- Itera a través del inventario y compara los nombres de los productos
con el nombre proporcionado.
- Si el producto ya existe, actualiza la cantidad.
- Si no existe, agrega un nuevo producto al inventario.
2. `ver_inventario()`: Muestra el inventario de productos con sus detalles.
- Utiliza un bucle `for` para recorrer el inventario.
- Imprime los detalles (nombre, precio, cantidad) de cada producto.
- Debería verse:
```python
Nombre: Camisa, Precio: $20, Cantidad: 50
Nombre: Pantalón, Precio: $30, Cantidad: 30
Nombre: Zapatos, Precio: $50, Cantidad: 40
Nombre: Camisa, Precio: $20, Cantidad: 50
```
ventario
4. `actualizar_stock(nombre, cantidad)`: Actualiza el stock de un producto
en el inventario. Debe recibir el nombre del producto y la cantidad a
agregar o quitar como parámetros.
- Utiliza un bucle `for` para recorrer el inventario.
- Busca el producto por nombre.
2 / 6
evaluacion-final-pt.md 2024-10-07
- Actualiza la cantidad según la entrada del usuario.
- Si el producto no esta en el inventario muestra un mensaje
indicándolo.
5. `eliminar_producto(nombre)`: Elimina un producto del inventario por
nombre. Debe recibir el nombre del producto como parámetro.
- Utiliza un bucle `for` para recorrer el inventario.
- Busca el producto por nombre.
- Elimina el producto del inventario si existe.
- Si el producto no esta en el inventario muestra un mensaje
indicándolo.
6. `calcular_valor_inventario()`: Calcula y muestra el valor total del
inventario.
- Utiliza un bucle for para calcular el valor total del inventario.
- Itera a través del inventario y suma el valor de cada producto
(precio x cantidad). Es decir, calcula el valor total del inventario.
Ejemplo:
```python
# si tenemos 5 camisas que valen 5 euros
# y 10 calcetines que valen 1 euro
# este método te tiene que devolver: 35 euros
valor_camisas = 5 * 5
valor_calcetines = 10 * 1
valor_camisas + valor_calcetines = 35
```
7. `realizar_compra()`: Permite a un cliente realizar una compra
seleccionando productos del inventario. Debe interactuar con el cliente para
seleccionar productos y calcular el costo total de la compra.
- Utiliza un bucle `while` para permitir al cliente realizar múltiples
compras.
- Muestra el inventario y solicita al cliente ingresar el nombre del
producto que desea comprar.
- Registra los productos seleccionados en un carrito y actualiza el
inventario.
3 / 6git restore
evaluacion-final-pt.md 2024-10-07
- Calcula el costo total de la compra.