# 🍽️ Restaurant La Cocina de Niña Vicenta
### Landing Page — Gastronomía Salvadoreña Auténtica

<br>

> **Proyecto desarrollado como actividad práctica del**  
> 🎓 *Bootcamp: Transformación Digital para la Docencia Técnica*

---

## 📋 Descripción del proyecto

**La Cocina de Niña Vicenta** es una landing page de una sola página *(Single Page Application)* desarrollada con tecnologías web fundamentales: **HTML5, CSS3 y JavaScript puro**, sin frameworks ni dependencias externas.

El sitio representa a un restaurante de gastronomía salvadoreña auténtica ubicado en el **Cantón Las Marías, Jocoro, Morazán Sur, El Salvador**, y fue construido siguiendo los requerimientos de la actividad: *"Implementación de interactividad avanzada: manipulación del DOM, validación de formularios y publicación con control de versiones y apoyo de IA"*.

---

## 🌐 Ver el sitio en línea

> 🔗 **[https://tu-usuario.github.io/restaurante-la-cocina-de-nina-vicenta](https://tu-usuario.github.io/restaurante-la-cocina-de-nina-vicenta)**  
> *(Actualizar con la URL real de GitHub Pages una vez publicado)*

---

## 🗺️ Ubicación del negocio

📍 **Cantón Las Marías, Jocoro, Morazán Sur, Morazán, El Salvador**  
[Ver en Google Maps →](https://maps.app.goo.gl/U23pNWm9ve1cEQj46)

---

## 🎯 Temática elegida

De las tres opciones disponibles en la actividad, se seleccionó:

| # | Temática | Estado |
|---|----------|--------|
| 1 | Alojamientos Turísticos | — |
| ✅ **2** | **Gastronomía de El Salvador** | **Seleccionada** |
| 3 | Agencia de Viajes a Centroamérica | — |

**Negocio representado:** Restaurant La Cocina de Niña Vicenta  
Restaurante familiar con más de 15 años de tradición, especializado en platillos típicos salvadoreños.

---

## 📁 Estructura del proyecto

```
restaurante-la-cocina-de-nina-vicenta/
│
├── index.html          ← Archivo principal (toda la página)
└── README.md           ← Este archivo
```

> El proyecto es de **un solo archivo** `index.html` que contiene el HTML, CSS y JavaScript integrados, tal como lo requiere la actividad: *"landing page de una sola página"*.

---

## 🧩 Secciones obligatorias implementadas

| # | Sección | Descripción | ✅ |
|---|---------|-------------|---|
| 1 | **Hero** | Imagen de fondo completa, título, subtítulo y dos botones CTA | ✅ |
| 2 | **Navbar** | Fija con anclas a cada sección y menú hamburguesa responsive | ✅ |
| 3 | **Nosotros** | Historia del negocio, descripción y características del restaurante | ✅ |
| 4 | **Servicios** | 6 tarjetas con CSS Grid y efectos hover (Flexbox) | ✅ |
| 5 | **Formulario** | Reserva de mesa con validación completa en JavaScript | ✅ |
| 6 | **Footer** | Redes sociales, horarios, ubicación, mapa, año y créditos | ✅ |

**Secciones adicionales implementadas:**
- 🍲 **Menú Destacado** — 8 platillos típicos con precios
- 🗺️ **Mapa embebido** de Google Maps con la ubicación exacta

---

## ⚙️ Funcionalidades técnicas

### Manipulación del DOM
- Navbar que cambia de estilo al hacer scroll (`scrolled` class vía `window.addEventListener`)
- Menú hamburguesa que abre/cierra el panel de navegación móvil
- Año dinámico en el footer generado con `new Date().getFullYear()`
- Animaciones de aparición progresiva con `IntersectionObserver API`
- Mensaje de éxito que reemplaza el formulario al enviarlo correctamente

### Validación de formulario con JavaScript
El formulario de reserva valida en tiempo real los siguientes campos:

| Campo | Tipo de validación |
|-------|-------------------|
| Nombre completo | Mínimo 2 caracteres |
| Teléfono | Expresión regular `/^[\d\s\-\+]{7,15}$/` |
| Correo electrónico | Expresión regular `/^[^\s@]+@[^\s@]+\.[^\s@]+$/` |
| Fecha de reserva | No puede ser una fecha pasada |
| Hora | Campo obligatorio |
| Número de personas | Selección obligatoria |

- Resaltado visual de campos inválidos con clase `.error`
- Mensajes de error específicos por campo
- Limpieza automática del error al corregir el campo
- Fecha mínima dinámica (`min` del input = fecha de hoy)

### CSS avanzado
- Variables CSS (`--rojo`, `--dorado`, `--crema`, etc.) para paleta coherente
- CSS Grid para la cuadrícula de servicios (`repeat(auto-fit, minmax(280px, 1fr))`)
- Flexbox para navbar, footer y tarjetas
- Animaciones CSS con `@keyframes` (hero zoom, scroll pulse, fade up)
- Transiciones suaves en hover para tarjetas, botones y enlaces
- Diseño completamente responsive con media queries (`max-width: 900px`, `680px`)

---

## 🎨 Decisiones de diseño

| Elemento | Decisión | Justificación |
|----------|----------|---------------|
| **Paleta** | Rojo oscuro `#8B1A1A`, dorado `#C8860A`, crema `#FDF6EC` | Colores cálidos asociados a la gastronomía y tradición salvadoreña |
| **Tipografía** | Playfair Display (títulos) + Nunito (cuerpo) | Contraste entre elegancia y legibilidad |
| **Imágenes** | Unsplash.com (servicio gratuito, sin atribución requerida) | Fotos de alta calidad de comida y restaurantes |
| **Mapa** | Google Maps Embed API | Sin costo, sin API Key requerida para uso básico |
| **Íconos sociales** | SVG inline | Sin dependencias externas, carga instantánea |

---

## 📦 Control de versiones — Historial de commits

El proyecto fue desarrollado de forma incremental siguiendo buenas prácticas de Git:

| # | Commit | Contenido |
|---|--------|-----------|
| 1 | `init: estructura base y navbar` | HTML base, variables CSS, navbar fija con anclas y menú hamburguesa |
| 2 | `feat: hero section` | Imagen de fondo con zoom animado, título, subtítulo y CTAs |
| 3 | `feat: seccion nosotros` | Historia del negocio, imagen con badge y tarjetas de características |
| 4 | `feat: servicios y menu destacado` | CSS Grid de 6 servicios + sección de 8 platillos con precios |
| 5 | `feat: formulario de reserva con validacion JS` | Validación completa, estados de error y mensaje de éxito |
| 6 | `feat: footer y mapa embebido` | Columnas de footer, redes sociales SVG, mapa de Google Maps |
| 7 | `fix: responsive y animaciones` | Media queries, IntersectionObserver, scroll reveal y pulido final |

---

## 🚀 Instrucciones de uso

### Ver localmente
```bash
# 1. Clonar el repositorio
git clone https://github.com/tu-usuario/restaurante-la-cocina-de-nina-vicenta.git

# 2. Abrir el archivo directamente en el navegador
# No requiere servidor, no requiere instalación de dependencias
open index.html
```

### Publicar en GitHub Pages
```bash
# 1. Ir a Settings del repositorio en GitHub
# 2. Sección "Pages" → Source → "Deploy from a branch"
# 3. Branch: main → Carpeta: / (root)
# 4. Guardar — el sitio estará disponible en minutos
```

---

## 🛠️ Tecnologías utilizadas

| Tecnología | Versión | Uso |
|------------|---------|-----|
| HTML5 | — | Estructura semántica de la página |
| CSS3 | — | Estilos, Grid, Flexbox, animaciones |
| JavaScript | ES6+ | Validación, DOM, IntersectionObserver |
| Google Fonts | — | Playfair Display + Nunito |
| Unsplash | — | Imágenes gratuitas de alta calidad |
| Google Maps Embed | — | Mapa interactivo de ubicación |
| Git + GitHub | — | Control de versiones y publicación |

> ✅ **Sin frameworks. Sin librerías. Sin npm.** Solo tecnologías web estándar.

---

## 📱 Compatibilidad

| Dispositivo | Soporte |
|-------------|---------|
| Desktop (1200px+) | ✅ Completo |
| Tablet (768px – 900px) | ✅ Adaptado |
| Móvil (< 680px) | ✅ Menú hamburguesa + columnas apiladas |

Probado en: Chrome, Firefox, Edge y Safari (versiones modernas).

---

## ✏️ Personalización pendiente

Antes de publicar el sitio definitivamente, se deben actualizar los siguientes datos reales del negocio:

- [ ] Número de teléfono / WhatsApp (`+503 XXXX-XXXX`)
- [ ] URL de página de Facebook del restaurante
- [ ] URL de perfil de Instagram
- [ ] URL de perfil de TikTok
- [ ] Correo electrónico del negocio
- [ ] Precios actualizados del menú

---

## 👩‍💻 Información académica

| | |
|---|---|
| **Actividad** | Implementación de interactividad avanzada: manipulación del DOM, validación de formularios y publicación con control de versiones y apoyo de IA |
| **Modalidad** | Individual |
| **Programa** | Bootcamp: Transformación Digital para la Docencia Técnica |
| **Temática elegida** | Gastronomía de El Salvador |
| **Negocio** | Restaurant La Cocina de Niña Vicenta |
| **Tecnologías** | HTML5 · CSS3 · JavaScript ES6+ |
| **Repositorio** | GitHub |
| **Publicación** | GitHub Pages |

---

## 📜 Créditos

- **Imágenes:** [Unsplash.com](https://unsplash.com) — Licencia gratuita para uso personal y comercial
- **Tipografías:** [Google Fonts](https://fonts.google.com) — Playfair Display · Nunito
- **Mapa:** [Google Maps](https://maps.google.com) — Embed API gratuita
- **Iconos sociales:** SVG personalizados basados en estándares web

---

<div align="center">

Hecho por: Alan W. Moris y Ovidio O. Martínez en El Salvador · © 2026 Restaurant La Cocina de Niña Vicenta
