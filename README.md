# texas-hold'em

Texas Hold'em es una variante del póker en la que a cada jugador se le reparten dos cartas ocultas ("hole cards"). Luego, los jugadores realizan una serie de apuestas mientras se revelan cinco cartas comunitarias ("community cards"). Si queda más de un jugador cuando terminan las apuestas, se produce un "showdown", donde los jugadores muestran sus cartas. Cada jugador debe formar la mejor mano posible de cinco cartas, usando cualquier combinación entre sus dos cartas ocultas y las cinco comunitarias.

Jerarquía de manos (de mayor a menor):
 - Escalera de color (straight-flush): cinco cartas consecutivas del mismo palo.
 - Póker (four-of-a-kind): cuatro cartas del mismo rango.
 - Full house: tres cartas del mismo rango y dos de otro.
 - Color (flush): cinco cartas del mismo palo.
 - Escalera (straight): cinco cartas consecutivas.
 - Trío (three-of-a-kind): tres cartas del mismo rango.
 - Doble par (two pair): dos pares de diferentes rangos.
 - Par (pair): dos cartas del mismo rango.
 - Carta alta (high card): si no se logra ninguna de las combinaciones anteriores.

Dadas las cartas ocultas y comunitarias, implementa la función hand que devuelva un objeto con:

 - `type`: el tipo de mano (en minúsculas, por ejemplo `"pair"`, `"flush"`, etc.).

 - `ranks`: una lista con los rangos de cartas en orden descendente, usada para desempates.

Ejemplo:
```javascript
hand(["A♠", "A♦"], ["J♣", "5♥", "10♥", "2♥", "3♦"])
// Resultado: {type: "pair", ranks: ["A", "J", "10", "5"]}

hand(["A♠", "K♦"], ["J♥", "5♥", "10♥", "Q♥", "3♥"])
// Resultado: {type: "flush", ranks: ["Q", "J", "10", "5", "3"]}
```

**Nota: Para escaleras con As, solo se acepta la escalera con As alto (por ejemplo: 10, J, Q, K, A). La escalera con As bajo (A, 2, 3, 4, 5) no es válida.**

1. Haz un fork de este repositorio.

2. Implementa la función `hand` en un archivo .js dentro del repositorio (por ejemplo `index.js`).

Asegúrate de que tu código esté correctamente comentado y estructurado.
