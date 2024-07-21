# Unidad 1 

## ¿Qué es Java? 
Es una teconologia pensada para desarrollar apicaciones grandes y escalables, de gran integracion con otras tecnologias. 

- *Multiplataforma*: 
    Significa que su código es portable , es decir se puede transportar por distintas plataformas, es decir, escribir una sóla vez el código y luego poder ejecutarlo sobre cualquier plataforma. 

- *Sintaxis basada en C/C++*: 
    Aporta una gran simplicidad ya que es una de las formas de escribir código más reconocidas y difundidas. 
- *Orientado a objetos*: 
    Respeta el paradigma de orientacion a objetos, permitiendo utilizar los fundamentos del mismo (herencia, polimorfismo, abstraccion, encapsulamiento) 
- *manejo automatico de memoria*: 
    De manejar la memoria se encarga el *Garbage Collector* un proceso propio de la tecnologia que monitorea y elimina el espacio ocupado que no está siendo utilizado. 

## Ediciones de Java: 
- **Java SE o Java Standard Edition**: Esta área tiene como objetivo el desarrollo de aplicaciones de escritorio. Incluye la funcionalidad básica del lenguaje, como manejo de clases, colecciones, entrada/salida de datos, acceso a base de datos, manejo de sockets, hilos de ejecucion, etc. 

- **Java EE**: Esta área tiene como objetivo el desarollo de aplicaciones empresariales (Enterprise Edition), de gran envergadura. Contempla ambientes web, como los ambientes manejados por servidores de aplicación. Las tecnologias principales incluidas en area son Servlets, JSP, y EJB, entre otras. 

- **Java ME (Micro Edition)**: Esta área del lenguaje se encarga del desarollo de aplicaciones móviles, tales como GPS, Handhelds (Palm), celulares y otros dispositivos moviles programables. 

## Desarrollo compilacion y ejecucion: 

### Java Development Kid (JDK): 
Este es el kit de desarollo propuesto por la Sun Microsystem para desarrollos en JAVA. Incluye herramientas como un compilador, un debugger, un documentador, un empaquetador para crear archivos de distribucion entre otras herramientas pero no incluye un IDE. 

### El compilador: 
Este viene incluido con el JDK, lo podemos encontrar en Windows como javac.exe (ejecutable). El compilador transforma los archivos de código fuente (es decir, los .java), en archivos compilados, denomidados bytecode. Los archivos compilados tienen la extension '.class' y son archivos binarios. 

> creo que se compila en la con sola con una sentecia como: `javac miArchivo.java` 

### El java runtime enviroment (JRE): 
El JRE es el ambiente de ejecucion de Java, y también está incluido en el JDK. Tiene como componentes más importantes a la Java Virtual Machine y a las class libraries, que son las que contienen a las clases base del lenguaje de programacion Java (las que llamamos con los imports) 

El JRE lo podemos encontrar de forma indepente a al JDK, ya que es necesario para ejecutar aplicaciones Java. 

### La Java Virtual Machine: 
La JVM viene incluida dentro del JRE y tiene como principal objetivo la ejecución de código Java compilado, es decir del archivo .class. La JVM se encarga de interpretar el bytecode y convertirlo a código nativo en tiempo de ejecucion, lo cuál hace que esta última sea un poco más lenta, pero garantiza la portabilidad. Así, Java se puede ejecutar en cualquier sistema que tenga instalada el JRE. 

### La variable de entorno CLASSPATH 

Esta se utiliza para referenciar al *directorio* dónde estarán ubicadas todas las clases construidas en JAVA, para que el JRE al ejecutar una clase sepa dónde ubicar al resto de las clases o archivos empaquetados que contiene clases. 


## Tipos de datos 

En la programacion los tipo de datos más comúnes son: 

- **Entero**: Es un número dentro del conjunto de los números enteros. 

- **Real**: Los numeros reales, como:  2.25, 1429, 1456,  0.0 -12.0, -27.34.

- **Caracter**: Está conformado por un único elemnto que puede ser un dígito, una letra o un símbolo de puntuacion o simbolo "especial" como los de pregunta, exclamacion, slash, entre otros. Algunos ejemplos: 'a', 'D', '&', '^', '%', '!'. Generalmente se los envuelve en comillas simple. 

- **Cadenas (string)**: Este valor está formado por un *conjunto de caracteres*. 
Ejemplos: "Juan", "Av. Rivadavia 950", "Matricula", " ". Este último dato es lo que conocemos como una cadena vacía (sin caracteres) y se represneta como dos comillas seguidas. 

- **Tipo Lógico**: 
Este dato puede tomar los siguientes valores: *True* o *False*, que los utilizaremos para realizar operaciones lógicas o para trabajar con condiciones. 

## Números, Cadenas de Texto y Booleanos: 

En java existen mucho tipos de datos, para represntarlos podriamos por ejemplo usar el comando: 

`System.out.println(12);` 

Con los números solemos representar informacion cuantitativa y hacer operaciones matematicas. Las Strings para repesentar caracteres, cualesquiera que sea: 

`System.out.println("Soy una cadena de caracteres &%");` 

Los booleanos representar datos del tipo de lógica computacional, es decir representan 2 valores, true o false. 

`System.out.println(true)` 

También podemos indicar que existen los tipo de datos primitivos, estos son `double`, `int`, `float`, `short`, `long`, `boolean`, `char`, `byte`. Cada uno con sus distintas caracteristicas. 



## Variable y constantes JAVA 

- Variables: Una variable es un espacio en memoria, cuenta con un identificador y un valor asociado segun el tipo declarado. Se usa para "recordar" y recuperar un dato cuando lo necesitemos. 

Para declararla, indicamos su tipo: 
`int numero1;` 

Si bien aún no tiene un valor asociado (es decír, no está inicializada) el espacio en memoria ya está "reservado". 
Si luego quisieramos usarla, usariamos por ejemplo: 

`System.out.println(numero1);` 

Pero esto nos daría un error, ya que no podemos imprimir nada si no tiene un valor asociado. 




- Constante: A diferencia de las varibales, el valor de las constantes (el dato asociado) no puede ser alterado. 

Para nombrar a las variables usamos *nombres significativos*, que representen al contenido. Dicho nombre puede comenzar con cualquier letra, o los simoblos '$' o '_'. Debemos considerar que se hace distintcion de las mayusculas o minusculas(*case sensitive*). Por convencion se útiliza camelCase. 

