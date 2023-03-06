# Evidencia-1.-Actividad-Integradora

En este documento se simula una intersección en la que están presentes cuatro semáforos, uno en cada esquina, y los vehículos avanzan en sus respectivos carriles según la dirreción en la que avanzan teniendo la posibilidd de cambiar de carriles y al llegar a la intersección pueden seguir recto o girar a la izquierda o derecha, con el objetivo de simular de la manera más realista el comportamiento ideal de los conductores en una intersección y así plantear estrategias para mejorar los tiempos de espera en los semáforos.

En este ejercio participan tres agentes distintos:
  **Pasto:** se ubica en las esquinas y únicamente *cambian de color* entre tres tonos para simular pasto.
  **Semáforos:** se encuentran en las esquinas de las intersecciones y poseen tres estados: *verde*, *ámbar* y *rojo*. Su única acción es el *cambio de color* y los realizan cada cierto tiempo sin tomar en cuenta  a los vehículos.
  **Vehículo:** se mueven a lo largo de toda la intersección y como acciones tienen: *avanzar en línea recta*, *frenar*, *dar vuelta* y *cambiar de carril*. Para que pueda avanzar un vehúculo necesita que no haya otro veículo enfrente y que su luz sea verde, para frenar detectan si hay un veículo quieto frente a ellos y que la luz sea roja, para que puedan dar vuelta necesitan estar en la intersección y que su luz sea verde y para que puedan cambiar de carril debe de no haber vehículo en la casilla diagonal de dónde se encuentra el vehículo en ese momento.

Los vehículos toman la información de los semáforos y parte de su comportamiento está condicionado al estado del mismo semáforo, así como también interactúan con otros vehúculos al tomer en cuenta su posición con respetco de sí mismos y así saber si pueden cambiar de carril, avanzar o frenar evitando choques.

El entorno consiste en la intersección, en la que en cada dirección hay seis carriles, de los cuales tres son para una dirección y los otros tres son para la dirección opuesta y al llegar a la intersección hay treintaseis casillas en las cuales se pueden mover los vehículos siguiendo en línea recta o dando vuelta de tal modo que se mantengan en el sentido correcto.

El sistema puede modificarse un poco al poder elegir la cantidad de vehículos que estarán presentes en la simulación y la cantidad de fotogramas por segundo para observar el movimiento de los vehículos. El parámetro de la cantidad de vehículos actúa directamente en cómo los otros vehículos percibirán su entorno al encontrarse rodeados de hasta ocho vehículos. Así como los tiempos de los semáforos que se pueden modificar para que duren más o menos en un estado.

Para la simulación se utiliza MESA para recrear celdas con cada uno de nuestros agentes, al iniciar la simulación se generan aleatoriamente agentes de vehículos dentro de las celdas que corresponden a las calles y un comportamiento si quieren mantenerse en el carril o no o si van a querer dar vuelta en la intersección o no. También se genera el pasto con un estado aleatorio según el color que  pueden tomar, pero este agente no condiciona el comportamiento de los vehículos.

Al simular se pueden observar cómo el sistema permite que los vehículos estén en constante movimientoo reduciendo al máximo el tiempo de espera en cada semáforo, esto es gracias al tiempo dado a cada semáforo para que se mantengan rotando los estados y no afecten de manera negativa a los vehículos. Una vez los vehículos pasan la intersección y salen del mapa regresan al lado opuesto para mantenerse en línea recta ya que solo pueden realizar los cambios de dirección una vez.

# https://github.com/RaulMurilloA/Evidencia-1.-Actividad-Integradora.git
