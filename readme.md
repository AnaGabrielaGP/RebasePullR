#Ana Gabriela García Páramo   
Tarea N°. 4   

___
___

**¿Qué es un patrón de diseño?** 

Los patrones de diseño son un conjunto de prácticas óptimas de diseño que se utilizan para abordar problemas recurrentes en la programación orientada a objetos. 

Brindan una solución ya probada y documentada a problemas de desarrollo de software que están sujetos a contextos similares. Debemos tener presente los siguientes elementos de un patrón: su nombre, el problema (cuando aplicar un patrón), la solución (descripción abstracta del problema) y las consecuencias (costos y beneficios).

Existen diversas maneras de agrupar los patrones de diseño. Quizá la más extendida es agruparlos según su propósito. En este caso tendríamos las siguientes categorías:  

* _Patrones creacionales:_ utilizados para instanciar objetos, y así separar la implementación del cliente de la de los objetos que se utilizan. Con ellos intentamos separar la lógica de creación de objetos y encapsularla.
* _Patrones de comportamiento:_ se utilizan a la hora de definir como las clases y objetos interaccionan entre ellos.
* _Patrones estructurales:_ utilizados para crear clases u objetos que están incluidos dentro de estructuras más complejas.

___

**¿En Que consiste el patron singleton?**

El patrón Singleton asegura que exista una única instancia de una clase. A primera vista, uno puede pensar que pueden utilizarse clases con miembros estáticos para el mismo fin. Sin embargo, los resultados no son los mismos, ya que en este caso la responsabilidad de tener una única instancia recae en el cliente de la clase. El patrón Singleton hace que la clase sea responsable de su única instancia, quitando así este problema a los clientes.  
Si todos los métodos de esta clase son estáticos, éstos no pueden ser extendidos, desaprovechando así las capacidades polimórficas que nos proveen los entornos orientados a objetos.
El funcionamiento de este patrón es muy sencillo y podría reducirse a los siguientes conceptos:
1. Ocultar el constructor de la clase Singleton, para que los clientes no puedan crear instancias.
2. Declarar en la clase Singleton una variable miembro privada que contenga la referencia a la instancia única que queremos gestionar.
3. Proveer en la clase Singleton una función o propiedad que brinde acceso a la única instancia gestionada por el Singleton. Los clientes acceden a la instancia a través de esta función o propiedad.
Estas reglas se cumplen en todas las implementaciones del Singleton, independientemente de los recaudos que deban tomarse para soportar la correcta ejecución en entornos multihilo.

___

**¿En que consiste el patron Factory?**

Una factoría es un objeto que maneja la creación de otros objetos. Las factorías se utilizan cuando la creación de un objeto implica algo más que una simple instanciación. Los siguientes ejemplos son casos donde una factoría puede ayudar:  
* Es necesario acceder a algún recurso para la creación y configuración de un objeto.
* No conocemos hasta el momento preciso de la instanciación qué tipo concreto de objeto se va a instanciar.

En estos casos, en lugar de que sea el propio objeto quien se encargue de todos los aspectos realativos a la creación, se crea otro objeto que lo haga. De esta manera, se libera al objeto que va a ser creado de aquellas responsabilidades que no le corresponden pero que son necesarias para su creación, manteniendo su independencia.

El siguiente es un ejemplo de la utilización de una factoría para la creación de objetos. Se pueden crear figuras geométricas y calcular su área. Las figuras estarían definidas por una interfaz. Las figuras posibles son círculos y cuadrados.

Se va a utilizar una factoría para crear las figuras, puesto que no conocemos de antemano a qué clase pertenece el objeto que tenemos que instanciar. El uso de una factoría permite separar la lógica de negocio, igual para todos los casos, de la lógica de instanciación de los objetos. 

___

**¿En que consiste el patron Builder?**

- *Problema y Contexto:* Un único proceso de construcción debe ser capaz de construir distintos objetos complejos, abstrayéndonos de los detalles particulares de cada uno de los tipos.
- *Se aplica cuando:* Nuestro sistema trata con objetos complejos (compuestos por muchos atributos) pero el número de configuraciones es limitada. El algoritmo de creación del objeto complejo puede independizarse de las partes que lo componen y del ensamblado de las mismas. 
- *Solución y Estructura:* La solución será crear un constructor que permita construir todos los tipos de objetos, ayudándose de constructores concretos encargados de la creación de cada tipo en particular. Un objeto director será el encargado de coordinar y ofrecer los resultados.

La estructura es la siguiente:  

1. *Director:* Se encarga de construir un objeto utilizando el Constructor (Builder).
2. *Builder:* Interfaz abstracta que permite la creación de objetos.
3. *Concrete Builder:* Implementación concreta del Builder definida para cada uno de los tipos. Permite crear el objeto concreto recopilando y creando cada una de las partes que lo compone.
4. *Product:* Objeto que se ha construido tras el proceso definido por el patrón.

