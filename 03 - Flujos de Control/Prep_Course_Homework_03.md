## Flujos de Control

1) Crear una variable que contenga un elemento del conjunto de números enteros y luego imprimir por pantalla si es mayor o menor a cero

a = 10
if (a < 0):
    print(a, 'es menor que cero')
elif (a > 0):
    print(a, 'es mayor que cero')
else:
    print(a, 'es igual a cero')

2) Crear dos variables y un condicional que informe si son del mismo tipo de dato

b = True
c = 'True'
if (type(b) == type(c)):
    print('b y c son iguales')
else:
    print('b y c no son iguales')

3) Para los valores enteros del 1 al 20, imprimir por pantalla si es par o impar

a = 0
for a in range(1,21):
    if (a % 2 == 0):
        print(a, 'es un numero par')
    else:
        print(a, 'es un numero impar')

4) En un ciclo for mostrar para los valores entre 0 y 5 el resultado de elevarlo a la potencia igual a 3

for i in range(0, 6):
    print('Valor:', str(i), 'Elevado a la 3ra potencia:', str(i**3))

5) Crear una variable que contenga un número entero y realizar un ciclo for la misma cantidad de ciclos

f = 10
for f in range(0, f):
    print('ciclo', f)
    pass

6) Utilizar un ciclo while para realizar el factorial de un número guardado en una variable, sólo si la variable contiene un número entero mayor a 0

numero = 4
factorial = 1
while(numero > 1):
    factorial = numero * factorial
    print(factorial)
    numero = numero - 1

7) Crear un ciclo for dentro de un ciclo while

n = 0
while(n < 5):
    for i in range(1,n):
        print('Ciclo while nro ' + str(n))
        print('Ciclo for nro ' + str(i))
    
    n += 1

8) Crear un ciclo while dentro de un ciclo for

n = 5
for i in range(1, n):
    while(n < 5):
        n -= 1
        print('Ciclo while nro ' + str(n))
        print('Ciclo for nro ' + str(i))

9) Imprimir los números primos existentes entre 0 y 30

min = 1
max = 30
for n in range(min, (max + 1)):
    primo = True
    j = 2
    while(j < n):
        if (n % j == 0):
            primo = False
            break
        j += 1
    if (primo):
        print('El número', n, 'es primo')

10) ¿Se puede mejorar el proceso del punto 9? Utilizar las sentencias break y/ó continue para tal fin

n = 0
primo = True
while (n < tope_rango):
    for div in range(2, n):
        if (n % div == 0):
            primo = False
            break
    if (primo):
        print(n)
    else:
        primo = True
    n += 1

11) En los puntos 9 y 10, se diseño un código que encuentra números primos y además se lo optimizó. ¿Es posible saber en qué medida se optimizó?

ciclos_con_break = 0
n = 0
primo = True
while (n < tope_rango):
    for div in range(2, n):
        ciclos_con_break += 1
        if (n % div == 0):
            primo = False
            break
    if (primo):
        print(n)
    else:
        primo = True
    n += 1
print('Cantidad de ciclos: ' + str(ciclos_con_break))
print('Se optimizó a un ' + str(ciclos_con_break/ciclos_sin_break) + '% de ciclos aplicando break')

12) Si la cantidad de números que se evalúa es mayor a treinta, esa optimización crece?

ciclos_con_break = 0
n = 0
primo = True
while (n < tope_rango):
    for div in range(2, n):
        ciclos_con_break += 1
        if (n % div == 0):
            primo = False
            break
    if (primo):
        print(n)
    else:
        primo = True
    n += 1
print('Cantidad de ciclos: ' + str(ciclos_con_break))
print('Se optimizó a un ' + str(ciclos_con_break/ciclos_sin_break) + '% de ciclos aplicando break')

13) Aplicando continue, armar un ciclo while que solo imprima los valores divisibles por 12, dentro del rango de números de 100 a 300

n = 99
while(n <= 300):
    n+=1
    if (n % 12 != 0):
        continue
    print(n, ' es divisible por 12')

14) Utilizar la función **input()** que permite hacer ingresos por teclado, para encontrar números primos y dar la opción al usario de buscar el siguiente

n = 1
sigue = 1
primo = True
while (sigue == 1):
    for div in range(2, n):
        if (n % div == 0):
            primo = False
            break
    if (primo):
        print(n)
        print('¿Desea encontrar el siguiente número primo?')
        if (input() != '1'):
            print('Se finaliza el proceso')
            break
    else:
        primo = True
    n += 1

15) Crear un ciclo while que encuentre dentro del rango de 100 a 300 el primer número divisible por 3 y además múltiplo de 6

n = 100
while(n<=300):
    if (n % 6 == 0):
        print('El número es: ', str(n))
        break
    n += 1