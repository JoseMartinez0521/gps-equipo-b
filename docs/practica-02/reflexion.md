# Reflexión - Práctica 2

## 1. ¿Qué porcentaje aproximado del sistema parece ser código propio frente a dependencias?

El inventario muestra que el repositorio contiene código propio, recursos de interfaz y componentes externos.

`Controladores` contiene 19 archivos y `Modelos` contiene 261 archivos, mientras que `Vistas` contiene 6992 archivos.

No es posible obtener un porcentaje exacto únicamente mediante el conteo de archivos, debido a que algunas carpetas pueden contener una mezcla de código, recursos y dependencias.

Por esta razón, para realizar una estimación más precisa del tamaño del sistema sería necesario separar el código desarrollado específicamente para el sistema de las bibliotecas y recursos externos.

El número total de archivos del repositorio, por sí solo, no representa necesariamente la cantidad de código propio que tendría que mantener el equipo.

## 2. ¿Qué riesgos existen al depender de librerías que el equipo no mantiene?

Las dependencias externas pueden generar problemas de compatibilidad, mantenimiento y seguridad.

Si una librería deja de actualizarse, puede ser necesario modificar el sistema cuando cambien PHP, el servidor web u otros componentes utilizados por la aplicación.

En este repositorio se identificaron componentes como `PHPMailer` y `tcpdf`, por lo que sería necesario conocer sus versiones y estado de mantenimiento antes de realizar modificaciones importantes.

Otro riesgo es que un cambio en una dependencia pueda afectar el funcionamiento de partes del sistema que dependen de ella.

## 3. ¿La arquitectura facilita o dificulta el mantenimiento? ¿Por qué?

La separación entre controladores y modelos ayuda a identificar las responsabilidades de diferentes partes del sistema.

Por ejemplo, `CarrerasC` contiene operaciones relacionadas con el procesamiento de carreras, mientras que `CarrerasM` concentra las operaciones relacionadas con el acceso a los datos.

Esto facilita localizar determinadas funciones cuando se necesita analizar o modificar una funcionalidad.

Sin embargo, la gran cantidad de archivos y componentes existentes en el repositorio puede dificultar la localización y comprensión de todas las relaciones del sistema.

Por lo tanto, la separación observada entre controladores y modelos ayuda a organizar determinadas responsabilidades, mientras que el tamaño y cantidad de componentes del repositorio representan un reto adicional para el mantenimiento.
