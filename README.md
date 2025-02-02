# tarea_independiente.py
# tarea_independiente
# ejercicio_1

### main.py

```python
import math

def temperatura(t, T0=5, Ts=40, k=0.45):
    return Ts + (T0 - Ts) * math.exp(-k * t)

def tiempo_para_temp_deseada(Td, T0=5, Ts=40, k=0.45):
    return -(math.log((Td - Ts) / (T0 - Ts)) / k)

if __name__ == "__main__":
    # Temperaturas a las 1, 5, 12 y 14 horas
    for horas in [1, 5, 12, 14]:
        print(f"Temperatura después de {horas} horas: {temperatura(horas):.2f} ºC")

    # Tiempo para que la temperatura sea 0.5ºC menos que la temperatura ambiente
    Td = Ts - 0.5
    tiempo = tiempo_para_temp_deseada(Td)
    print(f"Tiempo para alcanzar {Td} ºC: {tiempo:.2f} horas")
```

### Rama 1: `temperatura_horas`

```python
import math

def temperatura(t, T0=5, Ts=40, k=0.45):
    return Ts + (T0 - Ts) * math.exp(-k * t)

if __name__ == "__main__":
    # Temperaturas a las 1, 5, 12 y 14 horas
    for horas in [1, 5, 12, 14]:
        print(f"Temperatura después de {horas} horas: {temperatura(horas):.2f} ºC")
```

### Rama 2: `tiempo_para_temp_deseada`

```python
import math

def tiempo_para_temp_deseada(Td, T0=5, Ts=40, k=0.45):
    return -(math.log((Td - Ts) / (T0 - Ts)) / k)

if __name__ == "__main__":
    # Tiempo para que la temperatura sea 0.5ºC menos que la temperatura ambiente
    Td = Ts - 0.5
    tiempo = tiempo_para_temp_deseada(Td)
    print(f"Tiempo para alcanzar {Td} ºC: {tiempo:.2f} horas")
```

### Rama 3: `funciones_generales`

```python
import math

def temperatura(t, T0=5, Ts=40, k=0.45):
    return Ts + (T0 - Ts) * math.exp(-k * t)

def tiempo_para_temp_deseada(Td, T0=5, Ts=40, k=0.45):
    return -(math.log((Td - Ts) / (T0 - Ts)) / k)

if __name__ == "__main__":
    # Temperaturas a las 1, 5, 12 y 14 horas
    for horas in [1, 5, 12, 14]:
        print(f"Temperatura después de {horas} horas: {temperatura(horas):.2f} ºC")

    # Tiempo para que la temperatura sea 0.5ºC menos que la temperatura ambiente
    Td = Ts - 0.5
    tiempo = tiempo_para_temp_deseada(Td)
    print(f"Tiempo para alcanzar {Td} ºC: {tiempo:.2f} horas")
```

# ejercicio_2

### main.py

```python
def calcular_letra_dni(dni):
    letras = "TRWAGMYFPDXBNJZSQVHLCKE"
    return letras[dni % 23]

if __name__ == "__main__":
    # Solicitar número de DNI al usuario
    dni = int(input("Introduce el número de DNI: "))
    letra = calcular_letra_dni(dni)
    print(f"La letra del DNI es: {letra}")
```

### Rama 1: `calculo_dni`

```python
def calcular_letra_dni(dni):
    letras = "TRWAGMYFPDXBNJZSQVHLCKE"
    return letras[dni % 23]

if __name__ == "__main__":
    # Solicitar número de DNI al usuario
    dni = int(input("Introduce el número de DNI: "))
    letra = calcular_letra_dni(dni)
    print(f"La letra del DNI es: {letra}")
```

### Rama 2: `funcion_dni`

```python
def calcular_letra_dni(dni):
    letras = "TRWAGMYFPDXBNJZSQVHLCKE"
    return letras[dni % 23]
```

### Rama 3: `main_dni`

```python
if __name__ == "__main__":
    # Solicitar número de DNI al usuario
    dni = int(input("Introduce el número de DNI: "))
    letra = calcular_letra_dni(dni)
    print(f"La letra del DNI es: {letra}")

def calcular_letra_dni(dni):
    letras = "TRWAGMYFPDXBNJZSQVHLCKE"
    return letras[dni % 23]
```

# ejercicio_3

### main.py

