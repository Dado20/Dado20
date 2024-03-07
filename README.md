import random

def jugar_adivinanza():
    numero_secreto = random.randint(1, 100)
    intentos_realizados = 0

    print("¡Bienvenido a Adivina el Número!")
    print("Estoy pensando en un número entre 1 y 100. ¿Puedes adivinar cuál es?")

    while True:
        suposicion = int(input("Introduce tu suposición: "))
        intentos_realizados += 1

        if suposicion < numero_secreto:
            print("Tu suposición es demasiado baja. Inténtalo de nuevo.")
        elif suposicion > numero_secreto:
            print("Tu suposición es demasiado alta. Inténtalo de nuevo.")
        else:
            print("¡Felicidades! ¡Adivinaste el número en", intentos_realizados, "intentos!")
            break

jugar_adivinanza()
