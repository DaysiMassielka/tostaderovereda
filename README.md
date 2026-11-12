# Origen Club — landing de lanzamiento

Abrí `dist/index.html` para ver la landing.

El formulario valida los campos obligatorios, muestra el mensaje de confirmación solicitado y guarda una copia local mientras no se configure un destino externo. Para recibir reservas por email o Google Sheets, reemplazá el valor vacío de `DESTINATION_ENDPOINT` en `dist/index.html` por la URL de un endpoint de Google Apps Script, Formspree u otro receptor compatible con `POST` en formato JSON.
