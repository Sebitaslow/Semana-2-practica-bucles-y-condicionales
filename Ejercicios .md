# Semana-2-practica-bucles-y-condicionales
- Ejercicio 1
Clasificador de números Escribe un programa que pida al usuario un número entero y determine si es positivo, negativo o cero.

```python
Numero_entero = (int(input("Escribe un numero o sino eres parangaricutimicuaro: ")))
if Numero_entero >0:
    print("El numero es positivo :D")
elif Numero_entero <0:
    print ("El numero es negativo D:")
else:
    print ("El numero es 0 :b")
```
- Ejercicio 2
Aprobado o reprobado Crea un programa que reciba la calificación de un estudiante (0 a 100) e indique si está aprobado (60 o más) o reprobado (menos de 60).

```python
calificacion = int(input("Ingresa tu calificaciÃ³n de 0 a 100: "))
if calificacion >=60 and calificacion <=100:
    print("Aprobado")
else:
    if calificacion < 60:
      print("Reprobado")
```
- Ejercicio 3
Tabla de multiplicar Escribe un programa que muestre la tabla de multiplicar de un número ingresado por el usuario (del 1 al 10) usando un bucle for.

```python
# Pedir al usuario que ingrese el número que quiere multiplicar
Numero_multiplicar = int( input("Escribe un numero que te guistaria multiplicar: "))
# Realizar la multiplicación con los números del 1 al 10
for Numero_multiplica in range (1, 11):
    resultado = Numero_multiplicar * Numero_multiplica #Se crea una multiplicación que va desde 1 a 10
    print (f"{Numero_multiplicar}  X  {Numero_multiplica}  =  {resultado}")

```
- Ejercicio 4
Contador regresivo Crea un programa que pida un número positivo al usuario y haga una cuenta regresiva desde ese número hasta 0 usando un bucle while.

```python
import time # Se importa el tiempo para que sea mas lento el programa
# Pedir al usuario un número positivo
Numero_positivo = int (input("Pon un número positivo entero para generar una cuenta regresiva: "))

# Verificar que el número sea positivo
if Numero_positivo >0:
    while Numero_positivo >=0:
        print(Numero_positivo)
        time.sleep(1)
        Numero_positivo -= 1 
        #Este bucle finaliza hasta que el numero puesto sea 0 atra vez de la resta del numero 
else:
    print("¡Por favor, ingresa un número positivo!") 
    #Con esto si el numero es negativo no daria
```
- Ejercicio 5
Adivina el número Crea un programa que genere un número aleatorio entre 1 y 10, y le pida al usuario que lo adivine. El programa debe indicar si el número ingresado es mayor, menor o correcto. El usuario tiene hasta 3 intentos.


```python
import random

# Generar el número aleatorio entre 1 y 10
numero_aleatorio = random.randint(1, 10)

# Número de intentos
intentos = 3

print("¡Bienvenido al juego Adivina el número!")
print("He generado un número entre 1 y 10. Tienes 3 intentos para adivinarlo.")

# Bucle para los intentos
for intento in range(1, intentos + 1):
    # Pedir al usuario que ingrese un número
    adivinanza = int(input(f"Intento {intento}: ¿Cuál es tu número? "))

    # Comprobar si el número es mayor, menor o correcto
    if adivinanza < numero_aleatorio:
        print("¡El número es mayor!")
    elif adivinanza > numero_aleatorio:
        print("¡El número es menor!")
    else:
        print(f"¡Felicidades! Has adivinado el número {numero_aleatorio} en {intento} intentos.")
        break
else:
    print(f"Lo siento, no has adivinado el número. El número correcto era {numero_aleatorio}.")
```
