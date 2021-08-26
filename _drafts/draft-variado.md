---
layout: post
title: "Draft variado"
date: 2022-08-29 20:00:00 -0600
tagline: "draf variado"
description: "draf variado"
category: Python
comments: true
---

## Tarea para casa  

Ahora, vamos a utilizar una variable. ¿Te acuerdas de tus clases de matemáticas? Las letras podían almacenar números, por ejemplo x indicaba dónde estaba escondido el tesoro pirata XD. No, x indicaba un número desconocido. Algo parecido es una variable en programación.

Una variable es como una caja donde podemos guardar datos, ya sean letras, números, funciones, etc. El punto es que esos datos pueden variar. Por eso, se llaman variables.  

Para guardar/escribir un dato dentro de una variable utilizamos el signo `=`.

**Atento: `=` ¡No significa igualdad!**  

### El operador `=` asignación  

El `=` es un operador que indica a Python que va a guardar lo que está después del `=` dentro de la variable (leyendo de izquierda a derecha).  

```python
edad = 20
```

La variable guarda en la memoria RAM ese valor. Si cierras el intérprete, se pierde la variable y lo que tenías guardado en ella.  

Vas a llamar a las variables `nombre` y `edad`. Vas a guardar dentro ellas tu nombre y edad.  

```python
nombre = "tu nombre dentro de las comillas"
edad = #el número entero de tu edad sin commillas y sin el signo gato/almohadilla/número
print("Hola soy",nombre,"tengo",edad)
```

El caracter `#` indica a Python que lo que está a después del `#` es un comentario. Python no procesa los comentarios, se los salta.  

Para cerrar el intérprete de Python en línea de comandos utilizamos:  

```python
exit()
```


*********
## Símbolo `>>>` en el intérprete de Python  

Para hablar con Python, abre la terminal y llama al intérprete. Aparece el símbolo `>>>`. Se llama *prompt*. El prompt indica que el intérprete nos está escuchando. Está preguntando ¿qué quieres que haga? ¿qué sigue?  El cursor se coloca después del prompt y podemos escribir nuestras órdenes para Python.  

```python
@usuario> python
Python 3.8.5 (default, Sep  4 2020, 07:30:14) 
[GCC 7.3.0] :: Anaconda, Inc. on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```

## Cerrar el intérprete con `quit()`

Para despedirnos de Python, utilizamos el comando: `quit()`.

```python
@usuario> python
Python 3.8.5 (default, Sep  4 2020, 07:30:14) 
[GCC 7.3.0] :: Anaconda, Inc. on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print("Hola Python y adiós")
Hola mundo
>>> quit()
```

## Mensajes de error en Python

Python es muy exigente. Si no entendió lo que pides, te lo hace saber en un instante:  

```python
>>> Hola mundo
  File "<stdin>", line 1
    Hola mundo
         ^
SyntaxError: invalid syntax
```

El programa se ejecuta línea por línea, se rompe cuando encuentra un error. En ese momento no te enfades o entres en pánico. ¿Qué debemos hacer? Python nos da una pista de qué pudo haber ido mal. Cuando nuesto programa lanza un error es el momento de ir a la caza del error para corregirlo. A eso se le llama depurar. La depuración la veremos a continuación.  

## Escribir en un programa en el editor de código  

Cuando ecribimos un programa, usualmente lo hacemos en un editor de código. Es más cómodo y no tiene los límites del interprete en la línea de comandos.  

Llamamos *script* a un archivo con instrucciones para realizar una tarea. Los archivos de Python terminan con la extensión .py.

1. Primero, abirmos nuestro editor de código favorito, Visual Studio Code.
2. Creamos un nuevo archivo en el directorio elegido y lo nombro `holamundo.py`.
3. Allí escribimos el famosísimo "Hola mundo" y guardamos cambios.
4. Por último, abrimos el intérprete de Python, le pasamos el nombre de nuestro script y damos *enter*.

```python
@usuario> python holamundo.py
Hola mundo
```

Hecho, hemos ejecutado nuestro primer script. Ese fue un script de una línea, nuestro script puede tener tantas líneas como necesite.  

**********



### ¿Qué es la ingeniería de software?  

La ingeniería de software busca resolver problemas mediante el diseño, creación y mantenimiento de software de calidad. Aplica los métodos de la ingeniería al desarrollo de software.  

### Software y los humanos  

El ser humano y el software, una creación hecha por el hombre, se complementan. Por una parte, el ser humano es mejor para unas tareas que el software y viceversa. Por un lado, el software no entiene el contexto, el humano sí. Por el momento, esto es una limitante del software. En cambio, nosotros entendemos el contexto y reparamos cosas cuando nos equivocamos al hablar, escribir, etc. Además poseemos la intuición y la experiencia. En ocasiones nos saltamos parte del proceso lógico porque podemos intuir el resultado.  

Por otro lado, las computadoras son mejores que nosotros para los cálculos exactos, para tareas repetitivas y aburridas, o para tareas peligrosas por ejemplo cuando se usan robots. Las computadoras no se cansan. Imagínate que debes contar el número de palabras que hay en la primera página del libro Don Quijote y tienes un minuto para hacerlo. Ahora qué pasaría si debes contar todas las palabras del libro y cuántas veces se repite cada una. ¡Exacto! 😂 Mejor que lo haga Word u otro programa.  
