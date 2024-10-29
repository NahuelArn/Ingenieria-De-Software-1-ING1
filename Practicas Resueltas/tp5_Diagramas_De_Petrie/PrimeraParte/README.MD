### a) Tipos de problemas que se pueden modelar con Redes de Petri
Las Redes de Petri son útiles para modelar problemas que involucran sistemas de eventos discretos, como:
1. **Sistemas de control de flujo**: por ejemplo, en procesos de manufactura y producción, donde se deben coordinar múltiples tareas.
2. **Sistemas de concurrencia**: modelan situaciones en las que múltiples procesos o recursos deben sincronizarse, como en sistemas operativos o redes de comunicación.
3. **Sistemas de gestión de recursos**: útiles para representar cómo los recursos limitados se asignan y utilizan en un sistema.
4. **Sistemas de colas y redes de transporte**: representan el flujo de elementos en un sistema, como clientes en una cola o datos en una red.
5. **Modelado de protocolos de comunicación**: simulan la transmisión de mensajes y la sincronización entre distintos componentes.

### b) Elementos de las Redes de Petri
Los elementos principales en una Red de Petri incluyen:
1. **Plazas (Lugares)**: representan condiciones o estados en el sistema. Están representadas como círculos y contienen marcas o tokens.
2. **Transiciones**: representan eventos o acciones que pueden ocurrir en el sistema y se ilustran mediante rectángulos o barras.
3. **Arcos**: conectan las plazas con las transiciones y viceversa, indicando la dirección del flujo. Los arcos definen la relación entre las plazas y transiciones, determinando cómo el sistema cambia de estado.
4. **Tokens (Marcas)**: representan el estado actual del sistema y se colocan en las plazas. El número y la distribución de tokens indican el estado de los recursos o condiciones en el modelo.

### c) Marcas o tokens
Las **marcas** o **tokens** son los elementos que permiten representar el estado de una Red de Petri en un momento dado. Se colocan en las plazas y se mueven entre ellas según las transiciones activas. Un conjunto particular de tokens en las plazas se llama **marcado** del sistema y define su estado. La cantidad de tokens en una plaza puede indicar, por ejemplo, la disponibilidad de un recurso o el cumplimiento de una condición en el sistema.

### d) Transición con salidas pero sin entradas
Una transición con salidas pero sin entradas se conoce como una **transición de generación** o **creación**. Esto significa que dicha transición puede activarse sin ninguna condición previa, y al activarse, introduce nuevos tokens en las plazas conectadas a su salida. Este tipo de transición puede representar un evento externo o el comienzo de un proceso en el sistema.

|--> 0

### e) Transición con entradas pero sin salidas
Una transición con entradas pero sin salidas se denomina **transición de consumo** o **eliminación**. Cuando esta transición se activa, consume los tokens de las plazas en sus entradas sin producir nuevos tokens en ninguna plaza. Esto puede representar la finalización de un proceso o evento que no tiene efectos posteriores en el sistema.

0 --> |