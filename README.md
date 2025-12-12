# Portafolio Personal - Corzo

Portafolio profesional de desarrollador Full Stack con diseño moderno y animaciones interactivas.

## 🚀 Características

- **Diseño Moderno**: Tema oscuro con gradientes púrpura/azul
- **Animaciones Suaves**: Efectos de scroll, hover y transiciones fluidas
- **Responsive**: Adaptado para móviles, tablets y escritorio
- **Secciones Incluidas**:
  - Hero con presentación personal
  - Habilidades técnicas con barras de progreso animadas
  - Timeline de experiencia profesional
  - Formulario de contacto
  - Footer con redes sociales

## 📋 Personalización

### 1. Información Personal

**En `index.html`:**

- **Línea 39-41**: Cambia tu email, LinkedIn y GitHub en los métodos de contacto
- **Línea 16**: Actualiza las estadísticas (años, empresas, tecnologías)
- **Línea 12**: Tu imagen está en `./assets/yop.png`

### 2. Redes Sociales

**En `index.html` (Footer - Líneas 132-152):**

```html
<!-- Actualiza estos links con tus perfiles reales -->
<a href="https://linkedin.com/in/TU-PERFIL">
<a href="https://github.com/TU-USUARIO">
<a href="mailto:TU-EMAIL@ejemplo.com">
```

### 3. Habilidades

**En `index.html` (Líneas 30-100):**

Para agregar o modificar habilidades, busca las secciones `.skill-item` y edita:
- `skill-name`: Nombre de la tecnología
- `data-progress`: Nivel de dominio (0-100)

Ejemplo:
```html
<div class="skill-item">
    <span class="skill-name">Nueva Tecnología</span>
    <div class="skill-bar">
        <div class="skill-progress" data-progress="85"></div>
    </div>
</div>
```

### 4. Experiencia Profesional

**En `index.html` (Líneas 105-185):**

Para cada trabajo, modifica:
- `timeline-year`: Fechas del trabajo
- `timeline-title`: Puesto
- `timeline-company`: Empresa
- `timeline-description`: Descripción de tus logros
- `timeline-tags`: Tecnologías usadas

### 5. Colores del Tema

**En `style.css`:**

Los gradientes principales están definidos como:
```css
/* Gradiente principal */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

Para cambiar el esquema de colores, busca `#667eea` y `#764ba2` en el CSS y reemplázalos con tus colores preferidos.

### 6. Formulario de Contacto

**En `script.js` (Línea 165):**

El formulario actualmente solo muestra un mensaje de éxito. Para implementar el envío real:

**Opción 1: EmailJS**
```javascript
// Regístrate en emailjs.com y agrega:
emailjs.send("service_id", "template_id", formData)
    .then(() => {
        // Mensaje de éxito
    });
```

**Opción 2: Tu propio backend**
```javascript
fetch('/api/send-email', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(formData)
});
```

## 🎨 Estructura de Archivos

```
portafolio/
│
├── index.html          # Estructura HTML
├── style.css           # Estilos y animaciones
├── script.js           # Funcionalidad JavaScript
└── assets/
    └── yop.png         # Tu foto de perfil
```

## 💡 Funcionalidades Interactivas

- **Animaciones de Scroll**: Las secciones aparecen al hacer scroll
- **Barras de Progreso**: Se animan cuando entran en el viewport
- **Contador Animado**: Las estadísticas se animan al cargar
- **Parallax**: Los elementos flotantes se mueven con el mouse
- **Ripple Effect**: Efecto de onda en los botones
- **Scroll to Top**: Botón flotante para volver arriba
- **Navegación por Teclado**: Usa teclas 1-4 para navegar entre secciones

## 🔧 Personalización Avanzada

### Agregar Nueva Sección

1. Agrega el HTML en `index.html`
2. Agrega los estilos en `style.css`
3. Si necesitas animaciones, agrégalas en `script.js`

### Cambiar Animaciones

Las animaciones principales están en `style.css`:
```css
@keyframes fadeInUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
}
```

## 📱 Responsive

El diseño se adapta a:
- **Móviles**: < 480px
- **Tablets**: 480px - 768px
- **Laptop**: 768px - 1024px
- **Desktop**: > 1024px

## 🌐 Deployment

### GitHub Pages
1. Crea un repositorio en GitHub
2. Sube los archivos
3. Ve a Settings > Pages
4. Selecciona la rama main
5. Tu sitio estará en: `https://tu-usuario.github.io/repo-name`

### Netlify
1. Arrastra la carpeta a netlify.com/drop
2. Tu sitio estará listo en segundos

### Vercel
1. Instala Vercel CLI: `npm i -g vercel`
2. Ejecuta: `vercel`
3. Sigue las instrucciones

## 📝 Notas

- Las imágenes deben estar en la carpeta `assets/`
- Optimiza tu foto de perfil (recomendado: 500x500px, formato WebP o PNG)
- Actualiza el `<title>` en el HTML con tu nombre
- Agrega un favicon.ico para el icono del navegador

## 🎯 Próximos Pasos

1. **Sección de Proyectos**: Agrega un portfolio de trabajos realizados
2. **Blog**: Integra una sección de artículos técnicos
3. **Modo Claro**: Implementa un toggle de tema claro/oscuro
4. **Multiidioma**: Agrega soporte para inglés/español
5. **Analytics**: Integra Google Analytics para rastrear visitas

## 📧 Contacto

Si tienes dudas sobre la personalización, no dudes en contactarme.

---

**Hecho con ❤️ en México** 🇲🇽
