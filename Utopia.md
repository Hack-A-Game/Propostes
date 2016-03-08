Utopia
===================


Descripción
----------
Utopia es un juego de estrategia, basado en turnos, donde el objetivo es ganar a un ejercito enemigo mediante el uso de unidades de diferentes tipos:

* Soldado
* Mago
* Arquero
* Curandero
* ...

La historia se desenvuelve en un mundo lejano, cuyo nombre recibe este juego (Utopia). El jugador estará en el papel de Abolon, un personaje del que podrá escoger su profesión (dentre los de arriba) y sobre el que recaerá salvar a su pueblo/país de la invasión de su país vecino.

El juego se compondrá de 2 tipos de escenas:

* Historia: Simple diálogo donde el jugador tendrá una intervención limitada, quizás opciones/respuestas distintas?
* Batallas:  Acción principal del juego, descrito en detalle más abajo.


Batallas
-------------

Las batallas se desarrollaran en campos divididos en cuadrados (a partir de ahora *grid*) de un tamaño NxN. Al principio de esta, el jugador podrá poner hasta un máximo de 5 personajes (quizás desbloqueables según se avanza, aunque no lo plantearía para la Hackathon) en unas posiciones iniciales determinadas.

> **Mapa:**
> 
> **Planteamiento incial**
> - Grid De N*N casillas, todas válidas y sin altura ni restricciones especiales
>
> **Avanzado** / si sobra tiempo
> - Grid de N*N casillas, con restricciones de altitud (ie. reducen movimiento), casillas invalidas, casillas con movimiento restringido (agua y parecidos)...


La batalla consiste en eliminar al contrincante, en concreto a cada una de sus unidades. Las unidades se caracterizan por:

> **Unidades:**
> 
> - **Vida**: Total de HP que tiene esta unidad
> - **Ataque**: Sea mágico, a distancia o cuerpo a cuerpo
> - **Rango**: Para las unidades de ataque a distancia, cuantos cuadrados abarca su distancia máxima
> - **Defensa**: Ante cualquier tipo de ataque (aunque, si diera tiempo y quisiéramos hacerlo bien, habría defensa mágica por separado).
> - **Velocidad**: Decide los turnos, quien ataca antes de quién.
> - **Unidades de movimiento**: Cuantos cuadrados puede moverse una unidad por turno


Así pues, ordenados por velocidad (independientemente de si son amigos o enemigos) las unidades empiezan sus turnos. Un turno puede componerse por las siguientes acciones:

> **Turnos:**
> 
> 1. **Movimiento**: Debe hacerse primero, puede moverse hasta un máximo de *unidades de movimiento*
> 2. **Atacar**: Permite reducir el HP de un enemigo. Si el ataque es cuerpo a cuerpo requiere que las unidades estén juntas, sinó que esté a en rango de ataque.
> 3. **Defender**: Si se recibe un ataque durante el siguiente turno, este se reduce en un 50% (?)

Si el jugador pierde, y por ello todas sus unidades mueren,  este ve una pantalla de "GameOver" y se le ofrece reintentar el nivel.


Imágenes
-----------
Vemos un ejemplo de 2 jugadas. En el primer turno, el soldado se mueve pero no puede atacar, porque no tiene el mago a rango. En General information se podría mostrar el HP, los movimientos restantes, etc.
![enter image description here](https://github.com/Hack-A-Game/Propostes/raw/master/Utopia-Turn1.png)
En el turno 2, el mago se mueve y, al tener a rango al soldado, le lanza un ataque mágico a distancia.
![enter image description here](https://github.com/Hack-A-Game/Propostes/raw/master/Utopia-Turn2.png)

Mejoras
----------

Si se tuviera el tiempo suficiente, se proponen las siguientes mejoras para los personajes:

* **Niveles**: Las unidades podrían tener niveles y, según subieran, obtener mejoras de HP, ataque, defensa...
* **Habilidades especiales**: Desbloqueables al subir de nivel o con objetos especiales, las unidades podrían tener ataques especiales (ie. *Bola de fuego* para el mago).
* **Historias alternativas** según las elecciones del jugador
* ...
