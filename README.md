# 6 Meses Viajando Juntos ✈️💕

Una versión especial de [Ask-out-your-Valentine](https://github.com/CodeKageHQ/Ask-out-your-Valentine), adaptada para celebrar un **6º mes de aniversario** con temática de **viajes**.

Inspirado en la idea original de [@mewtru](https://instagram.com/mewtru).

## ¿Qué hace?

Una experiencia web interactiva que pregunta: **"¿Quieres seguir viajando conmigo 6 meses más? ✈️💕"**.

- **Botones interactivos**: el botón "Sí" crece cada vez que se intenta pulsar "No", con mensajes cada vez más dramáticos y viajeros.
- **Pases de abordar**: la tarjeta principal tiene estilo de *boarding pass*, con sellos, perforaciones y motivos de viaje.
- **Avión animado**: un avión cruza la pantalla de fondo y hay emojis flotantes.
- **Imágenes temáticas**: cada "No" cambia la imagen por una foto de viaje (placeholders remotos).
- **Confeti**: un "Sí" celebra la respuesta con confeti y el mensaje "¡Nos vamos de aventura! 💕✈️".
- **Línea de tiempo "6 meses de recuerdos"**: seis tarjetas editables, una por mes, para ir guardando sus recuerdos.

## Cómo funciona

1. Se muestra una imagen y la pregunta inicial.
2. Cada "No" cambia la imagen, agranda el botón "Sí" y actualiza el texto del botón "No".
3. Un "Sí" dispara el confeti, cambia el mensaje y oculta los botones.

## Personalización

### Textos
Edita el arreglo de mensajes del botón "No" y el texto final dentro de `index.html` (bloque `<script>`), así como la pregunta en la etiqueta `<h2 id="valentineQuestion">`.

### Imágenes
Por defecto se usan placeholders remotos de [LoremFlickr](https://loremflickr.com/) (con palabras clave como `travel,airplane`, `beach,trip`, `passport`, etc.). Para usar fotos reales:

1. Crea una carpeta `images/`.
2. Añade tus fotos (por ejemplo `image1.jpg` … `image7.jpg`).
3. En `index.html`, reemplaza las URLs del arreglo `imagePaths` (y el `src` inicial de `<img id="imageDisplay">`) por rutas locales, por ejemplo `./images/image1.jpg`.

### Línea de tiempo
Las seis tarjetas de la sección **"6 meses de recuerdos"** son placeholders. Sustituye el texto de ejemplo de cada mes por sus recuerdos reales.

## Uso

No requiere instalación: Tailwind CSS se carga por CDN y el JavaScript está embebido.

```bash
open index.html
```

## Tecnologías

- HTML5
- Tailwind CSS (CDN)
- JavaScript
- [canvas-confetti](https://www.npmjs.com/package/canvas-confetti)

## Licencia

Este proyecto es open source y está disponible bajo la [Licencia MIT](LICENSE).

¡Felices 6 meses juntos! Sigamos viajando 💕✈️.
