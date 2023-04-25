# **Diseño de Sistemas - Clase 3**
## **Testing & Test Unitarios**
*¿Qué es el Testing?*

*Testing es la verificación dinámica de la adecuación del Sistema a los requerimientos / requisitos.*

* Busca encontrar fallas en el producto.
* Busca hacerlo lo más rápido y barato posible *(eficiencia)*.
* Busca encontrar la mayor cantidad de fallas.
* Intenta no detectar fallas que en realidad no lo son.
* Pretende encontrar las fallas más importantes.

**_Una prueba es exitosa si encuentra fallas_**

### **Testing - Conceptos generales**
* **Equivocación** -> es una acción humana que produce un resultado incorrecto.
* **Defecto** -> paso, proceso o definición de un dato incorrecto. También puede considerarse como la ausencia de cierta característica.
* **Falla** -> resultado de ejecución incorrecto (o distinto al valor esperado).

*- Una equivocación lleva a uno o más defectos que estén presentes en el Código.*

*- Un defecto lleva a cero, una o más fallas.*

*- La falla es la manifestación del defecto.*

*- Una falla tiene que ver con uno o más defectos.*

* **Condiciones de prueba** -> son descripciones de situaciones que quieren probarse ante las cuales el Sistema debe responder.
* **Casos de prueba** -> son lotes de datos necesarios para que se dé una determinada condición de prueba.

### **Testing - Tipos de Test**
* Pruebas Unitarias (de caja negra y de caja blanca)
* Pruebas de Integración
* Pruebas de Aceptación de Usuario (UAT)
* Pruebas de Stress
* Pruebas de Volumen y Performance
* Pruebas de Regresión
* Pruebas Alfa y Beta

### **Tests Unitarios**
**_Los test unitarios se realizan sobre unidades de código claramente definidas_**

* Generalmente las realizan las mismas personas que construyeron el módulo que se quiere probar.
* Los módulos altamente cohesivos son los más sencillos de probar.

---

## **Componentes Stateless y Stateful**
### **Componentes Stateless**
* Un proceso, una aplicación o, genéricamente, un componente sin estado se refiere a los casos en que éstos están aislados.
* No se almacena información sobre las operaciones anteriores ni se hace referencia a ellas.
* Cada operación se lleva a cabo desde cero, como si fuera la primera vez.

**Componentes Stateless - Objetos**
* Los objetos Stateless no deberían tener estado interno; o si lo tienen, éste no debería condicionar el funcionamiento frente a las distintas peticiones que podría recibir el objeto en cuestión.
* Si pensamos a nuestros objetos Stateless, podríamos llegar a la conclusión de que ellos son reutilizables; es decir, que no dependen de otros objetos para sobrevivir, sino que tienen sentido de existencia propio.

### **Componentes Stateful**
* Las aplicaciones, los procesos o, genéricamente, los componentes con estado son aquellos a los que se puede volver una y otra vez y éstos recuerdan “quiénes somos” y “qué hicimos anteriormente”.
* Se realizan con el contexto de las operaciones anteriores, y la operación actual puede verse afectada por lo que ocurrió previamente.

**Componentes Stateful - Objetos**
* Si pensamos a nuestros objetos Stateful, podríamos llegar a la conclusión de que generalmente ellos no serían reutilizables; es decir, que por estar – al menos - levemente acoplados a algún otro objeto, no podrían servir para que otro objeto realice operaciones con ellos