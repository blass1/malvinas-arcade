# Malvinas Arcade

Campaña arcade de tres niveles para el navegador, ambientada en la guerra de Malvinas (1982). Un solo archivo HTML, sin build ni dependencias: canvas 2D y Web Audio.

**Jugar:** abrí `index.html` en el navegador, o la versión publicada en GitHub Pages.

## Niveles

1. **Hangar Malvinas** — Sos mecánico de pista en la BAM Río Gallegos. Combustible, armamento y reparación contra reloj para despachar la escuadrilla (1:30).
2. **Estrecho de San Carlos** — Vista lateral. Un A-4B Skyhawk bombardea la flota a baja altura: por encima del radar te enganchan los misiles, por debajo de la altura de espoleta la bomba no arma. Un KC-130 te rearma. Objetivo: 8 buques.
3. **Cielo de Malvinas** — Combate aire-aire. Un Mirage IIIEA con cañones de 30 mm y bengalas contra oleadas de Sea Harrier. Objetivo: 10 derribos.

Si perdés en cualquier nivel, la campaña arranca de cero. El puntaje acumulado queda en la tabla de posiciones.

## Controles

| Acción | Teclado | Táctil |
| --- | --- | --- |
| Mover / subir y bajar | `WASD` o flechas | cruceta |
| Acción · bomba · cañones | `E` o `Espacio` | botón grande |
| Bengalas (nivel 3) | `F` o `Shift` | botón BENGALA |

## Tabla de posiciones

Fuera de claude.ai no hay backend: los puntajes se guardan en el `localStorage` del navegador de cada jugador. Para una tabla compartida hace falta un servicio externo (por ejemplo Supabase); el punto de entrada es la función `recordScore` y `loadBoard` en `index.html`.

## Publicar con GitHub Pages

1. Repo → **Settings → Pages**.
2. En *Build and deployment* elegí *Deploy from a branch*, rama `main`, carpeta `/ (root)`.
3. En un minuto queda en `https://<usuario>.github.io/<repo>/`.

## Licencia

Código propio. Los aviones, buques y sonidos están dibujados y sintetizados en código; no hay assets de terceros.
