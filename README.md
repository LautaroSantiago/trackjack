<div align="center">

# TrackJack

Endless runner 8-bits en HTML5 Canvas puro, sin frameworks ni dependencias.

[![Jugar ahora](https://img.shields.io/badge/%E2%96%B6%20JUGAR%20AHORA-e63946?style=for-the-badge)](https://lautarosantiago.github.io/trackjack/)
![HTML5](https://img.shields.io/badge/HTML5-e34f26?style=flat-square&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-f7df1e?style=flat-square&logo=javascript&logoColor=black)
![No dependencies](https://img.shields.io/badge/dependencias-0-2a9d8f?style=flat-square)

</div>

---

## Sobre el proyecto

Un personaje en patineta esquiva trenes, vigas, enemigos y bolas de fuego mientras el dia avanza hacia la noche y vuelve a amanecer. Todo el juego corre en un unico archivo HTML, sin librerias externas ni motor grafico.

GitHub no ejecuta JavaScript dentro del README, asi que el juego se juega en la version publicada con GitHub Pages (boton de arriba).

## Funcionalidades

- 3 vidas con invulnerabilidad temporal tras cada golpe
- Enemigos que disparan bolas de fuego a distintas alturas
- Trenes (saltar) y vigas altas (agachar), cada uno con su propia hitbox
- Ciclo dinamico de dia, tarde y noche con cielo interpolado en tiempo real
- Dificultad progresiva: la velocidad aumenta con la distancia recorrida
- Record persistente guardado en el navegador (`localStorage`)

## Controles

| Tecla | Accion |
|---|---|
| Espacio / Flecha arriba | Saltar |
| Flecha abajo | Agachar |

## Tecnologias

HTML5 Canvas + JavaScript vanilla. Sin React, sin librerias de fisica, sin build step.

## Como funciona

- Loop de juego con `requestAnimationFrame` y delta time, para que la velocidad no dependa del hardware.
- Colisiones por AABB (bounding box): compara bordes de rectangulos para detectar choques.
- El ciclo dia/noche interpola colores entre keyframes segun la fase del reloj interno del juego.
- Los enemigos disparan una bola de fuego a altura aleatoria (alta o baja) una vez que entran en pantalla.
- Obstaculos generados al azar con tiempo de espera variable entre spawns.

## Correr en local

Clonar el repo y abrir `index.html` directo en el navegador, no requiere servidor ni instalacion.

```bash
git clone https://github.com/LautaroSantiago/trackjack.git
cd trackjack
xdg-open index.html
```

---

## Autor

**Lautaro Subeldia**
Estudiante de la Tecnicatura Universitaria en Programacion — UTN Facultad Regional Avellaneda

[![GitHub](https://img.shields.io/badge/GitHub-LautaroSantiago-181717?style=flat-square&logo=github)](https://github.com/LautaroSantiago)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-lautaro--subeldia-0077b5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/lautaro-subeldia/)
