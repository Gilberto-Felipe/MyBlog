---
layout: post
title: "¿De qué se compone un lenguaje de programación?"
tagline: "Aprende los fundamentos de programación con Python"
description: "¿De qué se compone un lenguaje de programación? ¿Qué son las palabras reservadas?"
category: Python
comments: true
--- 

En esta entrada veremos cuáles son los elementos que componen un lenguaje de programación y cuáles son las palabras reservadas en Python.  

- [¿De qué se compone un lenguaje de programación?](#de-qué-se-compone-un-lenguaje-de-programación)
- [Símbolo `>>>` en el intérprete de Python](#símbolo--en-el-intérprete-de-python)
- [Cerrar el intérprete con `quit()`](#cerrar-el-intérprete-con-quit)
- [Mensajes de error en Python](#mensajes-de-error-en-python)
- [Escribir en un programa en el editor de código](#escribir-en-un-programa-en-el-editor-de-código)

## ¿De qué se compone un lenguaje de programación?  

Un lenguaje de programación es como un idioma. Un idioma se compone de palabras, frases y párrafos. Así pues, Python se compone de palabras, frases que siguen una gramática correcta y párrafos que llamaremos bloques.  

Los lenguajes de programación tienen un vocabulario muy reducido. No son como nuestros idiomas español o inglés. A esas palabras se les conoce como *palabras reservadas*. Son palabras que tienen un significado único para Python. Python obedece a estas palabras especiales. Solo las puedes usar para lo que Python estableció para ellas.  

> Las palabras reservadas tienen un significado único para Python.

Palabras reservadas en Python:  
***and del global not with as elif if or yield assert else import pass break except in raise class finally is return continue for lambda try def from nonlocal while***  

Veremos algunas de las palabras reservadas poco a poco.  

## Símbolo `>>>` en el intérprete de Python  

Para hablar con Python, abre la línea de comandos y llama al intérprete. El símbolo `>>>` indica que el intérprete nos está escuchando. Está preguntando ¿qué quieres que haga? ¿qué sigue?  

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

Python es muy exigente. Si no entendió lo que pides te lo hace saber en un instante:  

```python
>>> Hola mundo
  File "<stdin>", line 1
    Hola mundo
         ^
SyntaxError: invalid syntax
```

Hay diferentes tipos de error en Python que poco a poco iremos conociendo.

## Escribir en un programa en el editor de código  

Cuando ecribimos un programa, generalmente lo hacemos en un editor de código. Es más cómodo y no tiene los límites del interprete en la línea de comandos.  

Llamamos *script* a un archivo con instrucciones para realizar una tarea. Los archivos de Python terminan con la extensión .py.

1. Primero, abirmos abrimos nuestro editor de código favorito.
2. Creamos un nuevo archivo y lo nombro *holamundo.py*.
3. Allí escribimos el famosísimo "Hola mundo" y guardamos cambios. Ya tenemos el script.
4. Por último, para ejecutar el script, abrimos el intérprete de Python y le pasamos el nombre de nuestro script.

```python
@usuario> python holamundo.py
Hola mundo
```

Hecho, hemos ejecutado nuestro primer script.
