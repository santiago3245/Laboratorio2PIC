# Laboratorio2PIC

# Link GitHub:

---

### Carpeta: Htmls/

Contiene las vistas principales en formato HTML que estructuran las diferentes páginas del sitio web:

- **AcercaDe.html**: Página que proporciona información sobre el proyecto o la organización.
- **galeria.html**: Muestra una galería de imágenes o contenido multimedia.
- **index.html**: La página principal del proyecto, actuando como punto de entrada al sitio.
- **Perfil.html**: Página para mostrar información personalizada o perfiles de usuario.

---

### Carpeta: Scripts/

Incluye los archivos JavaScript para funcionalidades dinámicas del proyecto:

- **footer.js**: Controla la generación y comportamiento del pie de página.
- **Galery.js**: Maneja las interacciones y funcionalidades específicas de la galería.
- **header.js**: Gestiona el encabezado de las páginas, incluyendo menús y navegación.
- **home.js**: Proporciona funcionalidades específicas para la página principal.
- **menu-shadow.js**: Aplica efectos de sombra o animación al menú de navegación.
- **perfil.js**: Controla las funciones relacionadas con la página de perfil.
- **slots.js**: Implementa características relacionadas con un sistema de "slots" (probablemente para juegos o horarios).
- **Table.js**: Genera o administra tablas dinámicas dentro de las páginas.

---
### Descripció: Scripts
### **1. Footer**
Archivo: `footer.js`

Define un pie de página dinámico con diseño moderno. Utiliza Shadow DOM para encapsular su estilo y estructura, evitando colisiones con otros elementos de la página.

- **Clase**: `FooterShadow`
- **Uso**: `<mi-footer></mi-footer>`

**Características**:
- Pie de página responsivo con fondo oscuro y texto claro.
- Sombra para mejorar el diseño visual.
- Texto de derechos reservados con el año actual.

---

### **2. Galería**
Archivo: `Galery.js`

Este componente genera una galería dinámica de tarjetas basadas en datos obtenidos de una API. Renderiza información sobre personajes, planetas y transformaciones en un diseño de cuadrícula.

- **Clase**: `UserGalery`
- **Uso**: `<user-gallery api-endpoint="https://example.com/api/character"></user-gallery>`

**Características**:
- Integra una cuadrícula para mostrar contenido en tarjetas.
- Obtiene datos dinámicamente desde un endpoint API.
- Manejo de errores para garantizar una experiencia robusta.

---

### **3. Header**
Archivo: `header.js`

Un encabezado dinámico que muestra el título y subtítulo del sitio. Este componente encapsula sus estilos utilizando Shadow DOM.

- **Clase**: `HeaderShadow`
- **Uso**: `<mi-header></mi-header>`

**Características**:
- Título y descripción personalizables.
- Diseño responsivo que adapta tamaños de fuente para dispositivos móviles.
- Estilo moderno con fondo verde y texto blanco.

---

### **4. Home**
Archivo: `HomePage.js`

Un componente que muestra una pantalla de bienvenida minimalista para la página principal. Diseñado para ser el primer elemento visual que los usuarios encuentran al visitar el sitio.

- **Clase**: `HomePage`
- **Uso**: `<mi-home></mi-home>`

**Características**:
- Fondo claro con un mensaje centralizado.
- Texto con sombras para un efecto visual atractivo.
- Diseño limpio y responsivo.

---

### **5. Menú**
Archivo: `MenuShadow.js`

Un componente de menú horizontal que incluye enlaces de navegación. El diseño es simple y adaptable, con estilos modernos.

- **Clase**: `MenuShadow`
- **Uso**: `<menu-shadow></menu-shadow>`

**Características**:
- Navegación intuitiva con enlaces personalizables.
- Estilos de hover con resaltado en color cian.
- Estructura encapsulada que evita conflictos de estilo.

---

### **6. Perfil**
Archivo: `Perfil.js`

Un componente que representa un perfil de usuario con imagen, nombre, biografía y botones interactivos.

- **Clase**: `Perfil`
- **Uso**: `<mi-perfil profile-pic="url" username="Nombre" bio="Descripción"></mi-perfil>`

**Características**:
- Imagen de perfil circular con borde y sombra.
- Diseño responsivo y moderno.
- Botones interactivos con animaciones de hover.

---

### **7. Slot Component**
Archivo: `ComponentSlot.js`

Un componente que utiliza **slots** para permitir la personalización de su contenido. Ideal para tarjetas de presentación o información.

- **Clase**: `ComponentSlot`
- **Uso**: 
  ```html
  <component-slot>
      <div slot="image"><img src="image.jpg" alt="Example"></div>
      <div slot="titulo">Título Personalizado</div>
      <div slot="descripción">Descripción personalizada aquí.</div>
      <div slot="opciones">Opciones adicionales</div>
  </component-slot>

### **8. Tabla Personalizada**
Archivo: `CustomTable.js`

Este componente genera una tabla dinámica basada en datos obtenidos de una API. Permite mostrar información estructurada en columnas, como el ID, nombre, correo electrónico y ciudad de un usuario.

- **Clase**: `CustomTable`
- **Uso**: 
  ```html
  <custom-table api-endpoint="https://jsonplaceholder.typicode.com/users"></custom-table>
