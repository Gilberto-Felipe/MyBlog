---
layout: post
title: "¿Qué es un lenguaje de programación?"
tagline: "Aprende los fundamentos de programación con Python"
description: "En este artículo conocerás: ¿Qué son los lenguajes de progamación? ¿Cuáles son los lenguajes de alto nivel? ¿Qué es el código máquina?"
category: Python
comments: true
---

En este artículo veremos qué son los lenguajes de programación, alguna de sus clasificaciones y cómo una computadora puede entender las instrucciones que le damos.  

## ¿Qué es un lenguaje de programación?  

Un lenguaje de programación es un lenguaje formal, un conjunto de símbolos y códigos que permiten que el programador dé instrucciones a una máquina.  

## Clasifición de los lenguajes de programación  

Los lenguajes de programación se pueden clasificar de diferentes formas dependiendo del criterio que se tome en cada clasificación.  

### Según su nivel de abstracción  

Según su nivel de abstracción se clasifica a los lenguajes de programación en lenguajes de bajo nivel y lenguajes de alto nivel. Aquí abstancción significa qué tan anclado está un lenguaje de programación al hardware y a su organización y funcionamiento (arquitectura).  

#### Código máquina  

El código máquina es un código directamente interpretable por un microprocesador, el núcleo de una computadora. Está basado en el sistema binario, es decir, en solo dos estados representados por el 0 y el 1. Este es complicado para nosotros humanos.  

```binary
# Si conoces qué hace este programa, escríbelo en los comentarios
0 1 0 0 1 0 0 0 0 1 1 0 0 1 0 1 0 1 1 0 1 1 0 0 0 1 1 0 1 1 0 0 0 1 1 0 1 1 1 1 0 0 1 0 0 0 0 0 0 1 0 1 0 1 1 1 0 1 1 0 1 1 1 1 0 1 1 1 0 0 1 0 0 1 1 0 1 1 0 0 0 1 1 0 0 1 0 0 0 0 1 0 0 0 0 1
```

En principio los 0 y 1 no son relevantes para nosotros tanto como las palabras. ¡A no ser que sea nuestra cuenta de banco! 😂. Pero ya no sería código binario y nos desviamos del tema.  

#### Lenguaje ensamblador  

El lenguaje Ensamblador es el lenguaje de bajo nivel. En este lenguaje se utilizan palabras (llamadas mnemónicos) que sustituyen al código de máquina binario. Es la representación más directa del código máquina. Tanto el código máquina como el ensamblador están anclados a la manipulación del hardware.  

```assembly
# Un Hello World en Ensamblador
b8    21 0a 00 00   #moving "!\n" into eax  
a3    0c 10 00 06   #moving eax into first memory location  
b8    6f 72 6c 64   #moving "orld" into eax  
a3    08 10 00 06   #moving eax into next memory location  
b8    6f 2c 20 57   #moving "o, W" into eax  
a3    04 10 00 06   #moving eax into next memory location  
b8    48 65 6c 6c   #moving "Hell" into eax  
a3    00 10 00 06   #moving eax into next memory location  
b9    00 10 00 06   #moving pointer to start of memory location into ecx  
ba    10 00 00 00   #moving string size into edx  
bb    01 00 00 00   #moving "stdout" number to ebx  
b8    04 00 00 00   #moving "print out" syscall number to eax  
cd    80            #calling the linux kernel to execute our print to stdout  
b8    01 00 00 00   #moving "sys_exit" call number to eax  
cd    80            #executing it via linux sys_call
```

#### Lenguajes de alto nivel  

Los lenguajes de alto nivel son más semejantes al lenguaje natural. Por lo tanto, son mucho más fáciles de aprender y más significativos para nosotros. Algunos de ellos manipulan directamente el hardware y la asignación de memoria, podríamos llamarlos lenguajes de medio nivel. Entre ellos están C y C++.  

```c
# Hola mundo en C
#include <stdio.h>
int main() {
   // printf() muestra en pantalla (consola) el texto entre comillas
   printf("Hola mundo!");
   return 0;
}
```

Otros lenguajes más modernos, son más abstractos y el lenguaje maneja por ti la asignación de espacios de memoria y otras muchas cosas. Esto facilita la vida de los programadores 😀. Entre ellos están: Java, C#, JavaScript, Python y PHP entre otros.  

```python
# Hola mundo en Python
print("Hola mundo!")
```

El Hola mundo, por tradición, es el primer programa cuando aprendes a programar.  

### Según su propósito  

Según su propósito existen dos tipos de lenguajes: los de propósito general y los de propósito específico.  

- De propósito general son Python, Java o C# que permiten emplearlos en diferentes tareas y aplicaciones.  

- De propósito específico es por ejemplo SQL un lenguaje creado exclusivamente para manejar bases de datos relacionales.  

## ¿Cómo entiende una máquina un lenguaje de programación?  

Es una buena pregunta, puesto que la máquina solo entiende el código máquina. ¿Qué pasa para que la máquina pueda entender las instrucciones de los lenguajes de programación? En breve, esas instrucciones se deben traducir al lenguaje máquina. Para hacer esta traducción existen dos técnicas:  

### Intérprete  

El intérprete o traductor es un software que traduce las instrucciones del lenguaje de alto nivel al lenguaje máquina. Esto lo hace durante el tiempo de ejecución. El intérprete traduce línea por línea conforme el programa ejecuta las instrucciones. Si hay algún error, el programa se detiene donde encontró el error. Lenguajes interpretados son por ejemplo: JavaScript y Python.  

### Compilador  

Es la técnica opuesta. Todo el programa se compila (se traduce) a código máquina antes de ser ejecutado. Esto hace que el programa sea más eficiente, porque no se realiza la traducción en tiempo de ejecución. Tiene la ventaja de que el código compilado se puede almacenar para rehusarse luego. Si el compilador encuentra un error, el programa no puede ser compilado. Es necesario correjir el error y compilar. Lenguajes compilados son por ejemplo: C, C++. C# y Java.  

## Conclusión  

En resumen, en este artículo vimos qué es un lenguaje de programación, qué es el código máquina, qué es el lenguaje ensamblador, qué son los lenguajes de alto nivel, qué son los intérpretes y compiladores. En el siguiente artículo veremos que son los bugs en la jerga computacional.  
