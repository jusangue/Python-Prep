## Estructuras de Datos

1) Crear una lista que contenga nombres de ciudades del mundo que contenga más de 5 elementos e imprimir por pantalla

ciudades = ['Maracaibo', 'Bogota', 'Buenos Aires', 'Stanbul', 'Tokyo']
print(ciudades)

2) Imprimir por pantalla el segundo elemento de la lista

print(ciudades[1])

3) Imprimir por pantalla del segundo al cuarto elemento

print(ciudades[1:4])

4) Visualizar el tipo de dato de la lista

print(type(ciudades[2]))

5) Visualizar todos los elementos de la lista a partir del tercero de manera genérica, es decir, sin explicitar la posición del último elemento

print(ciudades[2:])

6) Visualizar los primeros 4 elementos de la lista

print(ciudades[:4])

7) Agregar una ciudad más a la lista que ya exista y otra que no ¿Arroja algún tipo de error?

ciudades = ['Maracaibo', 'Bogota', 'Buenos Aires', 'Stanbul', 'Tokyo', 'Tokyo', 'Venecia'] #ningun error

8) Agregar otra ciudad, pero en la cuarta posición

ciudades.insert(3,'Mexico city')

9) Concatenar otra lista a la ya creada

ciudades.extend(['Barranquilla','Medellin'])

10) Encontrar el índice de la ciudad que en el punto 7 agregamos duplicada. ¿Se nota alguna particularidad?

print(ciudades.index('Tokyo')) #nos da el indice de la primera coincidencia que aparece, es decir la que este primero, en mi caso es el index 4 y 5 es el duplicado, pero solo me da el 4.

11) ¿Qué pasa si se busca un elemento que no existe?

print(ciudades.index('Bucaramanga')) #nos dira que lo que estamos buscando no esta en la lista

12) Eliminar un elemento de la lista

ciudades.remove('Bogota')

13) ¿Qué pasa si el elemento a eliminar no existe?

ciudades.remove('Bucaramanga') #nos dara un error y este dira que el elemento no esta en la lista

14) Extraer el úlimo elemento de la lista, guardarlo en una variable e imprimirlo

ultima_ciudad = ciudades.pop()
print(ultima_ciudad)

15) Mostrar la lista multiplicada por 4

print(ciudades * 4)

16) Crear una tupla que contenga los números enteros del 1 al 20

mi_tupla = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20,)

17) Imprimir desde el índice 10 al 15 de la tupla

print(mi_tupla[10:16])

18) Evaluar si los números 20 y 30 están dentro de la tupla

print(20 in mi_tupla)
print(30 in mi_tupla)

19) Con la lista creada en el punto 1, validar la existencia del elemento 'París' y si no existe, agregarlo. Utilizar una variable e informar lo sucedido.

if ('paris' in ciudades):
    print('ya esta en ciudades')
else:
    ciudades.append('paris')
    print(ciudades.index('paris'))
    print(ciudades[5])

20) Mostrar la cantidad de veces que se encuentra un elemento específico dentro de la tupla y de la lista

ciudades.count('Bogota')
mi_tupla.count('2')

21) Convertir la tupla en una lista

mi_tupla1 = list(mi_tupla)

22) Desempaquetar solo los primeros 3 elementos de la tupla en 3 variables

numero1, numero2, numero3 = mi_tupla[:3]
print(numero1, numero2, numero3)

23) Crear un diccionario utilizando la lista crada en el punto 1, asignandole la clave "ciudad". Agregar tambien otras claves, como puede ser "Pais" y "Continente".

diccio = {'ciudades':[ciudades], 'pais':[''], 'continente': ['']}

24) Imprimir las claves del diccionario

print(diccio.keys())

25) Imprimir las ciudades a través de su clave

print(diccio['ciudades']) #imprime todas
