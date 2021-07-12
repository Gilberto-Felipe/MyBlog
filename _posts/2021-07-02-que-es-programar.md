---
layout: post
title: "¿Qué es programar?"
tagline: "Fundamentos de programación"
category: Python
comments: true
---


## Introducción  
Quiero dedicar una serie de artículos a los fundamentos de programación utilizando Python. Esto porque realicé el curso *[Python for every body](https://www.coursera.org/specializations/python)* impartido por el Dr. Charles Severance en la plataforma Coursera. El curso me inspiró a a compartir mi resumen del curso, sus ejercicios y el bául de conocimiento que llevo conmingo.  

El curso me encantó. Aprendí un montón sobre Python, internet, la web, bases de datos, estructuras de datos y algoritmos. El profesor es carismático y explica de forma sencilla muchos conceptos fundamentales de la programación y practicas lo aprendido con ejercicios.  

La idea de fondo del curso es que cualquiera puede programar, aunque no te dediques a eso profesionalmente. El curso está en inglés. Eso puede ser una desventaja. Pero si tienes un nivel intermedio básico, te animo a realizarlo.  

El objetivo de este primer artículo es dar un contexto y unos conceptos generales. Para que si los desconoces, puedas tener una base y se te facilice adentrarte en el mundo de la progamación.  

Cuando se aprende algo nuevo, se recomienda partir de lo más fácil a lo más difícil. Por eso escogí Python, porque es un lenguaje fácil de aprender. Además, es un lenguaje multipropósito; esto significa que con él podemos programar aplicaciones de escritorio, web, videojuegos, científicas, ciberseguridad, etc. Si vas iniciando tu viaje en el mundo de la programación y no sabes a qué área te gustaría dedicarte, Python es una gran opción.  

<p style="text-align: center;">
<i class="fab fa-python" style='font-size:40px;color: #159957;'></i> 
</p>

## ¿Qué es programar?  
Programar es dar instrucciones a una computadora para realizar una tarea. Programar es resolver problemas utilizando como herramienta un lenguaje de programación.  

Programar se parece a otras actividades humanas como cocinar o escribir un cuento. Por una parte, cocinar tiene ingredientes, una receta (una serie de pasos) y al final obtenemos como resultado un platillo. Por otra, escribir un cuento conlleva una introducción, una trama y un desenlace. Un programa cuenta una historia. Tiene una introducción, un proceso y un resultado final.  

### ¿Qué es un programa?  
Un programa es un conjunto de instrucciones que resuelve un problema. 

### ¿Qué es el hardware?  
Llamamos hardware a la parte física de una computadora. Por computadora entiéndase cualquier dispositivo de cómputo. Puede ser el procesador de una computadora, los periféricos como el ratón o el teclado, la pantalla, un celular, una tableta, una calculadora, una televisión, etc.  

### ¿Qué es el software?  
El software es un conjunto de programas que resuelven una tarea. Es el componente lógico de una computadora. Se entiende por oposición al hardware que es la parte física.  

El software forma parte de nuestra vida diaria. Todos los dispositivos digitales que utilizamos contienen software. Ese software fue diseñado, codificado y probado para resolver nuestros problemas. Por ejemplo, calentar agua en el microondas, acceder a la página web de tu escuela, o darle "me gusta" a las publicaciones de un amigo en Facebook.  

### ¿Qué es un lenguaje de programación?  
Es un lenguaje formal, un conjunto de símbolos y códigos que permiten que el programador creé programas. Es decir, le permiten a un programador dar instrucciones a una máquina.  

Los lenguajes de programación se pueden clasificar de diferentes formas dependiendo del criterio de división de cada clasificación. Según su nivel de abstracción, aquí abstancción significa qué tan atado está un lenguaje al hardware y a la arquitectura específica de una computadora, se clasifica a los lenguajes de programación en lenguajes de bajo nivel, lenguajes de alto nivel.  

El código máquina es un código directamente interpretable por un microprocesador, el núcleo de una computadora. Esta basado en el sistema binario, es decir, en solo dos estados representados por el 0 y el 1. Este lenguaje es muy difícil para un humano.  

El lenguaje de bajo nivel por excelencia es el Ensamblador. En este lenguaje se utilizan palabras llamadas mnemónicos que sustituyen al código de máquina binario. Es la representación más directa del código máquina. Tanto el código máquina como el ensamblador están anclados a la manipulación del hardware.  

Los lenguajes de alto nivel utilizan instrucciones más semejantes al lenguaje humano. Algunos manipulan directamente el hardware, podríamos llamarlos lenguajes de medio nivel. Entre ellos están C y C++. Otros lenguajes más modernos son más abstractos y el lenguaje maneja por ti la manipulación del hardware, como por ejemplo la asignación de espacios de memoria. Entre ellos están: Java, C#, JavaScript, Python, Go, Rust, PHP, entre otros.  

### ¿Quién es un programador?  
Es la persona que escribe programas de computadora. Es un intermediario entre el hardware y el usuario.  

### ¿Se programa con un teclado?  
Se programa con la inteligencia. Un teclado es un medio para programar, pero no la causa. Podríamos programar sin un teclado en una pantalla táctil, o con un ratón.  

### ¿Qué son los errores en programación?  
Un error es una instrucción que no es procesable para la computadora. Las instrucciones para la computadora deben ser exactas y sin ambigüedad. Un error significa que la computadora está perdida, que no entendió nuestra instrucción. No que somos tontos y no servimos para programar.  

En la computación a los errores se les conoce como bugs. En inglés bug significa insecto. Pero ¿qué tiene que ver un insecto con un error en las computadoras? [La historia](https://computerhoy.com/noticias/software/que-es-bug-51858#:~:text=Bug%20significa%20insecto%2C%20literalmente.,mal%20funcionamiento%20de%20un%20aparato.) es que en 1947 un insecto, una polilla para ser exactos, ocasionó un error en una de las computadoras Mark de la universidad de Hardvard. Pues sí, el origien del fallo era un *bug*.

### ¿Qué tipos de errores existen en la programación?  
Existen dos tipos de errores: los errores lógicos y los errores sintácticos.  

Los primeros son sustanciales. Se deben a un fallo en la lógica con la que afrontas el problema como por ejemplo cuando los pasos no siguen una secuencia lógica, o te faltó un paso. Cuando estos ocurren suelen ser más difíciles de detectar. Se advierten hasta que el programa se rompe y lanza un error.  

Los segundo son accidentales, como por ejemplo un error tipográfico o que estas utilizando una palabra reservada por el sistema. Generalmente, los editores de código o IDEs que utilizas para programar detectan los errores sintácticos y los colorean. 

### ¿Qué es un editor de código?  
Un editor de código es un software que sirve para escribir programas, es como un Word pero para los programadores. Algunos editores de código que puedes usar son: Visual Studio Code, Atom, Brackets y Sublime Text. Actualmente en el 2021, el editor de código más popular es Visual Studio Code. 

### ¿Qué es un IDE?  
Un IDE (*integrated development environment*) es un ambiente integrado de desarrollo. Es un software con herramientas integradas para construir aplicaciones. Contiene un editor de código, terminales, compiladores, herramientas para automatizar el despliegue del software en un servidor local y para hacer pruebas. Algunos de ellos son: Visual Studio, NetBeans e IntelliJ.  

### ¿Qué es la ingeniería de software?  
La ingeniería de software busca resolver problemas mediante el diseño, creación y mantenimiento de software de calidad. En otras palabras, es aplicar los métodos de la ingeniería a la construcción de software.  

### Software y los humanos  
El ser humano y el software, una creación hecha por el hombre, se complementan. Por una parte, el ser humano es mejor para unas tareas que el software y viceversa. El software no entiene el contexto, el humano sí. Por el momento, esto es una limitante del software. En cambio, nosotros humanos entendemos el contexto y reparamos cosas cuando nos equivocamos al hablar, escribir, etc. Además poseemos la intuición y la experiencia. En ocasiones nos saltamos parte del proceso lógico porque podemos intuir el resultado.  

Por otro lado, las computadoras son mejores que nosotros para los cálculos exactos, para tareas repetitivas y aburridas, o para tareas peligrosas por ejemplo cuando se usan robots. Las computadoras no se cansan.  

Imagínate que debes contar el número de palabras que hay en la primera página del Quijote y tienes un minuto. Ahora qué pasaría si debes contar todas las palabras del libro y cuántas veces se repite cada una. ¡Exacto! 😂 Mejor que lo haga Word.  

## Conclusión
Recapitulando, en este artículo vimos un contexto y conceptos generales relacionados con la programación que nos ayudan a tener una base. En el siguiente artículo veremos dónde viven los programas y cuatro patrones de código.  

## Referencias
Severance, C. *[Python for every body](https://www.coursera.org/specializations/python)*. El curso y todos sus materiales tienen una licencia Creative Commons Attribution 3.0. Todos los materiales son gratuitos.  
Severance, C. *[Python para todos](https://es.py4e.com/)*. Es el sitio web donde puedes encontrar los materiales del curso en español.  
[Documentación oficial de Python](https://www.python.org/doc/).