```python
def calcular_letra_dni(dni):
    letras = "TRWAGMYFPDXBNJZSQVHLCKE"
    return letras[dni % 23]

def calcular_pi(n=200):
    pi = 0
    for k in range(1, n + 1):
        pi += ((-1) ** (k + 1)) / (2 * k - 1)
    return 4 * pi

if __name__ == "__main__":
    # Parte 1: Cálculo de la letra del DNI
    dni = int(input("Introduce el número de DNI: "))
    letra = calcular_letra_dni(dni)
    print(f"La letra del DNI es: {letra}")

    # Parte 2: Cálculo de π
    pi_valor = calcular_pi()
    print(f"Valor aproximado de π: {pi_valor:.6f}")
```

### Rama 1: `calculo_dni`

```python
def calcular_letra_dni(dni):
    letras = "TRWAGMYFPDXBNJZSQVHLCKE"
    return letras[dni % 23]

if __name__ == "__main__":
    # Parte 1: Cálculo de la letra del DNI
    dni = int(input("Introduce el número de DNI: "))
    letra = calcular_letra_dni(dni)
    print(f"La letra del DNI es: {letra}")
```

### Rama 2: `calculo_pi`

```python
def calcular_pi(n=200):
    pi = 0
    for k in range(1, n + 1):
        pi += ((-1) ** (k + 1)) / (2 * k - 1)
    return 4 * pi

if __name__ == "__main__":
    # Parte 2: Cálculo de π
    pi_valor = calcular_pi()
    print(f"Valor aproximado de π: {pi_valor:.6f}")
```

### Rama 3: `funciones_generales`

```python
def calcular_letra_dni(dni):
    letras = "TRWAGMYFPDXBNJZSQVHLCKE"
    return letras[dni % 23]

def calcular_pi(n=200):
    pi = 0
    for k in range(1, n + 1):
        pi += ((-1) ** (k + 1)) / (2 * k - 1)
    return 4 * pi

if __name__ == "__main__":
    # Parte 1: Cálculo de la letra del DNI
    dni = int(input("Introduce el número de DNI: "))
    letra = calcular_letra_dni(dni)
    print(f"La letra del DNI es: {letra}")

    # Parte 2: Cálculo de π
    pi_valor = calcular_pi()
    print(f"Valor aproximado de π: {pi_valor:.6f}")
```

# ejercicio_4

### main.py

```python
def fibonacci(n):
    secuencia = [0, 1]
    while len(secuencia) < n:
        secuencia.append(secuencia[-1] + secuencia[-2])
    return secuencia

if __name__ == "__main__":
    # Número de términos deseados
    n = int(input("Introduce el número de términos de la sucesión de Fibonacci: "))
    print("Sucesión de Fibonacci:", fibonacci(n))
```

### Rama 1: `funcion_fibonacci`

```python
def fibonacci(n):
    secuencia = [0, 1]
    while len(secuencia) < n:
        secuencia.append(secuencia[-1] + secuencia[-2])
    return secuencia
```

### Rama 2: `main_fibonacci`

```python
if __name__ == "__main__":
    def fibonacci(n):
        secuencia = [0, 1]
        while len(secuencia) < n:
            secuencia.append(secuencia[-1] + secuencia[-2])
        return secuencia

    # Número de términos deseados
    n = int(input("Introduce el número de términos de la sucesión de Fibonacci: "))
    print("Sucesión de Fibonacci:", fibonacci(n))
```

### Rama 3: `calculo_fibonacci`

```python
def fibonacci(n):
    secuencia = [0, 1]
    while len(secuencia) < n:
        secuencia.append(secuencia[-1] + secuencia[-2])
    return secuencia

if __name__ == "__main__":
    # Número de términos deseados
    n = int(input("Introduce el número de términos de la sucesión de Fibonacci: "))
    print("Sucesión de Fibonacci:", fibonacci(n))
```
# ejercicio_5
 
 ### main.py

```python
if __name__ == "__main__":
    # Genera la lista con el cuadrado de los números pares y el cubo de los impares
    lista = [(i**2 if i % 2 == 0 else i**3) for i in range(1, 101)]
    suma_total = 0
    contador = 0

    # Calcula cuantos números se deben sumar para que el resultado sea cercano a un millón
    for numero in lista:
        if suma_total + numero < 1000000:
            suma_total += numero
            contador += 1
        else:
            break

    print(f"Se suman {contador} números para alcanzar la suma más cercana a un millón, que es {suma_total}")
```

