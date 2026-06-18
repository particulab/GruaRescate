# Grúa de Rescate

**Grúa de Rescate** es un minijuego educativo de física perteneciente al proyecto **EulerGames**.

El juego está desarrollado únicamente con **HTML, CSS, JavaScript y Canvas**, sin librerías externas. Todo el proyecto se encuentra en un solo archivo `index.html`, por lo que puede ejecutarse directamente en cualquier navegador moderno.

## Descripción del juego

Una grúa debe levantar una carga desde el suelo y recuperar la posición horizontal de su pluma. Para lograrlo, el jugador debe mover un contrapeso sobre el lado izquierdo de la grúa hasta compensar correctamente los torques generados por las cargas del lado derecho.

El objetivo no es adivinar ni resolver por tanteo, sino analizar los datos físicos de cada ronda, hacer el cálculo en libreta y después probar la respuesta dentro del juego.

Si el contrapeso es insuficiente, la grúa cae hacia el lado de la carga.
Si el contrapeso es excesivo, la grúa cae hacia el lado del contrapeso.
Si el equilibrio es correcto, la pluma se estabiliza en posición horizontal y la carga queda asegurada.

## Objetivo educativo

El juego permite trabajar conceptos de:

* torque;
* brazo de palanca;
* equilibrio rotacional;
* relación entre masa y distancia;
* interpretación física de un sistema mecánico;
* estimación y validación de resultados.

La filosofía de EulerGames es que el estudiante tenga que **calcular antes de actuar**. Por eso, el juego muestra los datos necesarios, pero no muestra la fórmula ni la solución antes del intento.

## Mecánica principal

Cada ronda genera un escenario diferente con valores aleatorios dentro de intervalos continuos:

* masa de la carga;
* distancia de la carga al eje;
* masa del contrapeso;
* lastre derecho fijo;
* posición ajustable del contrapeso.

El jugador debe mover el contrapeso hasta una posición adecuada y presionar el botón de prueba.

Durante el intento, la grúa se mueve usando una dinámica angular simplificada basada en:

* torque neto;
* aceleración angular;
* velocidad angular;
* amortiguamiento;
* contacto de los extremos con el suelo en caso de error.

Esto permite que los fallos pequeños produzcan movimientos suaves y los fallos grandes produzcan caídas más agresivas.

## Controles

### Teclado

* `←` mover el contrapeso hacia la izquierda en pasos de 0.10 m.
* `→` mover el contrapeso hacia la derecha en pasos de 0.10 m.
* `↑` ajuste fino hacia la izquierda en pasos de 0.01 m.
* `↓` ajuste fino hacia la derecha en pasos de 0.01 m.
* `Enter` o `Espacio` para probar el levantamiento.

### Botones en pantalla

El juego también incluye botones para mover el contrapeso, probar el intento, iniciar una nueva ronda y activar o desactivar el sonido.

## Retroalimentación

Después de cada intento, el juego muestra información sobre el resultado de la prueba, incluyendo:

* torque del lado derecho;
* torque del contrapeso;
* relación entre torques;
* diagnóstico del intento.

También se incluye un medidor visual de desviación porcentual del contrapeso:

* `0%` indica una posición correcta;
* desviación hacia la izquierda indica exceso de contrapeso;
* desviación hacia la derecha indica contrapeso insuficiente.

## Cómo ejecutar el juego

1. Descarga o clona este repositorio.
2. Abre el archivo `index.html` en cualquier navegador moderno.
3. No se requiere instalación, servidor local ni dependencias externas.

## Estructura del proyecto

```text
grua-rescate/
└── index.html
```

Todo el código del juego está contenido en el archivo `index.html`.

## Tecnologías utilizadas

* HTML5
* CSS3
* JavaScript
* Canvas API

## Estado del proyecto

Versión inicial jugable.

La versión actual incluye:

* generación aleatoria de rondas;
* vista lateral de la grúa;
* carga que se levanta desde el suelo;
* contrapeso ajustable;
* dinámica angular simplificada;
* medidor de desviación;
* retroalimentación después del intento;
* controles por teclado y botones;
* sonido opcional;
* diseño visual diurno.

## Proyecto EulerGames

EulerGames es una colección de minijuegos educativos de física y matemáticas diseñados para ejecutarse directamente en navegador.

La idea central es crear juegos simples, visuales y accesibles donde el estudiante deba razonar, calcular y comprobar sus respuestas dentro de una situación interactiva.

## Licencia

Este proyecto puede utilizarse con fines educativos.
Puedes modificarlo, adaptarlo y compartirlo citando el proyecto EulerGames.
