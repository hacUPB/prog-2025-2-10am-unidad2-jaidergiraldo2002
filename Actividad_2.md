# Simbolos basicos de un diagrama de flujo
    Ovalado: Símbolo de Inicio / Final
El símbolo de terminación marca el punto inicial o final del sistema. Por lo general, contiene la palabra "Inicio" o "Fin".

    Retangular: Símbolo de Acción o Proceso
Un rectangulo solo puede representar un solo paso dentro de un processo ("agregar dos tazas de harina"), o un subproceso completo ("hacer pan") dentro de un proceso más grande.

    Rombo: Símbolo de Decisión o Ramificación
Un punto de decisión o ramificación. Las líneas que representan diferentes decisiones surgen de diferentes puntos del diamante.

    Trapecio: Símbolo de Entrada / Salida
Representa el material o la información que entra o sale del sistema, como una orden del cliente (entrada) o un producto (salida).

    Circulo: Símbolo del Conector
Indica que el flujo continúa donde se ha colocado un símbolo identico (que contiene la misma letra).




# ejercicio 2:
    construye un algoritmo que, al recibir como datos el ID del empleado y los seis primeros digitos del sueldo del, calcule el ingreso total semestral y el promedio mensual, e imprima el ID del empleado, el ingreso total y el promedio mensual.

# solucion:

# pseudocodigo:


```
     Inicio
     Leer ID, S1, S2, S3, S4, S6
     Total = S1+S2+S3+S4+S5+S6
     Promedio = Total / 6
     Escribir: ID, Total, Promedio
     Fin
```

# imagenes: 
    [Actividad_2](/imagenes/Diagrama-de-flujo.PNG)
# ejercicio 3:

Realice un algoritmo para determinar cuánto se debe pagar por equis cantidad de lápices considerando que si son 1000 o más el costo es de $85 cada uno; de lo contrario, el precio es de $90. Represéntelo con el pseudocódigo y el diagrama de flujo.

| Variables | Tipo |
|---------|-----|
|Lapices |Entrada|
|Precio | Salida|
|85, 90 | Constantes|

## pseudocodigo:

```
Inicio
Leer Lapices
Si Lapices >= 1000:
    valor_unidad = 85
Sino 
    valor_unidad = 90
Fin Si
Precio = Lapices * valor_unidad
Escribir "El valor total es:", Precio
Fin
```
# ejercicio 4:

Un almacén de ropa tiene una promoción: por compras superiores a $250 000 se les aplicará un descuento de 15%, de caso contrario, sólo se aplicará un 8% de descuento. Realice un algoritmo para determinar el precio final que debe pagar una persona por comprar en dicho almacén y de cuánto es el descuento que obtendrá. Represéntelo mediante el pseudocódigo y el diagrama de flujo.

# Analisis: 
| Variables | Tipo | Comentario |
|-----------|------|------------------|
|total_compra| Entrada | Valor de la compra|
|descuento|Salida|Descuento total segun el valor de la compra|
|precio_final|Salida|Valor a pagar|
|15%, 8%, $250000| Constantes | Descuentos y valor limite|

# Pseudocodigo:
```
Inicio
Leer total_compra
Si total_compra > 250000:
    descuento = total_compra*0.15
Si no
    descuento = total_compra*0.08
Fin Si
precio_final = total_compra - descuento
Escribir precio_final
Fin
```
# ejercicio 5:

El director de una escuela está organizando un viaje de estudios, y requiere determinar cuánto debe cobrar a cada alumno y cuánto debe pagar a la compañía de viajes por el servicio. La forma de cobrar es la siguiente: si son 100 alumnos o más, el costo por cada alumno es de $65.00; de 50 a 99 alumnos, el costo es de $70.00, de 30 a 49, de $95.00, y si son menos de 30, el costo de la renta del autobús es de $4000.00, sin importar el número de alumnos.

# Analisis:
| Variables | Tipo | Comentario|
|-----------|------|-----------|
|cantidad_alumnos|Entrada|Numero de alumnos|
|costo_alumno|Salida|Precio por alumno|
|precio_total|Salida|Precio total a pagar segun la cantidad de alumnos|
|100, [50-99], [30-49], [0-29]|Constante|Rango del # de alumnos|
|$65, $70, $95, $4000| Constantes| Costo por alumno o costo total |

# Pseudocodigo:
```
Inicio
Leer cantidad_alumnos
Si cantidad_alumnos >= 100
    costo_alumno = 65
    precio_total = costo_alumno*cantidad_alumnos
Si no
    Si cantidad_alumnos >= 50
        costo_alumno = 70
        precio_total = costo_alumno*cantidad_alumnos
    Si no 
        Si cantidad_alumnos >= 30
            costo_alumno = 90
            precio_total = costo_alumno*cantidad_alumnos
        Si no
            precio_total = 4000
            costo_alumno = precio_total/cantidad_alumnos
        Fin Si
    Fin Si
Fin Si
Escribir "El precio total de la renta seria: ", precio_total, " y el precio por alumno: ", costo-alumno
Fin  

```