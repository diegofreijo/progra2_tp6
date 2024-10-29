# TP6 de Programación de Video Juegos 2: Combate, Sigilo, IA

## Metodología

|                        |                                   |
| ---------------------- | --------------------------------- |
| Integrantes por grupo: | 1                                 |
| Se aprueba con         | 6                                 |
| Fecha de entrega       | Jueves 31 de Octubre, 23:59 hs |
| Fecha de re-entrega    | Jueves 07 de Noviembre, 23:59 hs |


### Objetivos

- Implementar la IA de un enemigo simple
- Implementar las mecánicas de combate que el juego necesite

Recuerden que, por lo general, la solución más simple es la mejor.

----

## Entrega

### Código

Todo lo van a resolver en un repositorio de GitHub. Tiene que haber una `tag` que se llame `tp6`. Ese commit es el que voy a corregir.

 Antes de la fecha limite me tienen que mandar el link a la tag `tp6` por mail a <me@diegofreijo.com>.
 
----

## Requerimientos

Ya tienen un personaje que se puede mover en un nivel. Ahora necesitamos meterle dificultades agregando enemigos.

Los objetivos genéricos del TP son que implementen el sistema de combate que su juego necesite. Para eso van a tener que:

1. Actualizar la ficha técnica con la descripción del combate
2. Implementar la IA de los enemigos
3. Implementar sistemas de salud y daño con las armas que hayan
4. Implementar sistema de sigilo, si el juego lo requiere


### 1. Diseño y ficha técnica

Este punto no me parece tan importante como en el TP5. Pero igual necesito tener una idea de que sistema de combate quieren. Además les va a servir a ustedes mismos para volcar en concreto que necesitan, y que hay que implementar.

### 2. IA

No espero nada muy loco. Con que puedan tener enemigos que hagan las acciones que vimos en clase, me alcanza. O sea, cada uno debería hacer algo parecido a:

- patrulla
- cuando ve al jugador, lo persigue
- si esta a una distancia razonable del jugador, lo ataca
- si pierde de vista al jugador, vuelve a patrullar

### 3. Combate

Hay mucho de esto que ya implementaron en el Space Invaders. Necesitan que tanto el jugador como los enemigos tengan cierta salud, y que puedan ser dañadas con los ataques que existen. 

Ciertos juegos pierden el suspenso cuando el jugador se da cuenta que el enemigo es "matable". Así que si su juego lo requiere, pueden hacer un enemigo que no se pueda matar.

### 4. Sigilo

Algunos de ustedes eligieron un sistema de armas mas simple para compensar por el lado del sigilo. De ser así, ahora es el momento de implementarlo.

La lógica del sigilo se implementa en la IA. El código que permite que el jugador se pueda esconder es el mismo código que maneja los sentidos del NPC. O sea, que tan bien lo ven o escuchan al jugador. Lo mismo aplica para el tamaño de los triggers que están involucrados en los sentidos del NPC.

Los que se focalizaron en un juego de acción, pueden ignorar cualquier cosa relacionada al sigilo.
