# RETO 4 👽

+ Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.
```python
numero_entero = int(input("Escriba un número entero: ")) # Pedir número entero, por eso con int
if numero_entero >= 97 and numero_entero <= 122: # Sí el número se encuentra entre 97 y 122 es de letras minusculas
    if numero_entero == 97 or numero_entero == 101 or numero_entero == 105 or numero_entero == 111 or numero_entero == 117: # Sí el número es 97, 101, 105, 111 o 117 es una vocal minuscula, se utiliza or ya que puede ser cualquiera verdadera
        print("El número entero dado corresponde a una vocal minúscula")
    else: # Sí no sería una consonante minuscula, es decirque no es vocal minuscula
        print("El número entero dado no corresponde a una vocal minúscula")
else: # No es letra minúscula
    print("El número entero dado no corresponde a una vocal minúscula")
```

+ Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.
```python
cadena = input("Ingrese una cadena de longitud 1: ") # Pedir cadena
ascci = ord(cadena) # El código en ASCCI de la cadena de longitud 1
if ascci % 2 == 0: # Formula para saber si el código es par
    print("El código ASCII es par")
if ascci % 2 != 0: # Formula para saber si el código es impar
    print("El código ASCII es impar")
```

+ Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.
```python
caracter = input("Ingrese un carácter: ") # Pedir caracter
# Utilizando isdigit para saber si el caracter es un dígito o no
if caracter.isdigit(): # Sí es verdadero, entonces es un dígito
    print(caracter , "es un digito")
else: # Sí no, entonces
    print(caracter , "no es un digito")
```

+ Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:

Positivo: "El número x es positivo"

Negativo: "El número x es negativo"

Cero (0): "El número x es el neutro para la suma"
```python
numero_real = float(input("Escriba un número: ")) # Pedir número real, por eso con float
if numero_real == 0: # Sí el número es igual que 0, entonces
    print("El número", numero_real, "es el neutro para la suma")
if numero_real > 0: # Sí el número es mayor que 0 es decir positivo, entonces
    print("El número", numero_real, "es positivo")
if numero_real < 0: # Sí el número es menor que 0 es decir negativo, entonces
    print("El número", numero_real, "es negativo")
```

+ Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.
```python
# Se piden los valores en flotante ya que pueden contener decimales y pueden ser negativos
# Pedir el centro (x,y) y el radio
x_centro = float(input("Ingrese la coordenada del centro en el eje x: ")) 
y_centro = float(input("Ingrese la coordenada del centro en el eje y: ")) 
radio = float(input("Ingrese el radio del circulo: ")) 
# Pedir el punto (x,y)
x_punto = float(input("Ingrese la coordenada x del punto: ")) 
y_punto = float(input("Ingrese la coordenada y del punto: ")) 
# Formula para evaluar si el punto está dentro del círculo
distancia_del_centro = ((x_punto - x_centro)**2 + (y_punto - y_centro)**2)**0.5
if distancia_del_centro <= radio: # Sí está entonces
    print("El punto está dentro del círculo")
else: # Sí no está entonces
    print("El punto está fuera del círculo")
```

+ Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.
```python
# Pedir las longitudes en flotante, ya que pueden contener decimales
longitud_uno = float(input("Ingrese la primer longitud: "))
longitud_dos = float(input("Ingrese la segunda longitud: "))
longitud_tres = float(input("Ingrese la tercera longitud: "))
# Sí la suma de dos longitudes es mayor a la otra, aplicandola en todos los casos, entonces es un tríangulo
if longitud_uno + longitud_dos > longitud_tres and longitud_uno + longitud_tres > longitud_dos and longitud_dos + longitud_tres > longitud_uno: # Con and ya que todas se deben cumplir
    print("Con esas tres longitudes se puede formar un triangulo")
# Sí no entonces
else: 
    print("Con esas longitudes no se puede formar un triangulo")
```