### Rama 1: `generar_lista`

```python
if __name__ == "__main__":
    # Genera la lista con el cuadrado de los números pares y el cubo de los impares
    lista = [(i**2 if i % 2 == 0 else i**3) for i in range(1, 101)]
    print("Lista generada:", lista)
```

### Rama 2: `calcular_suma`

```python
if __name__ == "__main__":
    # Genera la lista con el cuadrado de los números pares y el cubo de los impares
    lista = [(i**2 if i % 2 == 0 else i**3) for i in range(1, 101)]
    suma_total = 0
    contador = 0

    # Calcula cuantos números se deben sumar para que el resultado sea cercano a un millón
    for numero in lista:
        if suma_total + numero < 1000000:
            suma_total += numero
            contador += 1
        else:
            break

    print(f"Se suman {contador} números para alcanzar la suma más cercana a un millón, que es {suma_total}")
```

### Rama 3: `funciones_generales`

```python
if __name__ == "__main__":
    # Genera la lista con el cuadrado de los números pares y el cubo de los impares
    lista = [(i**2 if i % 2 == 0 else i**3) for i in range(1, 101)]
    suma_total = 0
    contador = 0

    # Calcula cuantos números se deben sumar para que el resultado sea cercano a un millón
    for numero in lista:
        if suma_total + numero < 1000000:
            suma_total += numero
            contador += 1
        else:
            break

    print(f"Se suman {contador} números para alcanzar la suma más cercana a un millón, que es {suma_total}")
```

# ejercicio_6

### main.py

```python
def desglose_euros(cantidad):
    billetes_monedas = [500, 200, 100, 50, 20, 10, 5, 2, 1]
    desglose = {}
    for valor in billetes_monedas:
        if cantidad >= valor:
            desglose[valor] = cantidad // valor
            cantidad %= valor
    return desglose

if __name__ == "__main__":
    # Solicitar cantidad al usuario y comprobar que es un número entero
    try:
        cantidad = int(input("Introduce la cantidad en euros: "))
        desglose = desglose_euros(cantidad)
        print("Desglose en billetes y monedas:")
        for valor, cantidad in desglose.items():
            print(f"{cantidad} de {valor}€")
    except ValueError:
        print("Por favor, introduce un número entero válido.")
```

### Rama 1: `desglose_euros`

```python
def desglose_euros(cantidad):
    billetes_monedas = [500, 200, 100, 50, 20, 10, 5, 2, 1]
    desglose = {}
    for valor in billetes_monedas:
        if cantidad >= valor:
            desglose[valor] = cantidad // valor
            cantidad %= valor
    return desglose
```

### Rama 2: `solicitar_cantidad`

```python
if __name__ == "__main__":
    # Solicitar cantidad al usuario y comprobar que es un número entero
    try:
        cantidad = int(input("Introduce la cantidad en euros: "))
        desglose = desglose_euros(cantidad)
        print("Desglose en billetes y monedas:")
        for valor, cantidad in desglose.items():
            print(f"{cantidad} de {valor}€")
    except ValueError:
        print("Por favor, introduce un número entero válido.")

def desglose_euros(cantidad):
    billetes_monedas = [500, 200, 100, 50, 20, 10, 5, 2, 1]
    desglose = {}
    for valor in billetes_monedas:
        if cantidad >= valor:
            desglose[valor] = cantidad // valor
            cantidad %= valor
    return desglose
```

### Rama 3: `funciones_generales`

```python
def desglose_euros(cantidad):
    billetes_monedas = [500, 200, 100, 50, 20, 10, 5, 2, 1]
    desglose = {}
    for valor in billetes_monedas:
        if cantidad >= valor:
            desglose[valor] = cantidad // valor
            cantidad %= valor
    return desglose

if __name__ == "__main__":
    # Solicitar cantidad al usuario y comprobar que es un número entero
    try:
        cantidad = int(input("Introduce la cantidad en euros: "))
        desglose = desglose_euros(cantidad)
        print("Desglose en billetes y monedas:")
        for valor, cantidad in desglose.items():
            print(f"{cantidad} de {valor}€")
    except ValueError:
        print("Por favor, introduce un número entero válido.")
```


