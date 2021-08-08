---
layout: post
title: "¿Cómo instalar Python 3?"
tagline: "Instalando Python 3"
description: "En esta entrada veremos cómo instalar Python 3 en Windows o Linux"
category: Python
comments: true
---

En esta entrada veremos cómo instalar la última versión de Python; en este momento es la versión 3.9. La instalación es semejante para Windows, Linux o Mac OS.  

Ten encuenta que la versión va a cambiar con futuras actualizaciones.  

## ¿cómo revisar si tenemos instalado Python?  

Primero, revisa si tienes instalado Python. En en tu sistema operativo abre una línea de comandos. En Windows cmd, en Linux o Mac OS se llama Terminal.  

Escribe Python donde indica el cursor y da *enter*.  

```python
# En el símbolo de sistema
>python

# Algo semejante a esto:
Python 3.8.5 (default, Sep  4 2020, 07:30:14) 
[GCC 7.3.0] :: Anaconda, Inc. on linux
Type "help", "copyright", "credits" or "license" for more information.
```

La línea de comandos te arrojará información de la versión que tienes instalada. De lo contrario te arrojará un error.  

## ¿Cómo instalar Python 3 en Windows?  
1. Ve a la página de [descarga](https://www.python.org/downloads/) del sitio web oficial de Python.  
2. Descarga la última versión para tu sistema operativo.
3. Ejecuta como administrador el archivo ejecutable .exe.
4. Sigue el asistente de instalación.
    - Selecciona la casilla para instalar el lanzador para todos los usuarios. 
    - Selecciona la casilla añadir Python al PATH. 
5. Reinicia el equipo.
6. Comprueba la instalación en la línea de comandos.  

Al instalar Python se instala también su intérprete. Un intérprete es un programa que traduce en tiempo de ejecución las instrucciones escritas en un lenguaje específico. Para conocer más información sobre el intérprete, puedes leer mi entrada [¿Qué es un lenguaje de programación?]().  

## Intérprete de Python en línea  
Si no puedes o no deseas instalar Python en tu equipo, puedes utilizar intérpretes a través de la web. Algunos de ellos son [Google Colab](https://colab.research.google.com/notebooks/intro.ipynb?utm_source=scs-index#) y [Python tutor](http://www.pythontutor.com/visualize.html#mode=edit).

## Por qué Python 3.x  
La versión de Python 2 es imcompatible con Python 3. La versión 2 quedó sin soporte desde el 1 de enero de 2020. Por eso, instala la última versión mayor de Python y utiliza esta.  

El primer número de la versión, en este caso el **3**.9, indica la versión mayor. Es el numero más importante, significa que se realizaron cambios grandes.  

El segundo número, en este caso el 3.**9**, indica nuevas funcionalidades.  

## Nuestro primer programa en Python  
Ya que instalamos la última versión de Python, manos al teclado. Escribiremos nuestro primer programa. Es un programa sencillo y de consola. Vamos a imprimir el famosísimo "Hola Mundo". Lo haremos en la terminal.  

>De consola significa que no tiene interfaz gráfica. Se ejectua en una línea de comandos y nos mostrará el resultado por la misma línea de comandos.  

Abre la línea de comandos, escribe esta instrucción y presiona *enter*: 

```python
print("Hola Mundo")
```

¡Felicidades, ya escribiste tu primer programa en Python!  

`print()` es una instrucción en Python que imprime (*print* en inglés) en consola lo que pasamos dentro de los parentesis.  

`"Hola Mundo"` se escribe entre comillas (pueden ser dobles "" o simples ''), porque con ellas se indica que es un texto, lo opuesto a un número.  

Ahora intenta esto. Presiona enter después de cada línea/instrucción:

```python
print(5+5)
print("5+5")
```

¿Qué resultado imprimen ambas instrucciones? El resultado es diferente, ¿verdad?  

En el primer caso, Python realiza una suma. En cambio, en el segundo, imprime la operación como si fuera un texto.  

## Tarea para casa  
Ahora, vamos a utilizar una variable. ¿Te acuerdas de tus clases de matemáticas? Las letras podían almacenar números, por ejemplo x indicaba dónde estaba escondido el tesoro pirata XD. No, x indicaba un número desconocido. Algo parecido es una variable en programación.

Una variable es como una caja donde podemos guardar datos, ya sean letras, números, etc. Dedicaré otra entrada a las variables para tratarlas más a fondo. De momento, nos sirve para el ejercicio.  

Para guardar/escribir un dato dentro de una variable utilizamos el signo `=`. 

Atento: **`=` ¡No significa igualdad!**  

El `=` es un operador que indica a Python que va a guardar lo que está a la derecha del `=` (tu derecha) dentro de la variable. La variable guarda en la memoria RAM ese valor. Si cierras el intérprete, se pierde la variable y sus datos.  

Vamos a llamar a las variables `nombre` y `edad`. Vas a guardar dentro ellas tu nombre y edad. 

```python
nombre = "tu nombre dentro de las comillas"
edad = #[tu edad]
print("Hola soy",nombre,"tengo",edad)
```

El caracter `#` indica a Python que lo que está a la derecha del signo es un comentario. Python no procesa los comentarios, se los salta.  

Para cerrar el intérprete de Python en línea de comandos utilizamos:  

```python
exit()
```

## Conclusión  
Resumiendo, en estra entrada vimos cómo instalar la última versiópn de Python, en este caso 3.9, en tu sistema operativo y realizamos nuestro primer programa en Python y utlizamos variables para personalizar nuestro nombre y edad. ¡Yei!
