# Tostadero Vereda — landing de lanzamiento

Landing de una sola página para el lanzamiento de la suscripción mensual de café de especialidad de Tostadero Vereda.

## Ver la landing

Abrí `landing/index.html` para ver la versión principal. También existe una copia estática en `dist/index.html`.

## Formulario

El formulario valida los campos obligatorios, muestra el mensaje de confirmación solicitado y guarda una copia local mientras no se configure un destino externo. Para recibir reservas por email o Google Sheets, reemplazá el valor vacío de `DESTINATION_ENDPOINT` en el archivo HTML por la URL de un endpoint de Google Apps Script, Formspree u otro receptor compatible con `POST` en formato JSON.

## Publicación

El sitio es HTML, CSS y JavaScript sin dependencias de build. Para publicarlo en un hosting estático, usá la carpeta `landing` como directorio de publicación.
