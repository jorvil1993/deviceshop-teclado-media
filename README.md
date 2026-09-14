# Medios remotos del teclado DeviceShop BO

Este repositorio publica los archivos que los atajos multimedia del teclado pueden
actualizar sin reinstalar la aplicación.

`media.json` es el manifiesto público. Cada entrada incluye el código del atajo,
tipo de archivo, tamaño, checksum SHA-256 y un enlace HTTPS a un asset de Release.
El teclado descarga únicamente los archivos cuya versión cambió y conserva el
último archivo válido si una descarga falla.

Para publicar un medio nuevo:

1. Sube el archivo como asset de una nueva Release.
2. Actualiza `media.json` con su URL, tamaño y SHA-256.
3. Publica el cambio del manifiesto.

No subas archivos a este repositorio sin actualizar el manifiesto.
