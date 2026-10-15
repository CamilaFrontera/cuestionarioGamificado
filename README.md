# ¿El software es lo tuyo?

Test vocacional con estética arcade para el stand de la **Tecnicatura Superior en Desarrollo de Software** del ISFDyT N° 125 en la Noche de los Institutos.

Los estudiantes de sexto año responden 12 situaciones cotidianas y reciben:

- su **clase de jugador** (tipo de interés dominante) y su código de 3 letras,
- su **compatibilidad con Desarrollo de Software** y el rol que podrían ocupar en un equipo,
- un **pase al salón** (o pase de invitado, si la compatibilidad es baja),
- su compatibilidad con las otras carreras del instituto: Educación Inicial, Educación Especial, Logística y Enfermería.

## Cómo funciona

El test se basa en el modelo de intereses de John Holland (RIASEC: Realista, Investigador, Artístico, Social, Emprendedor, Convencional), el mismo que usa el O*NET Interest Profiler.

- Cada opción de cada situación suma a un tipo de interés, sin mostrarlo en pantalla. El orden de las opciones se mezcla en cada partida.
- El puntaje de cada tipo es la proporción de veces que se eligió sobre las veces que apareció, relativo al tipo más fuerte.
- La compatibilidad con cada carrera se calcula con el código de interés de O*NET de la ocupación asociada, ponderando la primera letra ×3, la segunda ×2 y la tercera ×1:

| Carrera | Ocupación O*NET | Código |
|---|---|---|
| Desarrollo de Software | Software Developers (15-1252.00) | IC |
| Educación Inicial | Kindergarten Teachers (25-2012.00) | SA |
| Educación Especial | Special Education Teachers (25-2057.00) | SAI |
| Logística | Logisticians (13-1081.00) | CEI |
| Enfermería | Registered Nurses (29-1141.00) | SCI |

Con 50% o más de compatibilidad con Software se muestra el pase al salón desbloqueado.

Es un juego orientativo, no un test vocacional profesional.

## Uso en el stand

- Abrir `index.html` en un navegador (no necesita servidor ni instalación) o usar la versión publicada en GitHub Pages.
- Se puede responder tocando o con las teclas `1`–`4` / `A`–`D`.
- La pantalla de resultado vuelve sola al inicio después de 90 segundos sin uso.
- El contador de "jugadores esta noche" se guarda en el navegador de ese dispositivo.
- Se necesita internet solo para cargar las tipografías; sin conexión funciona igual con fuentes de respaldo.

## Personalizar

Las situaciones, las carreras y los textos de resultado están al principio del `<script>` en `index.html`, en las constantes `SITUACIONES`, `CARRERAS`, `TIPOS` y `ROL_SOFT`. El umbral del pase está en `UMBRAL`.