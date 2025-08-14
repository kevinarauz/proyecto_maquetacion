# Guía de Uso - Generador de Portales Web

## Flujo de Trabajo Completo

### Proceso en 2 Etapas

#### **Etapa 1: Extracción con NotebookLLM**
1. Sube tu fuente de información (PDF, docs, web, etc.) a NotebookLLM
2. Usa el prompt: `notebook-llm-extraction-prompt.txt`
3. NotebookLLM te dará TODA la información extraída

#### **Etapa 2: Generación con Gemini**
1. Copia la información extraída de NotebookLLM
2. Usa el prompt: `json-structure-prompt.txt` (genera HTML directo)
3. O usa: `universal-portal-prompt.md` (sistema completo)
4. Gemini te genera un archivo `index.html` completo listo para usar

### Resultado Final

**UN SOLO ARCHIVO**: `index.html` con:
- ✅ CSS integrado en `<style>`
- ✅ JavaScript integrado en `<script>`
- ✅ Bootstrap 5 y Font Awesome desde CDN
- ✅ Diseño responsive mobile-first
- ✅ Listo para visualizar directamente

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