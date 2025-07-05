# Adivina-el-numero
Este es un pequeño juego en Python donde el usuario debe adivinar un número secreto generado aleatoriamente entre 1 y 100.

## ¿Cómo funciona?
El programa genera un número secreto aleatorio entre 1 y 100.

El jugador introduce un número en cada intento.

El programa indica si el número ingresado es demasiado bajo, demasiado alto o correcto.

El juego termina cuando el jugador adivina el número correctamente.

## Cómo jugar
Ejecuta el script en tu consola o terminal con Python 3.

Ingresa un número entre 1 y 100 cuando se te solicite.

Sigue las indicaciones hasta adivinar el número.


## Código principal
```bash
import random

numero_secreto = random.randint(1, 100)
intento = None

while intento != numero_secreto:
    intento = int(input("Adivina el número (1-100): "))
    if intento < numero_secreto:
        print("Demasiado bajo")
    elif intento > numero_secreto:
        print("Demasiado alto")
    else:
        print("¡Correcto!")
