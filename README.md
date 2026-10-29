# PomoRoom

Un temporizador pomodoro con una habitación 3D isométrica que decoras con lo que ganas estudiando.

**App:** https://estamberry70.github.io/pomroom

## Cómo funciona

- Cada sesión de enfoque completada da **10 monedas**; rendirse cuesta **5**.
- Con las monedas compras muebles, mascotas, adornos de pared, suelos y paredes.
- La habitación sigue la hora real: amanecer, día, atardecer y noche, con clima en las ventanas.
- Tu personaje estudia en el escritorio durante la sesión y celebra en los descansos.
- Las mascotas caminan solas y duermen en su propia cama.
- El progreso se guarda en el navegador. En **Ajustes** hay un código de copia de seguridad para respaldarlo o pasarlo a otro dispositivo.

## Instalar en el teléfono

- **Android (Chrome):** menú de tres puntos → *Agregar a pantalla de inicio*.
- **iPhone (Safari):** botón compartir → *Agregar a pantalla de inicio*.

Una vez instalada abre a pantalla completa y funciona sin conexión.

## Estructura

| Archivo | Qué es |
|---|---|
| `src/pomoroom.html` | El código fuente: toda la app en un archivo (estilos, lógica y motor de dibujo). |
| `build.py` | Genera la versión instalable a partir del fuente. |
| `index.html` | La app ya construida, lo que sirve GitHub Pages. |
| `manifest.webmanifest` | Nombre, iconos y colores de la app instalada. |
| `sw.js` | Service worker: permite abrirla sin conexión. |

## Hacer cambios

Edita `src/pomoroom.html`, luego:

```bash
python3 build.py
```

Eso regenera `index.html`. Súbelo y la app se actualiza sola la próxima vez que se abra.
