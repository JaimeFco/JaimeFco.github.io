---
title: Propuesta de Modernización del Transporte Público en Guanajuato.
tags: [Transport, Optimal, Social, Design, Politics]
style:
color: success
description: Realizo una propuesta para mejorar el transporte público en mi ciudad natal, con la finalidad de presentarla ante gobierno municipal y la población en general.

---

En mi ciudad natal, Guanajuato, desde hace tiempo que contamos con un sistema de transporte público que ha quedado completamente desactualizado a las tendencias globales, y que cada día que pasa aumenta su déficit tecnológico. Las unidades apenas han cambiado desde que soy usuario del sistema (10 años aproximadamente), siguen siendo unidades de diesel con 2 filas de asientos a cada lado, dos puertas ubicadas a la derecha de la unidad y que carecen de accesibilidad para personas con discapacidad motriz. El método de pago sigue siendo de moneditas que pagas al conductor al abordar la unidad, sin posibilidad de transferencia, con rutas largas que te llevan de un lugar a otro de la ciudad, rutas que no se encuentran en ningún mapa, y sin una frecuencia clara que permita planear los traslados. Digo, quien tenga duda que busque en Google Maps las rutas a ver si las encuentra.

> A mis lectores habituales, les pido una disculpa, pero este post estará enfocado a los habitantes de mi ciudad. Sin embargo, puede que en tu lugar también se tenga un problema similar y mis referencias puedan ayudarte a hacer una propuesta similar. Siéntete en la libertad de tomar las ideas que gustes.

Bien, en días pasados, la comisión del Ayuntamiento encargada del transporte, hizo a bien en realizar una consulta pública para que la población pudiera ser parte de la solución a los diversos problemas. Llevaba ya algún tiempo pensando en la renovación del sistema y esta convocatoria fue una oportunidad que no dejé pasar. Así que me puse manos a la obra y redacté una propuesta que me gustaría discutir en esta entrada de mi blog.

El punto de partida para evaluar el sistema fue un estudio del sistema de transporte elaborado en 2018, donde se muestra la situación de aquél entonces. Si me lo preguntan, los problemas crecieron en el último año debido a alteraciones en las rutas que hablaré más adelante.

El resto del post se divide como sigue:

Primer hago un análisis del tramado de las rutas y críticas que se le pueden hacer considerando investigación reciente en el área. En especial, me centro en la idea de acortar el recorrido de las rutas y eliminar, en la medida de lo posible, los circuitos. En la segunda sección abordo el problema de las paradas, donde realizo una propuesta de puntos de transferencia y problemas del sistema actual que se pueden solucionar con un sitema integrado de transporte (aquel donde todo el sistema de transporte actua como uno solo).

En un segundo post que publicaré más adelante, abordaré algunas ideas de cómo se puede llegar a esta propuesta y qué otras opciones se pueden considerar para enriquecerla.

## Análisis de las rutas

De acuerdo al Programa de Movilidad del Municipio de Guanajuato, Capítulo I del 2018, el servicio público de transporte de pasajeros contaba con un total de 50 rutas, cuya gráfica se despliga a continuación:

