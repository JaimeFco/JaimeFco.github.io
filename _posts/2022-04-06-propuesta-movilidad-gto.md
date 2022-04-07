---
title: Modernización del Transporte Público en Guanajuato.
tags: [Transport, Optimal, Social, Design, Politics]
style:
color: info
description: Realizo una propuesta para mejorar el transporte público en mi ciudad natal, con la finalidad de presentarla ante gobierno municipal y la población en general.

---

# Propuesta de Modernización del Transporte Público en Guanajuato

En mi ciudad natal, Guanajuato, hemos cargado con un problema de movilidad que ha quedado completamente desactualizado a las tendencias globales y que cada día que pasa aumenta su déficit tecnológico. Las unidades apenas han cambiado desde que soy usuario del sistema (10 años aproximadamente), siguen siendo unidades de diesel con 2 filas de asientos a cada lado, dos puestas ubicadas a la derecha de la unidad y poco adaptados para personas con discapacidad motriz. El méetodo de pago sigue siendo moneditas que pagas al conductor al abordar, sin posibilidad de transferencia, con rutas largas que te llevan de un lugar a otro de la ciudad, rutas que no se encuentran en ningún mapa, y sin una frecuencia clara que permita planear los traslados.

A mis lectores habituales, les pido una disculpa, pero este post estará enfocado a los habitantes de mi ciudad. Sin embargo, puede que en tu lugar también se tenga un problema similar y mis referencias e ideas puedan ayudarte a hacer una propuesta similar. Siéntete en la libertad de tomar las ideas que gustes.

Bien, en días pasados, la comisión del Ayuntamiento encargada del transporte, hizo a bien en realizar una consulta pública para que la población pudiera ser parte de la solución a los diversos problemas. Llevaba ya algún tiempo pensando en la renovación del sistema y esta convocatoria fue una oportunidad que no dejé pasar. Así que me puse manos a la obra y redacté una propuesta que discuto en esta entrada de mi blog, esperando sus comentarios.

Mi punto de partida fue un estudio del sistema de transporte elaborado en 2018, donde se muestra la situación que guardaba el sistema en aquél entonces. Si me lo preguntan, los problemas crecieron en el último año debido a alteraciones en las rutas que hablaré más adelante.

El resto del post se divide como sigue:

Primer hago un análisis del tramado de las rutas y críticas que se le pueden hacer considerando investigación reciente en el área. En especial, me centro en la idea de acortar el recorrido de las rutas y eliminar, en la medida de lo posible, los circuitos. En la segunda sección abordo el problema de las paradas, donde realizo una propuesta de puntos de transferencia y problemas del sistema actual que se pueden solucionar con un sitema integrado de transporte (aquel donde todo el sistema de transporte actua como uno solo). Para finalizar, presento algunas ideas de cómo se puede llegar a esta propuesta y qué otras opciones se pueden considerar para enriquecerla.

## Análisis de las rutas

De acuerdo al Programa de Movilidad del Municipio de Guanajuato, Capítulo I del 2018, el servicio público de transporte de pasajeros contaba con un total de 50 rutas, cuya gráfica se despliga a continuación:

![rutas](https://i.ibb.co/Bs83fgn/rutas.png)

Un lector no familiarizado con mi ciudad podrá notar, primero, que las calles son irregulares, lo cual presenta un desafío para el problema que nos ocupa; en segundo lugar se observa que varias rutas pasan por los mismos lugares, lo cual dificulta la lectura del mapa. ¿Cómo es que están estructuradas estas rutas? El sistema de transporte actual está enfocado a proporcionar rutas que privilegian reducir el número de transbordajes por medio de rutas que te llevan de un punto a otro de la ciudad. Este enfoque tiene sentido pues, de acuerdo al estudio previamente mencionado, existen más de 45 concesionarios que proporcionan su servicio de forma independiente unos de otros, unos con un camión y otros con más de 20, sumándo un parque de cerca de 200 unidades divididas en 50 rutas.

Esta forma de organizr presenta la ventaja de no tener que transbordar y pagar dos o más pasajes, en cambio presenta algunas desventajas. La primera, y la más evidente, es la poca legibilidad que tiene el mapa de rutas, un diseño algo complejo que impide su comprendimiento y aleja a usuarios eventuales y primerizos del sistema. Lo segundo, es que bajo este esquema, las rutas del transporte tienen una longitud considerable. De acuerdo al estudio, la longitud del recorrido de las rutas tiene un promedio de **26.88 km.** con una desviación estándar de 14.7 km. De esto podemos concluir que hay una gran variabilidad de distancias entre las rutas, pero que en general presentan una distancia de recorrido grande. Aún si se considera solo las rutas de modalidad urbana, se tiene un promedio de 16.2 km. de recorrido. 

¿Por qué nos importa la longitud del recorrido y la simplicidad de la maraña de rutas? Porque impacta directamente a la predictibilidad del tiempo de recorrido, a la imposibilidad de planear frecuencias ad hoc al tramo de la ruta que se maneja y al poco aprovechamiento del número de unidades. Voy a desmembrar cada punto.

Todo el mundo sabe que cuando se nos hace tarde el universo pareciera conspirar en nuestra contra, y lo que en una mañana fue un retraso de 5 minutos, puede convertirse en un retraso de una hora por la tarrde. Esto se debe, en gran medida, a que los imprevistos, que generan los retrasos, son acumulables. Estoes, los pequeños retrasos se van sumando al "retraso total", de forma tal que si consideramos que los imprevistos suceden de forma aleatoria a lo largo del tiempo, **entre más tiempo pasa**, mayor es la probabilidad de que tengamos más retrasos que abonen al problema. Este sistema es completamente análogo a las rutas de camión, pues para una correcta planeación de las frecuencias de los camiones, nos gustaría minimizar el número de imprevistos que le suceden a nuestro camiones. Entre mayor sea la longitud de la ruta, y por tanto mayor el tiempo que se hace en recorrerla, la probabilidad de acumular imprevistos es grande. Es por eso que las rutas con recorridos largos, suelen tener tiempos de recorrido menos predecibles. 

Siguiendo con esta serie de analogías, ahora imaginemos que se cuenta con un parque vehicular de 20 camiones y tenemos 10 rutas que servir, si quisiéramos repartir las unidades en las rutas a partes iguales, podríamos asignar 2 camiones a cada ruta. Si simplificamos las rutas a 5, y conservamos el mismo parque vehicular, ¿de a cuántos camiones le tocarían a cada ruta? De a 4. Con este proceso logramos duplicar la frecuencia de los camiones en las rutas sin incrementar el parque vehicular. Aquí radica la idea de que un grafo más simple, por ejemplo con rutas más cortas y bien planeadas. Además, como ahora andas más olgado de camiones por ruta, puedes asignar más camiones a unas rutas en ciertos momentos, y más a otras. Cuando se tenian 10 rutas, no tenías mucha libertad porque un cambio te dejaba un solo camión por ruta.

Por último, centremos ahora en este otro mapa que fue tomado del mismo estudio:

![densidad-rutas](https://i.ibb.co/2F6rsgx/densidad-rutas.png)

En la imagen se aprecia la densidad de las rutas, es decir, el número de rutas que pasan por cierta ubicación. Esto muestra como la densidad es desigual en varias zonas, habiendo lugares donde la densidad de autobuses es alta, pero de forma desincrinizada debido a que cada camión hace su recorrido en función de su ruta y no tanto de las demás, de forma tal que esos puntos de acumulación no presentan una frecuencia regular de autbuses. Más aún, es de esperarse que esta correlación responda a la densidad de pasajeros, lo que nos lleva a preguntarnos si sería mejor dividir las rutas en trozo más pequeños, fáciles de controlar y de predecir sus tiempos de recorridos. 

Por ejemplo, podríamos considerar la creación de rutas en zonas de alta densidad que tengan una frecuencia elevada, mientras que las rutas con poca densidad se conecten con estas por medio de transferencias gratuitas. Justo en esto se centra mi propuesta.

Las rutas más cortas resuleven las desventajas que presentan las rutas más largas a un módigo precio: hacer transbordos. ¿Es esto malo?

Puede parrecer containtuitivo, pero en realidad hay diversos estudios que muetran que bajo un buen diseño de rutas y frecuencias, es más eficiente hacer transbordajes com tiempo de espera pequeños, que esperar un tiempo considerable a que pase el que camión que nos lleva directo a nuestro destino.

Para ilustrar lo anterior, cito un artículo de un grupo de investigadores del Instituto de Estudios en Transporte de Berkeley. El artículo puede ser consultado en [este enlace](https://escholarship.org/uc/item/3996t4c6). El estudio describe los efectos de la renovación del transporte público en Barcelona, sistema que fue restructurado en 2012. Les dejo una imagen de cómo lucía el antiguo tramado de las rutas:

![barcelona_old](https://i.ibb.co/1RgrTM4/barcelona-old.png)

Es de notar el complejo tramado de las rutas. En el artículo se menciona que antes de 2012 habían 63 rutas que seguían la estrategia de "rutas directas", la misma estrategia que se usa actualmente en Guanajauto, conrutas que evitan transbordaje en la medida de lo posible. El antiguo sistema fue reemplazado por 28 rutas nuevas y 20 complementarias que se conservaron del tramado original. El resultado en 2018 fue el siguiente:

![barcelona_new](https://i.ibb.co/0JJKjRf/barcelona-new.png)

Podemos contemplar en las nuevas líneas un trazado más estructurado, sin rutas duplicadas y con puntos de curce de fácil identificación.

El artículo menciona que en 2015, con apenas 13 rutas nuevas, los resultados de la renovación fueron muy positivos. En particular se concluye que 

- Los pasajeros tuvieron menos aversión a los transbordajes que lo que se supone con frecuencia en las prácticas de planeación de las rutas.
- La red basada en transferencias atrajo a más usuarios pues se vió un incremento en la demanda de las rutas nuevas cuendo se comparó con las antiguas.
- Disminuye el tiempo de espera a la mitad (de 12.3 minutos a 6.18), sin aumentar el número de unidades, que de hecho disminuye de 761 a 573.

Algo muy destacado, es que las rutas del sistema de Barcelona, tienen una longutd promedio de entre 8 y 9 kilómetros. Claramente por debajo de, incluso, las rutas más cortas de Guanajuato.

En la misma dirección transitó Seúl en 2004, cuyo sistema recordaba mucho al de Guanajuato, con rutas que atravesaban el centro de la ciudade iban de un punto suburbano a otro. Dicho sistema fue divido en rutas internas y rutas externas conectadas entre sí:

![seoul](https://i.ibb.co/fCz2ywy/seoul.jpg)

El cambio fue muy positivo. De acuerdo con el sitio web [Reinventing Transport](https://www.reinventingtransport.org/2019/04/simplify-and-connect.html?m=1), este cambio disminuyó la competencia por el pasaje, estabilizó los tiempos de espera, redujo el cosoto operacional y el tráfico en la ciudad.

Con estos dos casos de éxito se ilustra la idea de cómo a veces menos es más. Rutas más cortas es ls clave. 

Ahora, si no se quiere ver ejemplos externos, los mismos autores del Programa de Movilidad del Municipio de Guanajuato: Capítulo I, ya menciona que "el prolongamiento de las rutas y exceso de viajes hacen que se reduzca la eficiencia operacional de la ruta."

Como nota al margen, el año pasado se realizó un cambio de parada, de una parada terminal muy solicitada, a otra que lo es menos pero con más conexiones. Este enfoque se justificó en una transición al enfoque de transbordaje, sin embargo sin un sistema de libre transbordaje, el efecto fue contraproducente pues ahora más personas necesitan transbordar, pero para hacerlo tienen que pagar doble pasaje. O en su defecto, caminar el resto de su trayecto. Esta medida afectó en mayor medida a quienes viven en las comunidades apartadas del centro, y a los adultos mayores y personas con discapacidad, quienes no tienen la alternativa de caminar a su destino y se ven firzados a transbordar. 

Recordemos que para obtener resultados positivos, se requiere un sistema de transbordaje libre: transbordar el número de veces que sean necesarios para llegar a tu destino, por un único precio.

## Análisis de las paradas

Dado el análisis de las rutas, debería quedar más o menos claro la dirección que debe llevar la renovación del sistema: la creación de un Sistema Integrado de Transporte donde los usuarios puedan hacer transbordajes libremente a través de rutas más cortas que se conecten unas a otras. Es justo esas conexiones las que abordamos aquí.

El año pasado se intentó 

Uno de los principales problemas del sistema de transporte de la ciudad es la falta de infraestructura vial. En particular, el estudio de 2018 menciona que de las más de 800 paradas de camión, solo alrededor de 180 son "oficiales", es decir, tienen una señalética que los oficializa. Incluso podemos ubicar 140 de ellos en un mapa:

<img src="https://i.ibb.co/LRpLPXB/map-bus-stops.png" alt="bus_stops" style="zoom:120%;" />



- Propuesta de paradas de transferencia modal
- Creación de una ruta centro para turismo y para conectar paradas de transferencia modal
- Señalización de paradas y supresión de no oficiales

## Métodos para la realización de transferencias

## Integración con otras propuestas de movilidad

- La importacia del uso masivo del transporte público y disminución del uso de automóvil
- Propuesta de servicios adicionales de transporte público
  - Vías rápidas
  - Horarios nocturnos
- Propuesta de ciclovías
- Restricción de la movilidad en el centro histórico
- Posibles carriles exclusivos para el transporte público