Consecuencias:  

POSITIVAS: 
+ Reduce el acoplamiento. 
+ Permite variar la representación interna del objeto, respetando la clase builder. Es decir, conseguimos independizar la construcción de la representación.  

NEGATIVAS: 
+ Introduce complejidad en los programas. 


___

**¿Investigar que es la herramienta ADB de Android?**

El ADB es básicamente un software o programa de PC a través del cual se puede dar órdenes especiales al móvil, usando comandos de texto. Estos comandos incluyen órdenes básicas que se usan en el sistema Linux (copiar, pegar, mover, son algunos ejemplos) así como una variedad de comandos específicos para desarrolladores. Estos comandos se pueden mandar al teléfono cuando el mismo está encendido/arrancado, y también cuando se encuentra en modo recovery. La herramienta ADB se puede utilizar para enviar comandos hacia dispositivos con y sin root.

___
**Para que sirve el operador final en JAVA**

*FINAL:* Indica que una variable, método o clase no se va a modificar, lo cuál puede ser útil para añadir más semántica, por cuestiones de rendimiento, y para detectar errores.  
* Si una variable se marca como final, no se podrá asignar un nuevo valor a la variable.
* Si una clase se marca como final, no se podrá extender la clase.
* Si es un método el que se declara como final, no se podrá sobreescribir.
Algo muy a tener en cuenta a la hora de utilizar este modificador es que si es un objeto lo que hemos marcado como final, esto no nos impedirá modificar el objeto en sí, sino tan sólo usar el operador de asignación para cambiar la referencia.

___

**¿Que Lenguajes soportan Sobre Carga de operadores?**

La sobrecarga de operadores es una herramienta que nos proporcionan algunos lenguajes como _C++_ para que podamos definir el significado de uno o varios operadores en el contexto de una determinada clase de objetos. _C#_ soporta la sobrecarga de operadores con el objetivo de simplificar la escritura de los programas y hacer más clara la lectura del código. _Java_ no admite la sobrecarga de operadores, aunque internamente sobrecarga el operador + para la concatenación de cadenas. 

___

**¿Para que sirve Gradle?**

Gradle es una herramienta para automatizar la construcción de nuestros proyectos, por ejemplo las tareas de compilación, testing, empaquetado y el despliegue de los mismos. Es muy flexible para la configuración, pero además ya tiene armadas las tareas para las mayoría de los proyectos por default.  

Gradle usa un “Domain Specific Language” (DSL) basado en “Groovy” para declarar la formas de construir el proyecto. Así que para configurarlo simplemente podemos escribir código en Groovy, el cual en su sintaxis es muy similar a Java, lo que nos va a hacer sencillo expresar, las tareas que queremos que realice.  

Maneja compilaciones incrementales, básicamente a que verifica si hubo algún cambio en el código fuente después de la última compilación, si es así re-compila todo, si no se ahorra la tarea.  

Tiene un gran soporte para multi-proyectos, nuestro proyecto puede depender de solo un proyecto, o varios, nosotros podremos definir la relación de dependencias así Gradle se encargará de ello. Además también soporta construcciones parciales, digamos que nuestro proyecto depende de uno que necesita o no ser re-compilado, Gradle verificará esa condición, y si es necesario re-compila el proyecto del que dependemos antes de realizar esa tarea con el nuestro.

Que es el Gradle wrapper?

Esto nos permite realizar las tareas de Gradle en sistemas donde no lo tengamos instalado, es una buena forma de compartir el código fuente con el sistema de construcción del proyecto con el. O también para obligar la utilización de cierta versión de Gradle.

___

**¿En que consiste la injección de dependencias en desarrollo de software, y por qué es útil utilizarla?**

Aparte de un patrón de diseño de software, éste nos ayuda a separar nuestro código por responsabilidades, siendo que en esta ocasión sólo se dedica a organizar el código que tiene que ver con la creación de los objetos.  

Uno de los principios básicos de la programación, y de las buenas prácticas, es la separación del código por responsabilidades. Pues la inyección de dependencias parte de ahí. En el código de una aplicación con OOP (Programación Orientada a Objetos) tenemos una posible separación del código en dos partes, una en la que creamos los objetos y otra en la que los usamos.  

Existen patrones como las factorías que tratan esa parte, pero la inyección de dependencias va un poco más allá. Lo que dice es que los objetos nunca deben construir aquellos otros objetos que necesitan para funcionar. Esa parte de creación de los objetos se debe hacer en otro lugar diferente a la inicialización de un objeto. 