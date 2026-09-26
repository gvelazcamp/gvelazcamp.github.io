# gvelazcamp.github.io

Página raíz del dominio de GitHub Pages. El juego real vive en
[`gira-y-adivina-rioplatense`](https://github.com/gvelazcamp/gira-y-adivina-rioplatense),
servido en `/gira-y-adivina-rioplatense/`.

## `index.html`

Es solo una redirección a esa carpeta. Redirige por JavaScript
(`location.replace`) apenas se lee el HTML, antes de que se llegue a
pintar nada — así, si alguien abre `gvelazcamp.github.io` a secas (en
vez de la URL completa del juego), no se alcanza a ver el texto plano
"Redirigiendo a..." con el link, que antes sí se veía un instante.
El detalle completo de por qué está armado así queda como comentario
adentro del propio archivo — no tocar el `<script>` de
`location.replace()` ni el fondo oscuro sin necesidad, son los que
evitan que se note la carga.

## `.well-known/assetlinks.json`

Archivo de verificación para la app de Android (TWA,
`io.github.gvelazcamp.twa`) — tiene que vivir en la raíz del dominio,
por eso está en este repo separado y no en el del juego.
