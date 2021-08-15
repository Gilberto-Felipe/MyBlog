---
layout: post
title: "¿Cómo instalar Python 3?"
tagline: "Instalando Python 3"
description: "En esta entrada veremos cómo instalar Python 3 en Windows o Linux"
category: Python
comments: true
---

En esta entrada veremos cómo instalar la última versión de Python. La última versión de Python es la 3.9, a fecha de agosto de 2021. Ten encuenta que la versión cambiará, y tendrás que descargar la versión que corresponda.

La instalación es semejante para Windows, Linux o Mac OS.  

Tabla de contenidos  

- [¿Cómo revisar si tenemos instalado Python?](#cómo-revisar-si-tenemos-instalado-python)
- [¿Cómo instalar Python 3 en Windows?](#cómo-instalar-python-3-en-windows)
- [Intérpretes de Python en línea](#intérpretes-de-python-en-línea)
- [Por qué Python 3.x](#por-qué-python-3x)
- [Nuestro primer programa en Python](#nuestro-primer-programa-en-python)
- [Conclusión](#conclusión)

## ¿Cómo revisar si tenemos instalado Python?  

En Windows abre el programa de Símbolo del sistema o cmd, en Linux o Mac OS una terminal.  

Escribe Python donde indica el cursor y da *enter*.  

```python
@usuario> python

Python 3.8.5 (default, Sep  4 2020, 07:30:14) 
[GCC 7.3.0] :: Anaconda, Inc. on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```

La línea de comandos mostrará información de la versión que tienes instalada. De lo contrario arrojará un error.  

## ¿Cómo instalar Python 3 en Windows?  

1. Ve a la página de [descarga](https://www.python.org/downloads/) del sitio web oficial de Python.  
2. Descarga la última versión para tu sistema operativo.
3. Ejecuta como administrador el archivo ejecutable .exe.
4. Sigue el asistente de instalación.
    - Selecciona la casilla para instalar el lanzador para todos los usuarios.
    - Selecciona la casilla añadir Python al PATH.
5. Reinicia el equipo.
6. Comprueba la instalación en la línea de comandos.  

Al instalar el lenguaje, se instala también su intérprete. Un intérprete es un programa que traduce en tiempo de ejecución las instrucciones a código máquina. Para conocer más información sobre el intérprete, puedes leer mi entrada [¿Qué es un lenguaje de programación?]().  

## Intérpretes de Python en línea  

Si no puedes o no deseas instalar Python en tu equipo, puedes utilizar intérpretes a través de la web. Algunos de ellos son [Google Colab](https://colab.research.google.com/notebooks/intro.ipynb?utm_source=scs-index#) y [Python tutor](http://www.pythontutor.com/visualize.html#mode=edit).

## Por qué Python 3.x  

La versión de Python 2 es imcompatible con Python 3. La versión 2 quedó sin soporte desde el 1 de enero de 2020. Por eso, instala la última versión mayor de Python y utiliza esta.  

¿Qué indican los números de las versiones?  

- El primer número de la versión, en este caso el **3**.9, indica la versión mayor. Es el numero más importante, significa que se realizaron cambios grandes.  
- El segundo número, en este caso el 3.**9**, indica nuevas funcionalidades.  

## Nuestro primer programa en Python  

Ya que instalamos la última versión de Python, manos al teclado. Escribiremos nuestro primer programa. Vamos a imprimir el famosísimo "Hola Mundo".  

Abre la línea de comandos.  

Para hablar con Python, tenemos que despertar al intérprete de Python. Escribe `python` en la línea de comandos y da *enter*.

```python
@usuario> python
Python 3.8.5 (default, Sep  4 2020, 07:30:14) 
[GCC 7.3.0] :: Anaconda, Inc. on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```

Luego, escribe esta instrucción después de los `>>>` y presiona *enter*:  

```python
>>> print("Hola Mundo")
```

¡Felicidades, ya escribiste tu primer programa en Python!  

`print()` es una instrucción en Python que imprime (*print* en inglés) en la línea de comandos lo que pasamos dentro de los parentesis.  

`"Hola Mundo"` se escribe entre comillas (pueden ser dobles " " o simples ' '). Con ellas se indica que es un texto, lo opuesto a un número.  

Ahora intenta esto. Presiona *enter* después de cada línea:

```python
print(5+5)
print("5+5")
```

¿Qué resultado imprimen ambas instrucciones? El resultado es diferente, ¿verdad?  

En el primer caso, Python realiza una suma. En cambio, en el segundo no realiza la operación; imprime la operación como si fuera un texto.  

## Conclusión  

Resumiendo, en estra entrada vimos cómo instalar la última versión de Python, en este caso 3.9, en tu sistema operativo y realizamos nuestro primer programa en Python. ¡Yei!  
