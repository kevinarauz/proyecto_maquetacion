# CLAUDE.md

Este archivo proporciona orientación a Claude Code (claude.ai/code) cuando trabaja con código en este repositorio.

## Resumen del Proyecto

Este es un **Sistema Generador de Portales Web** - una herramienta impulsada por IA para crear portales web modernos y responsivos para diferentes industrias. El sistema utiliza especificaciones JSON comprensivas combinadas con prompts detallados para generar portales web completos con HTML5, CSS3 y JavaScript.

## Componentes Principales

### Archivos Base
- `universal-portal-prompt.md` / `universal-portal-prompt.txt` - Plantilla de prompt principal para generación con IA
- `portal-generator-prompt.md` - Versión alternativa del prompt
- `portal-specifications.json` - Plantilla base de configuración JSON
- `portal-capacitacion-example.json` - Ejemplo para portales educativos/capacitación

### Archivos de Documentación
- `usage-guide.md` - Instrucciones completas de uso del sistema
- `mobile-first-guide.md` - Especificaciones de diseño mobile-first y breakpoints responsivos
- `personalizacion-por-industria.md` - Guía de personalización específica por industria

## Arquitectura y Sistema de Diseño

### Configuración Dirigida por JSON
El sistema utiliza un esquema JSON comprensivo que define:
- **Metadatos**: Título, descripción, idioma, palabras clave, autor
- **Sistema de Diseño**: Tipografía, colores, espaciado, breakpoints, variantes de botones
- **Layout**: Contenedores responsivos y sistemas de grid mobile-first
- **Componentes**: Header, hero, secciones, footer con personalización completa
- **Características**: Accesibilidad, SEO, optimizaciones de rendimiento
- **Integraciones**: Bootstrap, Font Awesome, Google Fonts

### Diseño Responsivo Mobile-First
- **Breakpoints**: xs(0px), sm(576px), md(768px), lg(992px), xl(1200px), xxl(1400px)
- **Tipografía**: Tamaños de fuente escalables para móvil/tablet/escritorio
- **Sistema Grid**: 1 columna (móvil) → 2 columnas (tablet) → 3+ columnas (escritorio)
- **Tamaños de Componentes**: Tamaños de botones responsivos, espaciado y layouts

### Sistema de Componentes
- **Header**: Navegación sticky con logo, elementos de menú y botón CTA
- **Hero Section**: Título, subtítulo, descripción, opciones de fondo, múltiples CTAs
- **Secciones de Contenido**: Cards, testimonios, estadísticas, precios, formularios de contacto
- **Footer**: Layout multi-columna con enlaces, información de contacto y redes sociales

## Flujo de Trabajo Común

### 1. Proceso de Generación de Portal
```
[Prompt Universal] + [JSON Personalizado] → Portal Web Completo
```

1. Copiar el prompt universal (`universal-portal-prompt.md`)
2. Personalizar las especificaciones JSON para la industria objetivo
3. Combinar prompt + JSON para generar portal vía IA
4. La salida incluye archivos HTML, CSS y JavaScript

### 2. Personalización por Industria
- Usar `personalizacion-por-industria.md` para modificaciones específicas por sector
- Educación/Capacitación: `portal-capacitacion-example.json` como plantilla
- Se proporcionan plantillas para Corporativo, E-commerce, Salud, Restaurante, Servicios Profesionales, Inmobiliaria, Creativo/Portfolio

### 3. Personalización de Diseño
- Modificar colores, tipografía y espaciado en JSON
- Usar `mobile-first-guide.md` para especificaciones responsivas
- Sistema de botones soporta 5 tamaños × 7 variantes (35 combinaciones)

## Principios de Diseño Clave

### Estándares Técnicos
- **Estructura HTML5 Semántica**: Uso apropiado de header, nav, main, section, article, footer
- **Layout CSS Moderno**: CSS Grid para layouts principales, Flexbox para componentes
- **Bootstrap 5+**: Integrado para grid responsivo y componentes
- **JavaScript ES6+**: Interactividad moderna y validación de formularios
- **Accesibilidad**: Cumplimiento WCAG 2.1 AA con atributos aria apropiados
- **Optimización SEO**: Meta tags completos, schema markup, optimización de rendimiento

### Adaptación por Industria
El sistema soporta generación de portales para:
- **Educación/Capacitación**: Cursos, certificaciones, testimonios de estudiantes, niveles de precios
- **Corporativo**: Servicios, casos de estudio, secciones de equipo, logos de clientes
- **E-commerce**: Grids de productos, características de compra, reseñas, promociones
- **Salud**: Servicios, especialidades del personal, testimonios de pacientes, contacto de emergencia
- **Restaurantes**: Categorías de menú, galería, ubicación/horarios, pedidos en línea
- **Servicios Profesionales**: Portfolio, explicación de proceso, credenciales, reserva de consultas
- **Inmobiliaria**: Listados de propiedades, perfiles de agentes, información de barrios, tours virtuales
- **Creativo/Portfolio**: Galerías masonry, servicios creativos, flujo de trabajo, contacto personalizado

## Estructura de Archivos (Salida Generada)
```
portal/
├── index.html              # Página principal con estructura semántica
├── assets/
│   ├── css/
│   │   ├── main.css        # Estilos principales con variables CSS
│   │   ├── components.css  # Estilos de componentes reutilizables
│   │   └── responsive.css  # Media queries y diseño responsivo
│   ├── js/
│   │   ├── main.js         # Funcionalidad JavaScript principal
│   │   └── components.js   # Componentes interactivos
│   └── images/             # Imágenes y assets optimizados
```

## Mejores Prácticas

### Al Modificar Configuraciones JSON
1. Mantener la estructura existente y campos requeridos
2. Usar las paletas de colores proporcionadas apropiadas para la industria
3. Mantener tipografía limitada a 2-3 fuentes para consistencia
4. Asegurar que todas las secciones requeridas tengan contenido apropiado
5. Probar comportamiento responsivo en todos los breakpoints

### Al Personalizar por Industrias
1. Referenciar `personalizacion-por-industria.md` para orientación específica por sector
2. Usar terminología y CTAs apropiados para la audiencia objetivo
3. Incluir proof points y testimonios relevantes
4. Optimizar formularios y métodos de contacto para la industria
5. Considerar optimización de conversión específica para el sector

### Rendimiento y Accesibilidad
- Todos los portales generados incluyen lazy loading, minificación y CSS crítico
- Cumplimiento WCAG 2.1 AA está integrado en las especificaciones de componentes
- El enfoque mobile-first asegura rendimiento óptimo en todos los dispositivos
- Optimización SEO incluye meta tags completos y markup semántico