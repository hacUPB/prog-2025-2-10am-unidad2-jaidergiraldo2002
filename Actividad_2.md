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
```
     Inicio
     Leer ID, S1, S2, S3, S4, S6
     Total = S1+S2+S3+S4+S5+S6
     Promedio = Total / 6
     Escribir: ID, Total, Promedio
     Fin
```