# Tostadero Vereda — landing de lanzamiento

Landing de una sola página para el lanzamiento de la suscripción mensual de café de especialidad de Tostadero Vereda.

## Tecnologías y servicios

- **HTML, CSS y JavaScript** para la landing, el diseño responsive y la validación del formulario.
- **Netlify** para alojar y publicar el sitio con el dominio `tostaderovereda.netlify.app`.
- **Zapier** para recibir los datos del formulario y automatizar el flujo de reservas.
- **Gmail** como destino de las notificaciones de nuevas reservas.

Flujo previsto:

```text
Formulario HTML → Zapier → Gmail
                         └→ registro o acción adicional
```

## Ver la landing

Abrí `landing/index.html` para ver la versión principal. También existe una copia estática en `dist/index.html`.

## Formulario

El formulario HTML valida los campos obligatorios y muestra el mensaje de confirmación después del envío. Para completar la integración, el botón de envío debe enviar los campos a un **Webhook de Zapier**. Zapier puede enviar automáticamente la reserva a Gmail y, si se necesita, guardarla en otra herramienta.

La URL del Webhook debe configurarse en `DESTINATION_ENDPOINT` dentro del archivo HTML. No incluyas claves, contraseñas ni tokens de Zapier en el repositorio.

## Publicación

El sitio es HTML, CSS y JavaScript sin dependencias de build. En Netlify, usá la carpeta `landing` como directorio de publicación. El repositorio contiene además una copia en `dist`.
