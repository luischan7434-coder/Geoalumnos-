GEOALUMNOS AMIGOS 2.0

Este prototipo permite a varias personas entrar a la misma sala con una clave compartida. La ubicación está apagada por defecto y cada usuario debe pulsar Compartir mi ubicación y autorizar al navegador. Al detenerla, el servidor elimina la ubicación de ese miembro del mapa.

EJECUTAR EN WINDOWS:
1. Instala Node.js LTS desde https://nodejs.org/
2. Extrae este ZIP.
3. Abre la carpeta en Visual Studio Code.
4. Terminal > Nueva terminal.
5. Ejecuta: npm install
6. Después: npm start
7. Abre http://localhost:3000

PARA USARLO EN VARIOS CELULARES:
Necesitas publicar el proyecto completo en un servicio que ejecute Node.js y dé una URL HTTPS. Todos los amigos entran a esa URL y usan la misma clave de sala. No basta con alojar solo los archivos estáticos, porque se necesita el servidor Socket.IO.

LIMITACIONES Y PRIVACIDAD:
- No hay cuentas ni verificación de identidad: cualquiera que sepa la clave puede entrar.
- Los datos de ubicación solo viven temporalmente en memoria del servidor; no hay base de datos.
- No se rastrea en segundo plano; si se cierra la página, la conexión se pierde.
- Para uso real se necesitan cuentas, salas privadas, controles de acceso, HTTPS, aviso de privacidad y consentimiento apropiado.
- El mapa y las librerías necesitan conexión a internet.
