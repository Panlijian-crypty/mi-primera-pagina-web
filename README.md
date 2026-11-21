# Mi primer sitio web publicado en GitHub Pages

Estudiante: **Pan Lijian Wong**. Programación Orientada al Usuario, UCA.

Actividad individual basada en el ejemplo del profesor [Nexxtor/ActividadSincronica19](https://github.com/Nexxtor/ActividadSincronica19). La portada muestra el nombre del estudiante en el H1. Consulta [ORIGEN.md](ORIGEN.md) para ver la fuente y el commit original.

## Sitio publicado

https://panlijian-crypty.github.io/mi-primera-pagina-web/

Repositorio: https://github.com/Panlijian-crypty/mi-primera-pagina-web

GitHub Actions confirmó el despliegue de producción el 21 de noviembre de 2026. Se comprobó la portada con el H1 «Pan Lijian Wong» y la carga del catálogo. El envío de eCampus se comprueba por separado.

## Ejecutar

Node.js 24 y npm.

```sh
npm ci
npm run dev
```

```sh
npm run build
npm run preview
```

## Publicar

El workflow `.github/workflows/deploy.yml` compila y publica en GitHub Pages al actualizar `main`. En Settings → Pages se debe seleccionar **GitHub Actions**. El nombre del repositorio se usa automáticamente como base de las rutas y los recursos. El build genera `404.html` para abrir rutas internas directamente.

## Comprobar

1. La portada debe mostrar «Pan Lijian Wong» como título principal.
2. «Cargar productos» abre el catálogo de DummyJSON.
3. Abrir un producto muestra su detalle y permite añadirlo al carrito.
4. El carrito conserva sus productos al recargar.
5. Tras una primera visita, el service worker puede recuperar los recursos y respuestas ya guardados si se pierde la conexión.


