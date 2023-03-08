# Conteo-de-bits

Prrograma en c++ para desarrollar un conteo de bits
La función countBits recibe como parámetro un entero n y devuelve un vector de enteros result de longitud n+1, 
donde result[i] es el número de 1's en la representación binaria de i.

Se inicializa el primer elemento del vector como 0 y se utiliza un bucle for para recorrer los elementos del vector a partir del segundo, 
calculando su valor con la expresión: 
result[i >> 1] + (i & 1).
La primera parte de la expresión (i >> 1) equivale a dividir i entre 2 y desplazar el resultado un bit a la derecha (lo que es equivalente a eliminar el último bit de la representación binaria de i). 
La segunda parte de la expresión ((i & 1)) equivale a tomar el último bit de la representación binaria de i. 

Por lo tanto, la expresión completa equivale a contar los 1's de la representación binaria de i / 2 y sumarle el último bit de la representación binaria de i.
