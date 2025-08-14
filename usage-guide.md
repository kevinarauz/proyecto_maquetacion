# Guía de Uso - Generador de Portales Web

## Cómo Usar el Sistema

### 1. Configuración del JSON

Edita el archivo `portal-specifications.json` según tus necesidades:

#### Metadata
```json
"metadata": {
  "title": "Tu Portal Web",
  "description": "Descripción de tu portal",
  "language": "es",
  "keywords": ["palabra1", "palabra2"],
  "author": "Tu Nombre"
}
```

#### Colores y Tipografía
- **Colors**: Modifica la paleta de colores en hexadecimal
- **Typography**: Especifica fuentes de Google Fonts o web-safe
- **Spacing**: Ajusta los espacios según tu diseño

#### Secciones
- **Header**: Logo, navegación, botón CTA
- **Hero**: Título, subtítulo, botones de acción
- **Services**: Cards de servicios con iconos
- **About**: Información sobre la empresa
- **Testimonials**: Reviews de clientes
- **Contact**: Formulario e información de contacto
- **Footer**: Enlaces, contacto, redes sociales

### 2. Uso del Prompt

Copia el contenido de `portal-generator-prompt.md` y úsalo con cualquier IA junto con tu JSON personalizado:

```
[PROMPT COMPLETO] + 

"Genera un portal web usando estas especificaciones JSON: [TU_JSON_PERSONALIZADO]"
```

### 3. Personalización Rápida

#### Cambios Básicos
- **Título y descripción**: Modifica `metadata`
- **Colores**: Cambia `colors.primary`, `colors.secondary`, etc.
- **Navegación**: Edita `header.navigation.items`
- **Contenido**: Modifica textos en cada sección

#### Cambios Avanzados
- **Layout**: Ajusta `layout` para diferentes estructuras
- **Componentes**: Habilita/deshabilita secciones con `enabled: true/false`
- **Features**: Activa funciones como `darkMode`, `animations`, etc.

## Ejemplos de Personalización

### Portal Corporativo
```json
{
  "colors": {
    "primary": "#1e40af",
    "secondary": "#64748b",
    "accent": "#dc2626"
  },
  "hero": {
    "title": "Soluciones Empresariales",
    "subtitle": "Innovación y tecnología para tu negocio"
  }
}
```

### Portal Creativo
```json
{
  "colors": {
    "primary": "#8b5cf6",
    "secondary": "#f59e0b",
    "accent": "#ec4899"
  },
  "typography": {
    "primaryFont": "Poppins",
    "secondaryFont": "Roboto"
  }
}
```

### Portal de Servicios
```json
{
  "sections": [
    {
      "type": "services",
      "columns": 4,
      "items": [
        {
          "title": "Consultoría",
          "description": "Asesoramiento especializado",
          "icon": "consulting"
        }
      ]
    }
  ]
}
```

## Mejores Prácticas Incluidas

### UI/UX
- ✅ Diseño mobile-first
- ✅ Jerarquía visual clara
- ✅ Espaciado consistente
- ✅ Contraste accesible (WCAG AA)
- ✅ Navegación intuitiva

### Técnicas
- ✅ HTML5 semántico
- ✅ CSS Grid + Flexbox
- ✅ Bootstrap 5 integrado
- ✅ Optimización de performance
- ✅ SEO básico implementado

### Responsividad
- ✅ Breakpoints: 576px, 768px, 992px, 1200px
- ✅ Imágenes responsivas
- ✅ Tipografía escalable
- ✅ Componentes adaptables

## Estructura de Archivos Generada

```
portal/
├── index.html              # Página principal
├── css/
│   ├── main.css           # Estilos principales
│   └── responsive.css     # Media queries
├── js/
│   └── main.js           # JavaScript funcional
└── assets/
    └── images/           # Imágenes optimizadas
```

## Tips de Personalización

1. **Colores**: Usa herramientas como Coolors.co para paletas armoniosas
2. **Tipografía**: Máximo 2-3 fuentes para mantener consistencia
3. **Contenido**: Mantén textos concisos y orientados a la acción
4. **Imágenes**: Usa imágenes de alta calidad y optimizadas
5. **Testing**: Prueba en diferentes dispositivos y navegadores

## Soporte y Extensiones

El sistema está diseñado para ser extensible. Puedes:
- Agregar nuevas secciones al JSON
- Modificar el prompt para requerimientos específicos
- Integrar con CMS existentes
- Añadir funcionalidades con JavaScript adicional