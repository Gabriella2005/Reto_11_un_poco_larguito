# Reto 11

Bienvenidos a este reto con matrices, estuvo un poco tedioso pero se logró, así que los dejo con las respuestas.

### 1) Desarrolle un programa que permita realizar la suma/resta de matrices. El programa debe validar las condiciones necesarias para ejecutar la operación.

```
# Sin tener la matriz base
list = [] # creamos una lista vacia
B = []# creamos una lista vacia
global n # creamos una variable global para usarla más adelante
n = int(input("ingrese el número de filas de su matriz: \n")) #definimos n
global m # creamos una variable global para usarla más adelante
m = int(input("ingrese el número de columnas de su matriz: \n")) # definimos m
for i in range(n): #filas
    for j in range(m): #columnas
        num = int(input("ingrese los números para su matriz: \n")) #pedimos los elementos de la matriz
        list.append(num) #añadimos los elementos a la lista
    B.append(list) #añadimos las listas a la lista B
    list = []
print(B) #imprimimos B
list2 = []# creamos una lista vacia
A = []# creamos una lista vacia
p = int(input("ingrese el número de filas de su matriz 2: \n"))#definimos p
q = int(input("ingrese el número de columnas de su matriz 2: \n"))#definimos q
for h in range(p): #filas
    for l in range(q):#columnas
        nm = int(input("ingrese los números para su matriz 2: \n")) #pedimos los elementos de la matriz
        list2.append(nm) #añadimos los elementos a la lista
    A.append(list2) #añadimos las listas a la lista A
    list2 = []
print(A) #imprimimos A

def sumatriz(): #definimos la suma de matrices
    list3 = []# creamos una lista vacia
    C = []# creamos una lista vacia
    x = 0 #iniciamos en la fila 0
    y = 0 #iniciamos en la columna 0
    for o in range(n):#filas
        for t in range(m):#columnas
            suma = (A[x][y])+(B[x][y]) #definimos suma como la suma de los elementos de la misma posicion
            list3.append(suma) #añadimos los resultados a la lista
            y = y + 1 #sumamos 1 a 'y'
            if y == n: #si y es igual a los elemntos de la fila, reiniciamos 'y' en 0 y sumamos 1 a 'x'
                y = y - y
                x = x + 1
        C.append(list3) #añadimos las listas a la lista C
        list3 = []
    print(C) #imprimimos C

def resatriz(): #definimos la suma de matrices
    list3 = []# creamos una lista vacia
    C = []# creamos una lista vacia
    x = 0 #iniciamos en la fila 0
    y = 0 #iniciamos en la columna 0
    for o in range(n):#filas
        for t in range(m):#columnas
            resta = (A[x][y])-(B[x][y]) #definimos resta como la resta de los elementos de la misma posicion
            list3.append(resta) #añadimos los resultados a la lista
            y = y + 1 #sumamos 1 a 'y'
            if y == n: #si y es igual a los elemntos de la fila, reiniciamos 'y' en 0 y sumamos 1 a 'x'
                y = y - y
                x = x + 1
        C.append(list3) #añadimos las listas a la lista C
        list3 = []
    print(C) #imprimimos C

if n == p:
    if m == q:
        print('la suma de sus matrices es la siguiente: \n') #si las matrices son del mismo tamaño, realizamos la suma y resta
        sumatriz()
        print('la resta de sus matrices es la siguiente: \n')
        resatriz()
    else:
        print('las matrices ingresadas no son del mismo tamaño por lo que no se pueden operar')
else:
    print('las matrices ingresadas no son del mismo tamaño por lo que no se pueden operar')
```

### 2) Desarrolle un programa que permita realizar el producto de matrices. El programa debe validar las condiciones necesarias para ejecutar la operación.
```
```

### 3) Desarrolle un programa que permita obtener la matriz transpuesta de una matriz ingresada. El programa debe validar las condiciones necesarias para ejecutar la operación.
```
```

### 4) Desarrollar un programa que sume los elementos de una columna dada de una matriz.
```
```

### 5) Desarrollar un programa que sume los elementos de una fila dada de una matriz.
```
```
