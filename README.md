Ejercicio 2.E.2 07 - Calculadora Promocion

Lógica del programa
Para este ejercicio del Bloque IV, trabajé con el concepto de sobrecarga de métodos (Overloading). Diseñé la clase `CalculadoraPromocion` con un único atributo privado llamado `descuentoBase` (double) y su respectivo constructor.

El objetivo principal fue crear múltiples versiones de un mismo comportamiento. Para ello, implementé tres variantes del método `calcularPrecioFinal`, diferenciándolas estrictamente por su firma (la cantidad y tipo de parámetros que reciben):
1. La primera versión recibe solo el `precioBase` (double) y calcula el total aplicando el porcentaje de descuento guardado en el atributo de la instancia.
2. La segunda versión recibe el `precioBase` (double) y un `porcentajeEspecial` (double) por parámetro, aplicando este nuevo porcentaje en lugar del descuento base.
3. La tercera versión recibe el `precioBase` (double) y un `cuponFijo` (int), realizando una resta directa del monto estipulado.

Dentro de la clase `Main`, implementé la siguiente lógica de prueba:
1. Instancié un objeto `CalculadoraPromocion` definiendo un descuento base inicial del 15.0%.
2. Realicé tres impresiones por consola llamando al método `calcularPrecioFinal()`, pero en cada caso le envié argumentos distintos (primero un `double`, luego dos `double`, y finalmente un `double` junto a un `int`).
3. Al ejecutar el código, pude comprobar exitosamente cómo la JVM resuelve en tiempo de compilación qué versión específica del método debe ejecutar basándose en los argumentos proporcionados.

## Ejecución en consola
<img width="1365" height="722" alt="{0460FFED-4267-4B46-97E6-0DD13BF7EF83}" src="https://github.com/user-attachments/assets/99826432-7be7-4257-ae01-7593f5888609" />
