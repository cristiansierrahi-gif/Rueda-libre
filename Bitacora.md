# Bitácora del Proyecto: Rueda Libre v1.0

## MiniReto 1: Fundamentos Web y Peticiones al Servidor

### 1. Estructura inicial del proyecto y configuración local
- **Control de versiones:** Inicialización del repositorio local con Git y creación de la estructura del proyecto.
- **Entorno de desarrollo:** Configuración del servidor local (Live Server / puerto 5500) para el desarrollo y visualización de la interfaz.

### 2. Análisis de peticiones HTTP (DevTools Network)
- **Petición local exitosa (`index.html`):**
  - **URL completa:** `http://127.0.0.1:5500/index.html`
  - **Protocolo:** HTTP/1.1
  - **Host:** `127.0.0.1`
  - **Puerto:** `5500`
  - **Ruta del recurso:** `/index.html`
  - **Método HTTP:** `GET`
  - **Código de estado:** `200 OK` (Indica que el servidor procesó la solicitud con éxito y devolvió el recurso solicitado).

- **Prueba de ruta errónea (Recurso no encontrado):**
  - **URL de prueba:** `http://127.0.0.1:5500/promociones.html`
  - **Código de estado:** `404 Not Found`
  - **Significado:** El servidor web responde con este código de error para notificar que el archivo o la ruta solicitada no existe en el directorio del servidor local.

### 3. Roles de las tecnologías web aplicadas en Rueda Libre
- **HTML:**
  - *Rol:* Cumple la función estructural y semántica del sitio web. Define los contenidos y el orden de los elementos.
  - *Ejemplo en Rueda Libre:* Las etiquetas `<header>`, `<main>`, `<section>`, `<h2>` y `<ul>` utilizadas para estructurar la sección de bienvenida y los servicios de alquiler de bicicletas.
- **CSS:**
  - *Rol:* Se encarga de la presentación visual, el diseño estético, la paleta de colores corporativos y la adaptabilidad responsive.
  - *Ejemplo en Rueda Libre:* La aplicación de variables de color en `:root` (`--verde-ruta`, `--naranja-pedal`, `--azul-noche`), el diseño con Flexbox/Grid y la carga tipográfica de Google Fonts.
- **JavaScript:**
  - *Rol:* Proporciona la capa de interactividad, dinamismo y lógica de comportamiento en el navegador del usuario.
  - *Ejemplo en Rueda Libre:* La manipulación del DOM para interacciones avanzadas o validaciones dinámicas complementarias en el formulario de reservas.