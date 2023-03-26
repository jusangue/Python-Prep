## Variables

1 Crear una variable que contenga un elemento del conjunto de números enteros y luego imprimir por pantalla

a = 100
print(a)

2 Imprimir el tipo de dato de la constante 8.5

b = 8.5
print(type(b))

3 Imprimir el tipo de dato de la variable creada en el punto 1

print(type(a))

4 Crear una variable que contenga tu nombre

Nombre = 'Julian Santos'

5 Crear una variable que contenga un número complejo

Numcomplejo = 3 - 45j

6 Mostrar el tipo de dato de la variable crada en el punto 5

print(type(Numcomplejo))

7 Crear una variable que contenga el valor del número Pi redondeado a 4 decimales

pi = 3.1416

8 Crear una variable que contenga el valor 'True' y otra que contenga el valor True. ¿Se trata de lo mismo?

var1 = 'True'
var2 = True
Diferentes, var1 es str y var2 es bool

9 Imprimir el tipo de dato correspondientes a las variables creadas en el punto 8

print(type(var1))
print(type(var2))

10 Asignar a una variable, la suma de un número entero y otro decimal

res10 = 10 + 25.4

11 Realizar una operación de suma de números complejos

comsum = 4j + 10j

12 Realizar una operación de suma de un número real y otro complejo

realcom = 10.5 + 50j

13 Realizar una operación de multiplicación

multi = 4 * 5

14 Mostrar el resultado de elevar 2 a la octava potencia

elevar = 2 ** 8
print(elevar)

15 Obtener el cociente de la división de 27 entre 4 en una variable y luego mostrarla

cociente = 27 / 4
print(cociente)

16 De la división anterior solamente mostrar la parte entera

cociente1 = 27 // 4
print(cociente1)

17 De la división de 27 entre 4 mostrar solamente el resto

cociente2 = 27 % 4
print(cociente2)

18 Utilizando como operandos el número 4 y los resultados obtenidos en los puntos 16 y 17. Obtener 27 como resultado

6 * 4 + 3

19 Utilizar el operador "+" en una operación donde intervengan solo variables alfanuméricas

print(Nombre + var1)

20 Evaluar si "2" es igual a 2. ¿Por qué ocurre eso?

2 == '2'  por que las 2 no son de el mismo tipo por ende da falso

21 Utilizar las funciones de cambio de tipo de dato, para que la validación del punto 20 resulte verdadera

2 == in('2')

22 ¿Por qué arroja error el siguiente cambio de tipo de datos? a = float('3,8')

Por que no pudo convertir una variable str a una float, esto podria ser debido a que no es un numero int o real.

23 Crear una variable con el valor 3, y utilizar el operador '-=' para modificar su contenido

c = 3
c -= 1

24 Realizar la operacion 1 << 2 ¿Por qué da ese resultado? ¿Qué es el sistema de numeración binario?



25 Realizar la operación 2 + '2' ¿Por qué no está permitido? ¿Si los dos operandos serían del mismo tipo, siempre arrojaría el mismo resultado?

2 + '2'
float(2) + float('2')
int(2) + int('2')
str(2) + str('2')

26 Realizar una operación válida entre valores de tipo entero y string

var1 = 'este texto se repite '
var2 = 3
print(var1 * var2 + str(var2) + ' veces')