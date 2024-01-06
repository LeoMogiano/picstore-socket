# Servidor de notificaciones en tiempo real

Este proyecto es un servidor de notificaciones en tiempo real construido con Express y Socket.IO.

[English](./README.md) | [Español](./README.es.md) | [Français](./README.fr.md) | [日本語](./README.jp.md)

## Requisitos

- Node.js
- npm

## Instalación

1. Clona este repositorio.
2. Navega hasta el directorio del proyecto.
3. Ejecuta `npm install` para instalar las dependencias.

## Uso

Para iniciar el servidor, ejecuta `node app.js` en la terminal. El servidor comenzará a escuchar en el puerto 3030 o en el puerto especificado en tu variable de entorno `port`.

El servidor tiene dos eventos principales de Socket.IO:

- `notification`: Este evento se dispara cuando un usuario emite una notificación. Los datos de la notificación se preparan para la inserción en la base de datos y luego se emite un evento `notification_processed` con los datos de la notificación.

- `notification_user`: Este evento se dispara cuando un usuario emite una notificación de usuario. Los datos de la notificación se preparan y luego se emite un evento `notification_processed_user` con los datos de la notificación.

## Contribución

Las contribuciones son bienvenidas. Por favor, abre un issue o un pull request para sugerir cambios o mejoras.

## Licencia

Este proyecto está licenciado bajo los términos de la licencia MIT.