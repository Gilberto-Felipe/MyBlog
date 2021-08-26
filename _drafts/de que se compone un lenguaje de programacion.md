---
layout: post
title: "¿De qué se compone un lenguaje de programación?"
tagline: "Aprende los fundamentos de programación con Python"
description: "¿De qué se compone un lenguaje de programación? ¿Qué son las palabras reservadas?"
category: Python
comments: true
--- 

En esta entrada veremos cuáles son los elementos que componen un lenguaje de programación.  

- [¿De qué se compone un lenguaje de programación?](#de-qué-se-compone-un-lenguaje-de-programación)
- [¿Qué son las palabras reservadas?](#qué-son-las-palabras-reservadas)
- [Instrucciones](#instrucciones)
- [Bloques de programación](#bloques-de-programación)
  - [1. Entrada](#1-entrada)
  - [2. Salida](#2-salida)
  - [3. Ejecución secuencial](#3-ejecución-secuencial)
  - [4. Ejecución condicional](#4-ejecución-condicional)
  - [5. Ejecución repetida o iterativa](#5-ejecución-repetida-o-iterativa)
  - [6. Reutilización o almacenar y rehusar](#6-reutilización-o-almacenar-y-rehusar)
- [Conclusión](#conclusión)

## ¿De qué se compone un lenguaje de programación?  

Un lenguaje de programación es como un idioma. Un idioma se compone de palabras, frases y párrafos. Así pues, Python se compone de palabras, frases que siguen una gramática (instruccionese) y párrafos que llamaremos bloques de código.  

## ¿Qué son las palabras reservadas?  

Los lenguajes de programación tienen un vocabulario muy reducido. No son como nuestros idiomas español o inglés. A esas palabras se les conoce como *palabras reservadas*. Son palabras que tienen un significado único para Python. Python obedece a estas palabras especiales. Solo las puedes usar para lo que Python estableció para ellas.  

> Las palabras reservadas tienen un significado único para Python.

Palabras reservadas en Python:  
***and del global not with as elif if or yield assert else import pass break except in raise class finally is return continue for lambda try def from nonlocal while***  

## Instrucciones  

Las instrucciones son las frases de Python. Al igual que en español, una sola palabra reservada aislada no dice mucho, por ejemplo `for`. Hace falta insertarla en un contexto más grande.

> Una instrucción representa una operación a realizar en un programa y sus datos correspondientes.  

## Bloques de programación  

Siguiendo el simil de los idiomas naturales, las frases se unen en párrafos que describen una idea. Algo parecido sucede en programación. Existen bloques de instrucciones que sirven para describir una tarea. Así como los párrafos sirven de estructura a un ensayo, así tambien estos bloques estructuran un programa.  

Estos bloques se agrupan en patrones conceptuales de bajo nivel. Un patrón es una estructura. Estas estructuras conceptuales son comunes a todos los lenguajes de programación. No son exclusivos de Python. Cada lenguaje las implementa en su sintaxis de forma diferente. He aquí 6 patrones:

### 1. Entrada

Sirve para obtener datos del mundo exterior (fuera del programa). Consiste en leer datos ya sean de la terminal, un archivo, sensor, GPS, etc.

```python
horasTrabajadas = input("Escribe en número de horas trabajas: ")
Costo = input("Escribe lo que cobras por hora: ")
```

### 2. Salida  

Sirve para mostrar los resultados del programa ya sea imprimirlos en pantalla, guardarlos en un archivo, enviarlos a otro dispositivo como una televisión, radio, etc.

```python
print("Tu pago total es de: ", pago)
```

### 3. Ejecución secuencial  

Sirve para ejecutar una instrucción tras otra en serie, en el mismo orden que aparecen en el script. La computadora después de cada línea pregunta ¿qué sigue? hasta que finaliza el programa. Esto sucede cuando pasamos un script con varias instrucciones al intérprete. Él va a ejecutarlos todos en orden secuencial.  

```python
python salarios.py
```

### 4. Ejecución condicional  

Sirve para dar inteligencia al programa. Pone una condición para ejecutar o una o varias instrucciones Las respuestas siempre son de verdadero o falso. El programa puede tomar diferentes caminos dependiendo de la respuesta. Es una forma de imitar las decisiones humanas. Por ejemplo, tengo un programa de venta de bebidas alcohólicas. Uno de los parámetros de decisión para vender o no una cerveza es la edad. Si eres mayor de 18 años, puedes comprar cerveza. De lo contrario, te vas con la manos vacías.

```python
if edad < 18:
    permiso = "Lo siento, no tienes la edad permitida para comprar bebidas alcohólicas."
else:
    cualCerveza = input("¿Qué cerveza quieres comprar?")
    cuantasCervezas = input("¿Cuántas?")
```

### 5. Ejecución repetida o iterativa  

Sirve para ejecutar un conjunto de instrucciones varias veces, incorporando alguna variación. Esto porque hay tareas repetitivas. Entonces, las podemos poner dentro de un bloque para que se repitan tantas veces cuantas determinemos. A esto en código lo conocemos como ciclos o iteraciones. El ciclo incluye el patrón condicional. Esto significa que cierto bloque de código se va a repetir hasta que cumpla con una condición dada. Esto porque usualmente no hacemos ciclos infinitos.  

```python
for line in file :
    words = line.split()
    for word in words :
        d[word] = d.get(word,0) + 1
```

### 6. Reutilización o almacenar y rehusar  

Sirve para escribir un conjunto de instrucciones una vez, ponerles un nombre y llamar a ese paquete cuando lo necesitemos. A los programadores *no nos gusta repetirnos*. La idea de fondo de este patrón es el concepto de DRY (siglas en inlgés de Don’t Repeat Yourself) "No te repitas a ti mismo".  Por ejemplo, si hay 4 líneas de código que voy a necesitar en 100 lugares diferentes. Luego, resulta que tengo que cambiarlas… Imagínate tener que cambiar las 100 veces. No, mejor las cambio una vez en la definición, y lo demás ya no se ve afectado.  

```python
file = open('donQuijote.txt')

# Definición de la función 
def palabrasMasRepetida(file):
    d = dict()
    for line in file :
        words = line.split()
        for word in words :
            d[word] = d.get(word,0) + 1
    print(d)

    lista = list()
    for k,v in d.items() :
        lista.append( (v,k) )
    #print(lista)

    lista = sorted(lista, reverse=True)
    #print(lista)

    #print("Las 10 palabras más repetidas:")
    for v,k in lista[:10] :
        print(k,"=",v)

    print("Fin")

# Llamada a la función en otro lugar del código
palabrasMasRepetida(file)
```  

Nótese que no tengo que escribir todo el código de la función de nuevo. Solo utilizo el nombre de la misma. Python entiende que debe ejecutar todas las instrucciones contenidas en la función.  

La función se define una vez con la palabra reservada `def` + nombre de la variable + ().  

Dentro de los paréntesis van los parámetros que recibe la función.  

## Conclusión  

Recapitulando, aprendimos que Pytnon se compone de palabras reservadas, que podemos formar frases -instrucciones- compuestas de palabras, y con las frases podemos formar bloques de código. Estos bloques de código conforman la estructura de un programa. También vimos los cuatro patrones de código más importantes, a saber: secuencial, condicional, repetivo y almacenamiento y rehutilización. 
