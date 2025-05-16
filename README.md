# ClipTape - Landing Page

## Descripción
Landing page profesional para ClipTape, empresa dedicada a la venta de despachadores de cinta adhesiva. Este sitio web está diseñado para mostrar los diferentes modelos de despachadores, sus características y facilitar el contacto con los clientes potenciales.

## Tecnologías utilizadas
- HTML5
- CSS3
- JavaScript
- Bootstrap 5
- AOS (Animate On Scroll)
- Font Awesome
- Google Fonts (Outfit)

## Estructura de archivos
```
├── index.html
├── assets/
│   ├── css/
│   │   └── styles.css
│   ├── js/
│   │   └── main.js
│   └── img/
│       └── (imágenes del sitio)
└── README.md
```

## Guía de personalización

### Modificar textos
Para actualizar los textos del sitio, simplemente edita el archivo `index.html` y busca las secciones correspondientes:

- **Título y descripción**: Modifica las etiquetas meta en el `<head>` para SEO.
- **Secciones principales**: Cada sección está claramente identificada con comentarios HTML (`<!-- Nombre Section -->`)

### Cambiar imágenes
1. Reemplaza las imágenes en la carpeta `assets/img/` manteniendo los mismos nombres o actualiza las rutas en el HTML.
2. Para el logo, reemplaza el archivo `LOGO2.gif` o actualiza la ruta en todas las instancias donde aparece.

### Actualizar colores
Los colores principales se definen como variables CSS en el archivo `assets/css/styles.css`:

```css
:root {
    --primary-color: #ff6b00;
    --secondary-color: #333333;
    --accent-color: #ffc107;
    --light-color: #f8f9fa;
    --dark-color: #212529;
    /* ... */
}
```

Modifica estos valores para cambiar el esquema de colores de todo el sitio.

### Añadir o modificar modelos
Para añadir un nuevo modelo o modificar los existentes:

1. Duplica uno de los bloques de modelo en la sección "Modelos":
```html
<div class="col-md-4 mb-4" data-aos="zoom-in" data-aos-delay="100">
    <div class="modelo-card">
        <div class="modelo-img">
            <img src="assets/img/1.jpg" alt="Modelo 1" class="img-fluid">
        </div>
        <div class="modelo-info">
            <h3>Modelo Estándar</h3>
            <p>Descripción del modelo...</p>
            <a href="#comprar" class="btn btn-outline-primary">Ver detalles</a>
        </div>
    </div>
</div>
```

2. Actualiza la imagen, título y descripción según sea necesario.

### Modificar información de contacto
Actualiza la información de contacto en dos lugares:

1. Sección de contacto (`id="contacto"`)
2. Pie de página (`<footer>`)

### Actualizar enlaces de redes sociales
Modifica los enlaces en la sección de contacto y en el pie de página:

```html
<div class="social-links mt-4">
    <a href="#" class="social-link"><i class="fab fa-facebook-f"></i></a>
    <a href="#" class="social-link"><i class="fab fa-instagram"></i></a>
    <!-- ... -->
</div>
```

### Cambiar videos
Para actualizar los videos demostrativos, reemplaza los enlaces de YouTube en la sección "Videos":

```html
<iframe src="https://www.youtube.com/embed/NUEVO_ID_VIDEO" title="Video demostrativo ClipTape" allowfullscreen></iframe>
```

### Modificar el botón de WhatsApp
Actualiza el número de WhatsApp en el enlace del botón flotante:

```html
<a href="https://wa.me/NUEVO_NUMERO" class="whatsapp-float" target="_blank">
    <i class="fab fa-whatsapp"></i>
</a>
```

## Optimización SEO
Para mejorar el posicionamiento en buscadores:

1. Actualiza las meta etiquetas en el `<head>`:
   - `<title>`: Título principal de la página
   - `<meta name="description">`: Descripción breve del sitio
   - `<meta name="keywords">`: Palabras clave relevantes

2. Asegúrate de que todas las imágenes tengan atributos `alt` descriptivos.

3. Mantén una estructura semántica con etiquetas HTML5 apropiadas.

## Mantenimiento

### Actualización de dependencias
Las bibliotecas externas se cargan desde CDN. Para actualizar a versiones más recientes, modifica los enlaces en el `<head>` y antes del cierre del `</body>`.

### Respaldo
Se recomienda hacer copias de seguridad regulares de todos los archivos antes de realizar modificaciones importantes.

---

Desarrollado por [Visual Enterprise](https://visualenterprise.com) - Especialistas en programación, diseño web, desarrollo de aplicaciones y ciencia de datos.