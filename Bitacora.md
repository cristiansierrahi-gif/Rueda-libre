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

## MiniReto 2: Estructura HTML, Jerarquía de Contenidos y Enlaces

### 1. Definición de la estructura base y metadatos
- **Configuración del documento:** Declaración del tipo de documento con `<!DOCTYPE html>` y configuración del idioma principal en español (`lang="es"`).
- **Metadatos corporativos (`<head>`):**
  - Codificación de caracteres estándar (`UTF-8`).
  - Configuración de la ventana gráfica para visualización adaptable (`viewport`).
  - Título oficial de la página e inclusión del icono (`favicon`).

### 2. Jerarquía de contenidos y encabezados
- **Estructura semántica de títulos:** Uso estricto de un único encabezado principal de nivel uno (`<h1>`), y subtítulos organizados jerárquicamente (`<h2>` y `<h3>`) para seccionar el contenido (bienvenida, quiénes somos, servicios, requisitos, beneficios y taller básico).

### 3. Implementación de listas HTML
- **Listas ordenadas (`<ol>`):** Implementadas para detallar los requisitos e instrucciones secuenciales obligatorias para los usuarios que desean realizar un alquiler de bicicletas.
- **Listas desordenadas (`<ul>`):** Utilizadas para agrupar los servicios principales de la empresa.

### 4. Integración de recursos multimedia (Imágenes)
- **Rutas y atributos:** Inserción del logotipo y de las fotografías requeridas por el cliente.
- **Accesibilidad visual:** Incorporación obligatoria del atributo descriptivo `alt` en cada recurso gráfico para garantizar la correcta interpretación del contenido visual.

### 5. Configuración de enlaces corporativos
- **Enlaces internos por ancla (`#`):** Creación de un menú de navegación rápido basado en identificadores (`id`) para saltar de forma fluida entre las secciones de la misma página y el botón de retorno superior (`#inicio`).
- **Enlaces absolutos externos:** Inserción del enlace de ubicación directa de la sede física en Google Maps, configurado de manera segura (`target="_blank" rel="noopener noreferrer"`).
- **Enlaces de correo electrónico (`mailto:`):** Habilitación del canal de contacto directo de atención al cliente mediante el protocolo de correo corporativo (`hola@ruedalibre.example`).