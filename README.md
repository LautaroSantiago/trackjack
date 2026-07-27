# TrackJack

Endless runner 8-bits hecho con HTML5 Canvas y JavaScript vanilla, sin dependencias ni frameworks.

## Jugar

https://lautarosantiago.github.io/trackjack/

## Controles

- Espacio o flecha arriba: saltar el tren
- Flecha abajo: agachar bajo la barrera

## Como funciona

- Loop de juego con `requestAnimationFrame` y delta time, para que la velocidad no dependa del hardware.
- Colisiones por AABB (bounding box): compara bordes de rectangulos para detectar choques.
- Obstaculos generados al azar con tiempo de espera variable entre spawns.
- La velocidad aumenta de forma progresiva segun la distancia recorrida.
- El record se guarda en el `localStorage` del navegador, asi que persiste entre partidas.

## Correr en local

Abrir `index.html` directo en el navegador, no requiere servidor ni instalacion.
