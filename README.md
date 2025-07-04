# Actividad 12 y tarea 10

**Autor:** Jorge Arcibar

## Descripción General del Proyecto

Este repositorio contiene el desarrollo de dos actividades principales que demuestran habilidades en el desarrollo web moderno con Laravel y Vue.js:

1.  **Integración de AdminLTE y Migración de la Actividad 11:** Se ha integrado el panel de administración AdminLTE en una aplicación Laravel, y se ha migrado el contenido del proyecto anterior (Actividad 11: "Sistema de Seguimiento y Gestión de Órdenes") a este nuevo entorno administrativo.
2.  **Aplicación Vue.js de Chistes de Chuck Norris (Tarea 10):** Se ha desarrollado una aplicación web sencilla utilizando el framework JavaScript Vue.js para mostrar una lista de chistes, implementando componentes y un diseño responsivo con Bootstrap.

## Funcionalidades Implementadas

### Parte 1: Integración de AdminLTE y Contenido de la Actividad 11

* **Integración de AdminLTE:** El panel de administración AdminLTE ha sido integrado en el proyecto Laravel, proporcionando una interfaz de usuario moderna y responsiva.
* **Vistas de Autenticación con AdminLTE:** Las páginas de login y registro utilizan ahora el diseño y los estilos de AdminLTE.
* **Dashboard Personalizado:** El dashboard principal para usuarios autenticados (`/dashboard`) ha sido configurado para mostrar un diseño de AdminLTE con tarjetas de ejemplo.
* **Menú Lateral Personalizado:** El menú de navegación lateral de AdminLTE ha sido modificado para incluir las opciones de la Actividad 11: "Inicio", "Fotos" y "Contacto".
* **Migración de Contenido de la Actividad 11:**
    * Las vistas de "Inicio", "Fotos" y "Contacto" de la Actividad 11 han sido adaptadas y colocadas dentro del panel de AdminLTE, manteniendo su contenido original.
    * Se han creado rutas específicas (`/home-actividad11`, `/photos-actividad11`, `/contact-actividad11`) para acceder a estas secciones dentro del panel.
* **Pie de Página Personalizado:** El pie de página del panel de AdminLTE ha sido editado para incluir la información del autor y enlaces relevantes.
* **Página Pública de Seguimiento de Órdenes:** Se ha mantenido una página de inicio pública (`/`) con un formulario de búsqueda de órdenes, que no requiere autenticación.

### Parte 2: Aplicación Vue.js de Chistes de Chuck Norris (Tarea 10)

* **Visualización de Chistes:** Muestra una lista predefinida de chistes de Chuck Norris.
* **Componente `<chuck-card>`:** Los chistes se renderizan utilizando un componente Vue.js personalizado, que encapsula la lógica de visualización de cada tarjeta.
* **Uso de `props`:** Los datos de cada chiste (`icon_url` y `value`) se pasan al componente `<chuck-card>` mediante propiedades (`props`).
* **Diseño Responsivo con Bootstrap:** La aplicación utiliza el sistema de grid de Bootstrap para mostrar 3 tarjetas por línea en pantallas grandes y 1 tarjeta por línea en pantallas pequeñas, asegurando una experiencia de usuario óptima en diferentes dispositivos.
* **Estilo Estético y Minimalista:** Incorpora un diseño limpio y agradable mediante CSS.

## Cómo Ejecutar el Proyecto

Este repositorio contiene dos partes principales: la aplicación Laravel (para AdminLTE y la Actividad 11) y la aplicación Vue.js (Tarea 10).

### Para la Aplicación Laravel (AdminLTE / Actividad 11)

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/JorgeGAR22/Actividad12.git](https://github.com/JorgeGAR22/Actividad12.git)
    ```
2.  **Navegar al directorio del proyecto:**
    ```bash
    cd Actividad12
    ```
3.  **Instalar dependencias de Composer:**
    ```bash
    composer install
    ```
4.  **Generar la clave de la aplicación:**
    ```bash
    php artisan key:generate
    ```
5.  **Instalar dependencias de NPM y compilar assets:**
    ```bash
    npm install
    npm run dev
    ```
    *(Mantén `npm run dev` ejecutándose en una terminal separada para que los estilos de AdminLTE se apliquen correctamente.)*
6.  **Iniciar el servidor de desarrollo de Laravel:**
    ```bash
    php artisan serve
    ```
7.  **Acceder a la aplicación Laravel:**
    * **Página Pública (Seguimiento de Órdenes):** Visita `http://127.0.0.1:8000/` en tu navegador web.
    * **Panel de Administración (Login):** Visita `http://127.0.0.1:8000/login`. Puedes registrar un nuevo usuario o usar las credenciales por defecto si has ejecutado los seeders (ej. `admin@example.com` / `password`).

### Para la Aplicación Vue.js (Tarea 10)

La aplicación Vue.js es un archivo HTML independiente dentro de este mismo repositorio.

1.  **Navegar al directorio de la aplicación Vue.js:**
    ```bash
    cd Actividad12/ChuckJokesVue
    ```
2.  **Abrir el archivo `index.html`:**
    Simplemente abre el archivo `index.html` en tu navegador web preferido. No se requiere un servidor web (como Apache o Nginx) ni Node.js para ejecutar esta aplicación, ya que Vue.js se carga directamente desde un CDN.

## URL del Proyecto en GitHub

[https://github.com/JorgeGAR22/Actividad12](https://github.com/JorgeGAR22/Actividad12)
