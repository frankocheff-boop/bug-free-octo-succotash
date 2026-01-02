# Verano Estate - Sistema de Gestión Web

![Verano Estate](https://i.imgur.com/1CQ3BSd.png)

## 📋 Descripción del Sistema

Sistema web completo para **Verano Estate by Chef Franko**, una propiedad de alquiler vacacional premium en Puerto Vallarta. Este sistema incluye formularios de información de huéspedes, menús interactivos, y paneles de control para eventos especiales.

## 🎯 Componentes del Sistema

### 1. Formulario Principal de Huéspedes (`index.html`)
Formulario completo y avanzado para recopilar información detallada de los huéspedes.

**Características:**
- ✅ Soporte para 3 idiomas (Español, Inglés, Francés)
- ✅ Información básica del grupo
- ✅ Opciones de transporte desde el aeropuerto
- ✅ Gestión de habitaciones (hasta 11 habitaciones)
- ✅ Asignación individual de habitaciones con fechas
- ✅ Servicios adicionales y ocasiones especiales
- ✅ Actividades (Mariachi, Yoga, Tours, Spa, Yate, etc.)
- ✅ Provisiones y bebidas personalizadas
- ✅ Integración con Formspree y WhatsApp

### 2. Formulario Simplificado (`guest-form.html`)
Versión simplificada para registro rápido.

**Características:**
- ✅ Soporte bilingüe (Español/Inglés)
- ✅ Campos básicos esenciales
- ✅ Envío directo por WhatsApp
- ✅ Diseño limpio y minimalista

### 3. Panel de Control de Eventos (`untitled-1.html`)
Dashboard especializado para gestión de bodas y eventos especiales.

**Características:**
- ✅ Vista de resumen con métricas clave
- ✅ Línea de tiempo del evento
- ✅ Itinerario detallado con acordeones interactivos
- ✅ Plan de atención personalizada para alergias
- ✅ Gráficos con Chart.js
- ✅ Sistema de tabs para organización

### 4. Menú Interactivo (`HTML-MENU.html`)
Sistema de selección de menú para huéspedes.

**Características:**
- ✅ Menú de desayuno con opciones diarias
- ✅ Selección de almuerzo con clásicos
- ✅ Menú de cena gourmet expandible
- ✅ Validación de selecciones
- ✅ Campo para alergias e instrucciones
- ✅ Vista previa para impresión
- ✅ Botón flotante de WhatsApp

### 5. Menú Estático (`menu-restaurante.html`)
Menú visual estático para presentación.

**Características:**
- ✅ Diseño elegante con gradiente
- ✅ Secciones organizadas (Entradas, Principales, Postres, Bebidas)
- ✅ Animaciones al cargar
- ✅ Efectos hover interactivos

## 🎨 Diseño y Marca

### Paleta de Colores
```css
--brand-teal: #003C3C;     /* Color principal */
--brand-bg: #FBF7F0;       /* Fondo cálido */
--accent: #4c7c7c;         /* Acento teal claro */
```

### Tipografía
- **Headings:** Playfair Display (serif)
- **Body:** Montserrat / Inter (sans-serif)

### Framework
- **CSS:** Tailwind CSS (CDN)
- **Charts:** Chart.js (CDN)
- **Icons:** Inline SVG

## 🚀 Inicio Rápido

### 1. Clonar el Repositorio
```bash
git clone https://github.com/frankocheff-boop/bug-free-octo-succotash.git
cd bug-free-octo-succotash
```

### 2. Servir los Archivos
```bash
# Opción 1: Python
python -m http.server 8000

# Opción 2: Node.js
npx http-server -p 8000

# Opción 3: Abrir directamente
open index.html
```

### 3. Acceder
```
http://localhost:8000/index.html
```

## 📱 Integraciones

### WhatsApp
- **Número:** +52 322 160 6843
- **Formato:** Mensaje personalizado por formulario
- **Función:** `sendToWhatsApp()` en cada archivo

### Formspree
- **Endpoint:** `https://formspree.io/f/xvgqddpg`
- **Método:** POST con `Accept: application/json`

## 🌐 Idiomas

| Componente | ES | EN | FR |
|------------|----|----|-----|
| index.html | ✅ | ✅ | ✅ |
| guest-form.html | ✅ | ✅ | ❌ |
| untitled-1.html | ✅ | ❌ | ❌ |
| HTML-MENU.html | ✅ | ✅ | ❌ |

## 🔧 Personalización

### Cambiar Número de WhatsApp
Buscar y reemplazar en todos los archivos:
```javascript
const phone = "523221606843"; // Tu nuevo número
```

### Modificar Habitaciones
En `index.html`, editar:
```javascript
const roomData = [
    { number: 1, type: "King Bed" },
    { number: 2, type: "2 Queen Beds" },
    // Agregar más...
];
```

### Agregar Idioma Nuevo
1. Agregar botón en el selector de idioma
2. Extender objeto `translations` con nuevo idioma
3. Agregar lógica en función `setLanguage()`

## 📞 Contacto

**Verano Estate by Chef Franko**
- 📱 WhatsApp: +52 322 160 6843
- 📧 Email: franko@veranostate.com
- 📸 Instagram: @veranostate
- 📍 Puerto Vallarta, México

## 🤝 Contribuir

1. Fork el proyecto
2. Crear feature branch (`git checkout -b feature/mejora`)
3. Commit cambios (`git commit -m 'Agregar mejora'`)
4. Push al branch (`git push origin feature/mejora`)
5. Abrir Pull Request

## 📄 Licencia

© 2025 Verano Estate by Chef Franko. Todos los derechos reservados.

## 📝 Notas Técnicas

### Estructura de Archivos
```
.
├── index.html              # Formulario principal (3 idiomas)
├── guest-form.html         # Formulario simplificado
├── untitled-1.html         # Dashboard de eventos
├── HTML-MENU.html          # Menú interactivo
├── menu-restaurante.html   # Menú estático
├── README.md              # Este archivo
├── _conffig.yml           # Configuración
└── .github/
    └── copilot-instructions.md
```

### Mejores Prácticas
- ✅ Código limpio y comentado
- ✅ Responsive design (mobile-first)
- ✅ Validación de formularios
- ✅ Manejo de errores
- ✅ Accesibilidad (ARIA labels)
- ✅ SEO básico (meta tags)

---

**Versión:** 1.0.0  
**Última actualización:** Enero 2025  
**Mantenido por:** Chef Franko Team
