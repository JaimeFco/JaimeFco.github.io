---
title: Brevísima Introducción a Redes Neuronales Artificiales
tags: [AI, ANN, Computer Science, Technology]
style:
color: info
description: Una breve, brevísima introducción a las redes neuronales, accesible para todo público
---

Para quien no me conoce, soy un joven estudiante a punto de egresar de la licenciatura en computación matemática. En los últimos años me he dedicado al estudio de una rama de la computación que intersecta con la estadística, llamada «Aprendizaje Estadístico». Dentro de este, cada vez más grande, campo de estudio, intimamente ligado a la Inteligencia Artificial, nos encontramos un conjunto particular de métodos de aprendizaje, llamado «Redes Neuronales Artificiales».

Aunque el concepto no es nuevo, pues data de, al menos, finales de 1940s con la [teoría de Hebbian](https://books.google.com/books?id=ddB4AgAAQBAJ), el concepto ha pasado por diversos cambios, años en los que las redes neuronales han tenido gran atención y periodos de tiempo en los que han sido olvidados. La más reciente revolución, que prevalece hasta nuestros días, empezó apenas a principios del siglo con el [aprendizaje profundo](https://www.cs.toronto.edu/~hinton/absps/ncfast.pdf) de la mano de Geoffrey Hinton.

En esta primera entrada voy a tratar de explicar qué rayos son las redes neuronales. Como ya había anticipado, las redes neuronales envuelven a un conjunto variado de métodos de aprendizaje, donde incluso algunas de ellas tienen poca relación entre sí. Esto hace que existan varios enfoque de las redes neuronales. Para facilitar el entendimiento, voy a estar saldando entre varios de estos enfoques, esperando que una vez quede claro uno de ellos, podamos entender el siguiente.

En lo que concierne a esta primera entrada sobre redes neuronales, me voy a restringir a una explicación más bien conceptual, sin entrar en detalles, de forma tal que sea cualquier persona, sin importar su experiencia previa, pueda llevarse algo.



Trae a tu mente a una niña de escasa edad caminando en la calle con su mamá. Mientras van caminando, la niña obervar un perro por primera vez. Nunca antes había visto uno, ni real, ni en ninguna animación. La pregunta que le hace a su mamá es la más natural de todas: ¿Qué es eso mamá? La mamá obervar al perro y se da cuenta que es un Poodle café que va muy amigablemente caminando a un lado de su dueña. «Es un perro, amor» le respode a su hija.

La niña entonces empieza a analizar al perro: Dos pedazos de piel con cabello que cuelgan a los lados, *¿Son alas? ¿Pueden volar los perros? ¿Son orejas o son dos colitas de cabello?*. La niña incluso ve un gran parecido a su osito de peluche. Mientras el perro pasa justo a un lado de ella, ladra. la niña aprende cómo suenan los perros.

Finalmente, el perro se va y la niña se queda con una sensación agradable de los perros. «Mamá, quiero un perro» dice la niña a su mamá.

Tiempo después, la mamá decide adoptar un perro Doberman. Su hija lo recibe con temor en los ojos. Eso no es un perro, los perros no son grandes, con orejas alzadas, de pelaje corto y un ladrido mucho más grave comparado con el de aquel poodle café.

Tiempo después, la niña acepta que un doberman también es un perro, y con el tiempo va aprendiendo a reconocer las caracteristicas que tiene en común los perros, de forma tal que cuando un día vió un Xoloitzcuintle, le dijo a su mamá «Mira, que curioso *perro*». Pero un buen día, la niña ve un lobo en la tele, y le dice a su mamá «Qué bonito perro mamá». La mamá le dice que ese no es un perro, sino un lobo, y le ayuda a ver en qué son diferentes de los perros.

Este proceso que siguió la niña para identificar a los perros se puede resumir en lo siguiente:

- Se le mostraron gradualemente diferentes ejemplos de perros para que la niña comprendiera las caracteristicas que estos tenían en común.
- Se le mostró ejemplos de cosas que no eran perros y se le enseñó a identificar esas características.

Este proceso idealizado del aprendizaje de una persona, nos sirve como analogía a lo que son las redes neuronales. Una red neuronal artificial es un algoritmo de aprendizaje supervisado, es decir, es un programa de computación capaz de desarrollar tareas por medio de un *entrenamiento* basado ejemplos, es decir, tu le enseñas a desarrollar una tarea, mostrandole muchos ejemplos de cómo esa tarea debe ser hecha (y tal vez cómo no).



## La caja negra

Tomemos como ejemplo la misma tarea de la niña, que es la identificación de perros en imágenes. También imaginemos, para tener un referente visual, que nuestra red neuronal es una caja negra que admite, por un lado, una imagen como entrada (como si fuera un fax), y  por el otro lado, tiene dos focos, uno verde y uno rojo. La caja, además, tiene varias perillas que podemos girar a nuestro antojo.

<img src="https://gblobscdn.gitbook.com/assets%2F-LIToAUdbcwk5_6AnVw3%2F-LUmrpMRdGmnh8y6bHVc%2F-LUmsoXNOnAexkWtudS2%2Fblackbox.png?alt=media&amp;token=b26fcf04-6559-4e9d-b222-e49777eb0b02" alt="Black-box" style="zoom:80%;" />

Para enseñarle a la caja, tenemos un paquete de fotos de perritos y de otros objetos y animales. Cada vez que nosotros metemos una imagen a la caja, esta la pasa por una maquinaria compleja controlada por las perillas, que activan un foco. Si la máquina considera que la imagen es un perro, el foco se muestra de color verde. En cambio, si piensa que no lo es, el foco se enciende rojo.

Nosotros, metemos la primera imagen de un perro a la caja, y como es de esperar, la caja no conoce a los perros y enciende el foco rojo. Nosotros no nos preocupamos y giramos las perillas hasta que el foco cambie a ser verde. Ahora, cuando metemos la misma imagen, el foco el verde. ¡Genial! Le hemos enseñado a identificar un perro, el que está en la imagen. Ahora le metemos otra imagen, ahora es un gato, y nos dice que... es un perro. Vamos, qué difícil tarea, ahora movemos un poco las perillas hasta que cambiamos el foco a rojo.

Este proceso lo siguimos haciendo hasta que hayamos procesado correctamente todas las imágenes. Más aún, le mostramos las mismas imagenes una y otra vez para hacegurarnos que con cada pequeño movimiento de perillas, no hayamos afectado el resultado de las imagenes ya procesadas.

Después de que hemos logrado que nuestra máquina clasifique correctamente una gran parte de nuestros ejemplos, decidimos probar qué tan bien funciona nuestra máquina. Para eso, consideramos nuevas imágenes, que nunca antes había visto nuestra caja y nos fijamos si la caja logra clasificarlos correctamente (algo similar al xoloitzcuintle que identificó correctamente la niña). Si nuestra caja clasifica bien muchos ejemplos nuevos, decimos que hemos entrenado satisfactoriamente nuestra caja.

Desde ya te habrás dado cuenta que hay cosas que vulven este entrenamiento muy difícil. Las perillas, por ejemplo, las estamos ajustando a ciegas, sin saber si una vuelta a la derecha empeorará o mejorará las cosas. Eso se puede corregir, cambiando nuestro foco por uno que soporte intensidades, donde al girar una perilla sepamos si el resultado mejora o empeora dependiendo de la intensidad del foco. Esto vuelve la misión del entrenamiento, mucho más fácil.

En esencia, así se construyen y entrenan las redes neuronales. Las perillas, son números que ajustamos para obtener un resultado numérico (el foco), donde 0 se lee como "No perro" y 1 se lee como "Perro"; y cualquier número intermedio nos dice que tanto piensa nuestra caja que en la imagen es o no de un perro. En la computadora, como las imagenes son simplemente tablas de números, es fácil imaginar que dentro de esta caja negra, se llevan a cabo operaciones matemáticas con esta tabla, y con esos números "perilla", parea que al final nos salga el resuktado deseado.

Todo suena bien, hasta este punto lo único que hacemos es darle a la caja un montón de números y rezar por que las operaciones de ahí adentro nos den el resultado que queremos. Pero.. ¿Qué operaciones podemos elegir de manera tal que nuestra caja sea buena clasificando?

Lo creas o no, estos modelos de aprendizaje no solo están inspirados en el método de prueba y error con el que aprendemos, sino que las operaciones que se realizan dentro de la caja, se parece ligeramente a como actuan nuestros cerebros biológicos.



## Neuronas

Vamos ahora a meternos dentro de la caja negra que hemos construido. Para ello, vamos a partir del la unidad de procesamiento en nuestro cerebro: la neurona.

En particular vamos a resaltar los aspectos en común entre una neurona artificial y una biológica para poder construir una expresión matemática.

![Neurona](https://upload.wikimedia.org/wikipedia/commons/4/44/Neuron3.png)

Las neuronas tienen la capacidad de comunicarse con precisión, rapidez y a larga distancia con otras células, ya sean nerviosas, musculares o glandulares. A través de las neuronas se transmiten señales eléctricas denominadas **impulsos nerviosos**.

Estos impulsos nerviosos viajan por toda la neurona comenzando por las **dendritas** hasta llegar a los botones terminales, que se pueden conectar con otra neurona, fibras musculares o glándulas. La conexión entre una neurona y otra se denomina **sinapsis**.

Las neuronas conforman e interconectan los tres componentes del sistema nervioso: sensitivo, motor e integrador o mixto; de esta manera, un estímulo que es captado en alguna región sensorial entrega cierta información que es conducida a través de las neuronas y es analizada por el componente integrador, el cual puede elaborar una **respuesta**, cuya señal es conducida a través de las neuronas.

La neurona artificial va a consistir de una unidad que procesa información que recibe por medio de sus dentritas, y que transmite por medio de el axón a otras multiples neuronas artificial.

De aquí podemos destacar algunas cosas que podemos recrear en una red neuronal artificial.

- *[Dendritas](https://en.wikipedia.org/wiki/Dendrites)* – En una neurona biológica, las dendritas permiten a la célula recibir señales de un gran número de neuronas vecinas con las cuales tienen conexión (>1000). Poseen quimiorreceptores capaces de reaccionar con los neurotransmisores enviados desde las vesículas sinápticas de la neurona siendo fundamentales para la correcta transmisión de los impulsos quimioeléctricos a través de la vía nerviosa. La neurona artificial podría imitar este comportamiento realizando una multiplicación por un valor que le de *peso* a la señal, ya sea una señal positiva (un peso positivo) o negativa (un peso negativo).
- *[Soma](https://en.wikipedia.org/wiki/Soma_(biology))* – En una neurona biológica, el soma actúa como una función de suma. Las señales químicas que se reciben en las dendritas, son mezcladas en el soma, creando una nueva señal. Nuestra neurona artificial puede imitar este comportamiento por medio de una función suma de todos los valores que recibimos en las dentritas, y tal vez procesarlas en otra función que nos diga si pasamos esta señal, o la retenemos.
- *[Axon](https://en.wikipedia.org/wiki/Axon)* – El axon, en una versión muy simplificada, toma la señal producida en el soma, y la distribuye  a sus células vecinas. De la misma manera, podemos imitar este comportamiento simplemente pasando esta suma de valores del soma, a las dendritas de otras células.

Así, nuestra neurona artificial tendría la siguiente forma:

<img src="https://upload.wikimedia.org/wikipedia/commons/b/b0/Artificial_neuron.png" alt="Neurona Artificial" style="zoom:150%;" />

Matematicamente, tenemos la siguiente fórmula:

$$y_k = \varphi(b_k + \sum_{j=1} ^m w_{kj}x_j)$$

donde $\{x_j\}_{j=1} ^m$ son los impulsos que entran a la neurona por las dendritas, meintras que $y_k$ es la señal que transmite la neurona a sus vecinas. Los valores desconocidos, los $w$'s, son los valores "perilla" de nuestra caja negra.



## Red Neuronal Densa

Una vez definida la neurona artificial, la red neuronal no es más que una colección de neuronas en capas, las neuronas de una capa conectadas a las de la siguiente, y así sucesivamente. A esta arquitectura se le conoce como una **red neuronal densa de tipo *feedfoward* con una sola capa oculta** (Wow! Demisiada especificidad 😜) como aquella que contiene tres capas de neuronas como en la siguiente imágen.

<img src="https://upload.wikimedia.org/wikipedia/commons/4/46/Colored_neural_network.svg" alt="Rnn" style="zoom:100%;" />

Los valores de entrada de la red neuronal, no es mas el dato que tenemos; en el ejemplo de la clasificación de perros, no es más que los pixeles de la imagen. Los datos de salida es el resultado llamado predicción o clasificación, que en nuestro caso bien puede ser un número entre $0$ y $1$ que nos indique qué tan segura esta la red de que la imagen sea de un perro.

Ya solo resta saber cómo encontrar esos pesos $w$'s. Una forma de hacerlo es minimizando el error de equivocarnos, que para los que saben matemáticas, se puede hacer usando información de la derivada de la red. Pero esta parte la dejaremos para otra entrada que estará más llena de detalles.

Como nota adicional, cabe resaltar que esta arquitectura no es la única. Hay arquitecturas que se alejan más de este enfoque biológico, como una Red Convolucional, o una Red Recurrente. Pero les reitero, ya habrá tiempo de hablar más adelante de ellas.



## Utilidades

Ya que sabemos qué demonios es una red neuronal artificial, es momento de hablar de su utilidad. Actualmente este tipo de arquitecturas te las encuentras hasta en la sopa. Cada vez que Netflix te sugiere una nueva serie basado en el contenido que has visto, en los coches autónomos para la segmentación y clasificación de objetos, se usan para análisis de imágenes médicas, para encontras medicinas, para la detección oportuna de enfermedades, están también dentrás de las aplicaciones que te hacen ver más viejo e incluso están ganandole a profesionales del Go.

Y esto, es solo una fracción del conjunto de todos los métodos de Inteligencia Artificial que existen, y que algún día, podrían rebasar al cerebro humano.