![rutas](https://i.ibb.co/Bs83fgn/rutas.png)

Un lector no familiarizado con mi ciudad podrá notar, primero, que las calles son irregulares, lo cual presenta un desafío para la planeación de rutas; en segundo lugar se observa que varias rutas pasan por los mismos lugares, lo cual dificulta la lectura del mapa. Esto nos lleva a preguntarnos cómo es que están estructuradas las rutas existentes. El sistema de transporte actual está enfocado en proporcionar rutas que privilegian reducir el número de transbordajes por medio de rutas que parten de un punto y te llevan a otro. Este enfoque tiene sentido pues, de acuerdo al estudio previamente mencionado, existen más de 45 concesionarios que proporcionan su servicio de forma independiente, unos participando con un camión y otros con más de 20, sumándo un parque de cerca de 200 unidades divididas en 50 rutas.

Esta forma de organizar presenta la ventaja de no tener que transbordar y pagar dos o más pasajes, en cambio presenta algunas desventajas. La primera, y la más evidente, es la poca legibilidad que tiene el mapa de rutas, un diseño algo complejo que impide su comprendimiento y aleja a usuarios eventuales y primerizos del sistema. Lo segundo, es que bajo este esquema, las rutas del transporte tienen una longitud considerable. De acuerdo al estudio, la longitud del recorrido de las rutas tiene un promedio de **26.88 km.** con una desviación estándar de 14.7 km. De esto podemos concluir que hay una gran variabilidad de distancias entre las rutas, pero que en general presentan una distancia de recorrido grande. Aún si se considera solo las rutas de modalidad urbana, se tiene un promedio de 16.2 km. de recorrido.

¿Por qué nos importa la longitud del recorrido y la simplicidad de la maraña de rutas? Porque impacta directamente a la predictibilidad del tiempo de recorrido, a la imposibilidad de planear frecuencias *ad hoc* al tramo de la ruta que se maneja y al poco aprovechamiento del número de unidades. Voy a desmembrar cada punto.

Todo el mundo sabe que cuando se nos hace tarde el universo pareciera conspirar en nuestra contra, y lo que en una mañana fue un retraso de 5 minutos, puede convertirse en un retraso de una hora por la tarrde. Esto se debe, en gran medida, a que los imprevistos, que generan los retrasos, son acumulables. Estoes, los pequeños retrasos se van sumando al "atraso total", de forma tal que si consideramos que los imprevistos suceden de forma aleatoria a lo largo del tiempo, **entre más tiempo pasa**, mayor es la probabilidad de que tengamos más retrasos que abonen al problema. Este sistema es completamente análogo a las rutas de camión, pues para una correcta planeación de las frecuencias de los camiones, nos gustaría minimizar el número de imprevistos que le suceden a nuestro camiones. Entre mayor sea la longitud de la ruta, y por tanto mayor el tiempo que se hace en recorrerla, la probabilidad de acumular imprevistos es grande. Es por eso que las rutas con recorridos largos, suelen tener tiempos de recorrido menos predecibles.

Siguiendo con esta serie de analogías, ahora imaginemos que se cuenta con un parque vehicular de 20 camiones y tenemos 10 rutas que servir, si quisiéramos repartir las unidades en las rutas a partes iguales, podríamos asignar 2 camiones a cada ruta. Si simplificamos las rutas a 5, y conservamos el mismo parque vehicular, ¿de a cuántos camiones le tocarían a cada ruta? De a 4. Con este proceso logramos duplicar la frecuencia de los camiones en las rutas sin incrementar el parque vehicular. Aquí radica la idea de que un grafo más simple, por ejemplo con rutas más cortas y bien planeadas, es capaz de incrementar la frecuencia y reducir los tiempos de espera. Volviendo al ejemplo, con 5 rutas y cuatro camiones por ruta, se anda ahora más olgado de camiones por ruta, lo que permite asignar más camiones a unas rutas en ciertos momentos, y más a otras en otro momento. Cuando se tenían 10 rutas, no se contaba con mucha libertad porque cambiar un camión de ruta, ¡te dejaba un solo camión por cubriendo una ruta!

Por último, les presento otro mapa que fue tomado del mismo estudio:

![densidad-rutas](https://i.ibb.co/2F6rsgx/densidad-rutas.png)

En la imagen se aprecia la densidad de las rutas, es decir, el número de rutas que pasan por cierta ubicación. Esto muestra como la densidad es desigual en varias zonas, habiendo lugares donde la densidad de autobuses es alta, pero de forma desincronizada debido a que cada camión hace su recorrido en función de su ruta y no tanto de las demás, de forma tal que esos puntos de acumulación no presentan una frecuencia regular de autobuses. Más aún, es de esperarse que esta correlación responda a la densidad de pasajeros, lo que nos lleva a preguntarnos si sería mejor dividir las rutas en trozo más pequeños, fáciles de controlar y de predecir sus tiempos de recorridos, de forma tal que las rutas en zonas de alta densidad tengan una frecuencia elevada, mientras que las rutas con poca densidad se conecten con estas por medio de transferencias gratuitas y disminuya un poco su densidad conservando el parque vehicular. Justo en esto se centra mi propuesta.

Las rutas más cortas resuleven las desventajas que presentan las rutas largas, teniendo un precio que pagar: hacer transbordos.

¿Es esto malo?

Puede parecer containtuitivo, pero en realidad hay diversos estudios que muestran que en sistema con un buen diseño de rutas y frecuencias, es más eficiente hacer transbordajes con tiempo de espera pequeños, que esperar un tiempo considerable a que pase el que camión que nos lleva directo a nuestro destino.

Para ilustrar lo anterior, cito un artículo de un grupo de investigadores del Instituto de Estudios en Transporte de Berkeley. El artículo puede ser consultado en [este enlace](https://escholarship.org/uc/item/3996t4c6). El estudio describe los efectos de la renovación del transporte público en Barcelona, sistema que fue restructurado en 2012. Les dejo una imagen de cómo lucía el antiguo tramado de las rutas:

![barcelona_old](https://i.ibb.co/1RgrTM4/barcelona-old.png)

Es de notar el complejo tramado de las rutas. En el artículo se menciona que antes de 2012 habían 63 rutas que seguían la estrategia de "rutas directas", la misma estrategia que se usa actualmente en Guanajauto, conrutas que evitan transbordaje en la medida de lo posible. El antiguo sistema fue reemplazado gradualmente por 28 rutas nuevas. El resultado a 2018 fue el siguiente:

![barcelona_new](https://i.ibb.co/0JJKjRf/barcelona-new.png)

Podemos contemplar en las nuevas líneas un trazado más estructurado, sin rutas duplicadas y con puntos de cruce de fácil identificación.

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

Cabe aclarar que después de la elaboración del programa, justo el año pasado, se realizó un cambio de parada, de una parada terminal muy solicitada, a otra que lo es menos pero con más conexiones. Este enfoque se justificó en una transición al enfoque de transbordaje, sin embargo generó más molestias que ventajas. La nueva parada se encuentra en una zona más alejada del centro de la ciudad a donde se suele tener más demanda, y sin un sistema de libre transbordaje, ahora más personas necesitan transbordar, pero para hacerlo tienen que pagar doble pasaje. O en su defecto, algunos optan por caminar el resto de su trayecto. Esta medida afectó en mayor medida a quienes viven en las comunidades apartadas del centro, y a los adultos mayores y personas con discapacidad, quienes no tienen la alternativa de caminar a su destino y se ven forzados a transbordar.

En los ejemplos citados se hace incapié en que para obtener resultados positivos, se requiere un sistema de transbordaje libre: transbordar el número de veces que sean necesarios para llegar a tu destino, por un único precio. Implementaciones parciales podrían ser contraproducentes.

## Análisis de las paradas

Dado el análisis de las rutas, debería quedar más o menos clara la dirección que debe llevar la renovación del sistema: la creación de un Sistema Integrado de Transporte donde los usuarios puedan hacer transbordajes libremente a través de rutas más cortas que se conecten unas a otras. Es justo esas conexiones las que abordamos aquí.

Uno de los principales problemas del sistema de transporte de la ciudad es la falta de infraestructura vial. En particular, el estudio de 2018 menciona que de las más de 800 paradas de camión, solo alrededor de 180 son "oficiales", es decir, tienen una señalética que los oficializa. Incluso podemos ubicar 140 de ellos en un mapa:

<img src="https://i.ibb.co/LRpLPXB/map-bus-stops.png" alt="bus_stops" style="zoom:120%;" />

Podemos obsevar que las rutas oficiales no se distribuyen de manera uniforme en la ciudad, así que con el tiempo los usuarios han demandado nuevas paradas que actualmente constituyen más del 70 % de las paradas totales.

¿Por qué formalizar las paradas?

Para empezar, porque nos gustaría poderlas identificar en un mapa. Pero más allá, para que se le dote de la infraestructura adecuada, esto es, señalética, lugar donde se puedan orrillar los camiones, y en algunos casos un cruce peatonal.

Otra cosa que se puede hacer para mejorar el servicio, es planificar las paradas de cruce entre líneas, pues estas deberán preparase para albergar más camiones y mayor flujo de personas. Actualmente existen dos paradas en donde confluyen varias rutas. La primera es la antigua estación de trenes, que con el cambio establecido el año pasado, se convirtió en la parada con mayor afluencia. La segunda es la del puente Marlboro, donde confluyen varias rutas de la zona sur a la zona centro.

En la búsqueda de la implementación de un sistema integrado de transporte, se deben establecer las paradas de transferencia siguiendo las siguientes nociones básicas:

- Concentren varias líneas
- Confluya una o más líneas de alta demanda
- Quede cerca de centros de trabajos, locales comerciales y oficinas de gobierno, lugares a los que la población podría acudir desde la parada
- Se distribuyan de forma equitativa en la ciudad
- Exista forma de moverse de una a otra en pocas rutas

Siguiendo esas guías, la parada de la exestación y la de la Alhóndiga cumplen con dichos requisitos, a lo cual se añadiria una parada en la zona sur, zona en la que habitan más del 30 % de la población guanajuatense, una en la zona de embajadoras y otra en Marfil. Dado lo anterior, muestro en un mapa algunas propuestas de paradas de transferencia:

- Glorieta El Laurel
- Glorieta Santa Fe
- Plaza Alaïa
- Embajadoras
- Alhóndiga
- Antigua estación de ferrocarriles

![paradas_principales](https://i.ibb.co/b6x2mGs/paradas.png)

En el plan de 2018 se sugería formalizar las paradas de transferencia modal en El Laurel, Exestación y Embajadoras, complementarias a las ya existentes como Glorieta Santa Fe y Alhóndiga. Sin embargo es revelador llegar a esta sugerencia por el análisis de los datos presentados en la sección anterior. En particular se observa como las paradas corresponden a la mancha urbana y tratan de ser equidistantes con una salvedad: en la zona centro, abajo de la leyenda "Guanajuato" se encuentra una gran área densamente habitada donde podría colocarse una parada intermedia entre Embajadoras y Alhóndiga. La excepción aquí correponde a que en el centro histórico se busca evitar que confluyan varios camiones, además de que es inviable la construcción de la infraestructura necesaria.

Este último punto debe solventarse con la implementación de una ruta que conecte la zona centro con las paradas de transferencia. La solución que propongo es la creación de una ruta por el centro histórico.

![ruta_centro](https://i.ibb.co/ZSnNK4h/ruta-centro.png)

Con el trazado que se muestra en el mapa, se observa una mejor integración entre las 3 paradas de la zona centro, con una ruta exestación-embajadoras vía Alhóndiga.

Ésta ruta sería la única que pasaría por el centro histórico de la ciudad y que simplifica la gran densidad de líneas que se tiene actualmente (ver mapa de densidad de rrutas en la sección anterior).

Para continuar con las conexiones entre las paradas principales, se debe observar el otro tramo de gran acumulación de rutas: el bulevar Euquerio Guerrero. De esta zona se puede llegar a las paradas por 3 vías: una que vaya rumbo a Marfil y pase por la Glorieta del Laurel, otra que vaya directo a la Alhóndiga y una más que vaya rumbo a la presa de forma directa. No hay más entradas a la ciudad. Es por esto que todas las rutas principales quedarían así:

<img src="https://i.ibb.co/g34Lgzt/vias-principales.png" alt="rutas_principales" style="zoom:120%;" />

Una disculpa si se despliegan todas del mismo color, las pensé primero como rutas de Google Maps pero estoy mudándome a OpenStreetMaps para poder programarlas con Python. Son 5 las rutas que podríamos denominar "Troncales" y que forman el eje principal del sistema:

1. Ruta Centro Histórico (Exestación-Embajadoras vía Alhóndiga)
2. Ruta Alaïa-Alhóndiga
3. Ruta Central de Autobuses-Embajadoras (vía Presa de la Olla)
4. Ruta Embajadoras-Central de Autobuses (vía Pozuelos)
5. Ruta Glorieta Santa Fe-Exestación (vía Marfil)

Las rutas troncales propuestas cumplen con los requisitos expuestos en la sección anterior:

- El recorrido es menor al promedio de las rutas existentes
- Responden a las zonas de más demanda
- En la medida de lo posible evita circuitos
- Conecta las paradas de mayor afluencia y de donde partirán las rutas de menor afluencia llamadas "ramales"

Para ilustrar los puntos anteriores, observe que las rutas que van a La Saceda, Lomas del Padre, Villas de Guanjuato, Mártires 22 de Abril, entre otras rutas que conectan colonias de la zona sur con el centro de la ciudad, pueden ser sustituidas por la combinación de una ruta troncal y una ruta ramal que parta de una parada principal como la Glorieta Santa Fé o la plaza Alaïa, y que haga un recorrido por la colonia de interés. Con este sistema se resuelve:

- Se aumenta la frecuencia de autobuses en zonas de más demanda, al establecer solo 5 rutas troncales que trabajan de manera coordinada, en zonas donde actualmente pasan más de 20 rutas (acuérdense del ejemplo de menos rutas = mayor frecuencia)
- Para alimentar las paradas pricipales, se establecen rutas ramales que abarcan una mayor cobertura, dejando a los usuarios más cerca de sus destinos
- Perimite aumentar o disminuir la frecuencia de una forma más flexible respondiendo a la demanda de los usuarios

Este nuevo diseño de las rutas y paradas, es tentativo y lo presento para ilustrar las ventajas de un nuevo sistema integrado de transporte, pero quiero que quede claro que el número de paradas de transferencia podría incrementarse (por ejemplo con alguna intermedia ente la Glorieta El Laurel y la exestación). Un trazado definitivo debe corresponder a las demandas de movilidad de la población y a la infraestructura que se requiera, además considero que para mejorar la fácil adaptavilidad de los usuarios, propongo que las rutas urbanas actuales puedan se cubierta cubiertas con a lo más una transferencia en el nuevo sistema, y que se pueda ir de un lugar a otro de la ciudad en a lo más 2 transferencias (ruta ramal + ruta troncal + ruta ramal).

Respecto a la infraestructura, en la Glorita Santa Fé se puede acondicionar la glorieta como un lugar de transferencia, pues a pesar de la construcción de andadores, ésta sigue siendo subutilizada y bien puede dar paso a una central multimodal (más adelante hablo de esto). Otro ejemplo es la glorieta El Laurel. Al día de hoy a pesar de ser una parada con gran demanda, carece de cruces peatonales bien demarcados y de lugar amplio para el acomodo de los camiones. En contraste a estos dos lugares, la parada del centro comercial Alaïa cuentan con amplios espacios como para albergar hasta 5 camiones al mismo tiempo, pero la parada es subutilizada.

Y cuando nos referimos a "infraestructura", ¿a qué nos estamos refiriendo? Eso lo abordaré en otra ocasión, donde comparto mi experiencia de cómo lo hacen en otras ciudades donde he usado el transporte público: Quebec, Montréal, León Gto. y London, On.

En particular quedan pendientes los siguientes puntos:

## Métodos para la realización de transferencias

- Caso León y diferencias con Guanajuato
- Ciudades con un casco histórico patrimonio de la humanidad
- La clave: tecnologías a bordo
- Unidades de piso bajo

## Integración con otras propuestas de movilidad

- La importacia del uso masivo del transporte público y disminución del automóvil
- Propuesta de servicios adicionales de transporte público
  - Vías rápidas
  - Horarios nocturnos
- Propuesta de ciclovías que complementen el servicio
- Restricción de la movilidad en el centro histórico
- Posibles carriles exclusivos para el transporte público
