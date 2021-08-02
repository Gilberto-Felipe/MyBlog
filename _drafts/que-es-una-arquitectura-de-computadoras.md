---
layout: post
title: "¿Qué es una arquitectura de computadoras?"
tagline: "Fundamentos de programación con Python"
description: "En este artículo conocerás qué es una arquitectura de computadoras, las arquitecturas Von Newmann y Hardvard, y por qué es importante conocer cómo se organiza el hardware."
category: Python
comments: true
---

En este artículo conocerás qué es una arquitectura de computadoras, las arquitecturas Von Newmann y Hardvard, y por qué es importante conocer cómo se organiza el hardware. 

## ¿Porqué es importante conocer sobre la arquitectura de computadoras?
Conocer cómo es una computadora por dentro, su organización y su funcionamiento, aunque sea de forma general, es importante porque los programas se ejecutan en ella. El software vive en las computadoras, especialmente en el procesador y en la memoria.  

## ¿Qué es una arquitectura de computadora?  
Una arquitectura de computadora es un modelo que representa cómo está organizado el hardware de una computadora y cómo funciona.  

## ¿Cuáles son los componentes de la arquitectura de computadora?
Los componentes son:  
- Periféricos
- Unidad central de procesamiento (CPU)
- Memoria principal
- Almacenamiento

### Periféricos  
Los periféricos sirven para la entrada y salida de datos. Sirven para que interactuemos con la computadora. Entre ellos están el ratón, el teclado, la pantalla, la impresora, etc.

### CPU  
La unidad central de procesamiento (CPU por sus siglas en inglés), o simplemente el procesador, es el componente más importante de una computadora. Su función es interpretar las instrucciones de un programa informático a través de operaciones matemáticas, lógicas y externas procedentes de los periféricos. Es el corazón de una computadora, es el componente que realza el cálculo. 

La CPU está compuesta por millones de transistores. Cada transistor puede hacer operaciones binarias. En breve, la misión del CPU es preguntar qué instrucción sigue y procesarla.  

Una computadora puede tener más de un CPU. Actualmente, los procesadores están implementados en un solo circuito integrado o chip. No solo eso, sino que un chip puede ser multinúcleo (multi-core en inglés), es decir, puede tener varios procesadores.   

### Memoria principal o RAM  
La memoria guarda los datos que va a usar la CPU. Es una memoria temporal. Si reiniciamos la computadora o se nos apaga, todos los datos de la memoria RAM se pierden. Aquí viven los datos y las instrucciones que interpretará la CPU.  

Características:
- Menor capacidad que el almacenamiento. 
- Mayor velocidad que el almacenamiento.   

Cuando la CPU necesita un programa que no está en la RAM, mánda por él al almacenamiento, el programa se carga en la memoria principal para que la CPU pueda interactuar con él.  

### Almacenamiento o memoria secundaria  
Es un almacenamiento permanente. Los datos se conservan si apagamos la computadora. Allí se alojan los programas que no están siendo utilizados.  

Características:
- Mayor capacidad de almacenamiento que la memoria principal.
- Menor velocidad que la memoria principal.  

Actualmente, esto coincide con nuestro disco duro o disco de estado sólido. Otros medios de almacenamiento permante fueron las cintas perforadas, las magnéticas, o los discos flexibles (floppies).  

## Arquitectura Von Neumann  
La arquitectua o modelo Von Neumann debe su nombre al polímata húgaro John von Neumann. Su modelo consta de tres componentes: 
- CPU o unidad de procesamiento
- Memoria principal
- Mecanismos de entradas y salidas  

La característica principal de este modelo es que la memoria principal puede almacenar tanto instrucciones como datos. El procesador y la memoria principal se comunican por un único bus común. Este es la principal desventaja de este modelo, porque no se pueden procesar instrucciones y datos al mismo tiempo. A esto se le llama el cuello de botella Von Neumann.  

Se llama bus a los canales digitales a través de los cuales los componentes de la computadora se pasan datos. Son cables o pistas de un circuito impreso por donde viajan los datos. La mayoría son de materiales metálicos como el cobre.  

## Arquitectura Hardvard  
Es una evolución de la arquitectura Von Neumann. El nombre viene de la computadora Harvard Mark I. El modelo consta de cuatro componentes:  
- CPU
- Memoria de instrucciones
- Memoria de datos
- Mecanismos de entradas y salidas  

La característica principal de este modelo es que separa los datos de las instrucciones. Es decir, cuenta con un espacio de memoria y bus dedicado para los datos, otro espacio y otro bus para las instrucciones.  

Las computadoras actuales utilizan una arquitectura Harvard modificada.  

## Conclusión  
En resumen, en este artículo conocimos qué es la arquitectura de computadoras, cuáles son sus principales componentes, las dos arquitecturas históricas que marcaron la arquitectura de computadoras: los modelos Von Neumann y Hardvard. Con todo esto nos podemos formar una idea de qué pasa a nivel hardware cuando se ejecuta el software.   







