# Guía Mobile-First, Tipografías y Botones

## Mobile-First Approach

### Breakpoints Actualizados
```json
"breakpoints": {
  "xs": "0px",      // Extra small devices (portrait phones)
  "sm": "576px",    // Small devices (landscape phones)
  "md": "768px",    // Medium devices (tablets)
  "lg": "992px",    // Large devices (desktops)
  "xl": "1200px",   // Extra large devices (large desktops)
  "xxl": "1400px"   // Extra extra large devices
}
```

### Contenedores Responsivos
```json
"containers": {
  "xs": "100%",     // Móvil: ancho completo
  "sm": "540px",    // Móvil landscape
  "md": "720px",    // Tablet
  "lg": "960px",    // Desktop pequeño
  "xl": "1140px",   // Desktop estándar
  "xxl": "1320px"   // Desktop grande
}
```

### Layout Responsivo por Dispositivo
```json
"responsive": {
  "mobile": {
    "headerHeight": "60px",
    "padding": "1rem",
    "fontSize": "14px",
    "gridColumns": 1
  },
  "tablet": {
    "headerHeight": "70px", 
    "padding": "1.5rem",
    "fontSize": "16px",
    "gridColumns": 2
  },
  "desktop": {
    "headerHeight": "80px",
    "padding": "2rem", 
    "fontSize": "16px",
    "gridColumns": 3
  }
}
```

## Sistema de Tipografías Responsivas

### Tamaños por Dispositivo
```json
"fontSizes": {
  "mobile": {
    "h1": "2.25rem",    // 36px
    "h2": "1.875rem",   // 30px
    "h3": "1.5rem",     // 24px
    "h4": "1.25rem",    // 20px
    "h5": "1.125rem",   // 18px
    "h6": "1rem",       // 16px
    "body": "1rem",     // 16px
    "small": "0.875rem", // 14px
    "xs": "0.75rem"     // 12px
  },
  "tablet": {
    "h1": "2.75rem",    // 44px
    "h2": "2.25rem",    // 36px
    // ... incremento gradual
  },
  "desktop": {
    "h1": "3.5rem",     // 56px
    "h2": "2.5rem",     // 40px
    // ... tamaños completos
  }
}
```

### Pesos y Alturas de Línea
```json
"fontWeights": {
  "light": 300,       // Títulos delicados
  "regular": 400,     // Texto normal
  "medium": 500,      // Subtítulos
  "semibold": 600,    // Títulos importantes
  "bold": 700,        // Llamadas de atención
  "extrabold": 800    // Títulos principales
},
"lineHeights": {
  "tight": 1.2,       // Títulos grandes
  "normal": 1.5,      // Texto general
  "relaxed": 1.75,    // Párrafos largos
  "loose": 2.0        // Espaciado amplio
}
```

## Sistema Completo de Botones

### Tamaños de Botones
```json
"sizes": {
  "xs": {
    "padding": "0.25rem 0.5rem",  // 4px 8px
    "fontSize": "0.75rem",        // 12px
    "height": "2rem"              // 32px
  },
  "sm": {
    "padding": "0.375rem 0.75rem", // 6px 12px
    "fontSize": "0.875rem",        // 14px
    "height": "2.25rem"            // 36px
  },
  "md": {
    "padding": "0.5rem 1rem",      // 8px 16px
    "fontSize": "1rem",            // 16px
    "height": "2.5rem"             // 40px
  },
  "lg": {
    "padding": "0.75rem 1.5rem",   // 12px 24px
    "fontSize": "1.125rem",        // 18px
    "height": "3rem"               // 48px
  },
  "xl": {
    "padding": "1rem 2rem",        // 16px 32px
    "fontSize": "1.25rem",         // 20px
    "height": "3.5rem"             // 56px
  }
}
```

### Variantes de Botones

#### Primary (Principal)
```css
background: #2563eb
color: #ffffff
border: 1px solid #2563eb
hover: #1d4ed8 + translateY(-1px)
```

#### Secondary (Secundario)
```css
background: transparent
color: #2563eb
border: 1px solid #2563eb
hover: fondo azul + texto blanco
```

#### Outline (Contorno)
```css
background: transparent
color: #64748b
border: 1px solid #e2e8f0
hover: fondo gris claro
```

#### Ghost (Fantasma)
```css
background: transparent
color: #64748b
border: transparent
hover: fondo sutil
```

#### Success/Warning/Danger
```css
success: #10b981
warning: #f59e0b  
danger: #ef4444
```

## Implementación CSS Mobile-First

### Media Queries Recomendadas
```css
/* Base: Mobile (xs) */
.btn {
  padding: 0.5rem 1rem;
  font-size: 1rem;
}

/* Small devices (sm) */
@media (min-width: 576px) {
  .btn-lg {
    padding: 0.75rem 1.5rem;
    font-size: 1.125rem;
  }
}

/* Medium devices (md) */
@media (min-width: 768px) {
  h1 { font-size: 2.75rem; }
}

/* Large devices (lg) */
@media (min-width: 992px) {
  h1 { font-size: 3.5rem; }
}
```

### Grid Responsivo
```css
/* Mobile-first grid */
.grid {
  display: grid;
  grid-template-columns: 1fr; /* Mobile: 1 columna */
  gap: 1rem;
}

@media (min-width: 768px) {
  .grid {
    grid-template-columns: repeat(2, 1fr); /* Tablet: 2 columnas */
  }
}

@media (min-width: 992px) {
  .grid {
    grid-template-columns: repeat(3, 1fr); /* Desktop: 3 columnas */
  }
}
```

## Uso en el Prompt

El sistema actualizado incluye:

✅ **Mobile-First**: Diseño desde móvil hacia desktop  
✅ **Tipografías Responsivas**: Tamaños escalables por dispositivo  
✅ **Sistema de Botones**: 5 tamaños × 7 variantes = 35 combinaciones  
✅ **Breakpoints Modernos**: xs, sm, md, lg, xl, xxl  
✅ **CSS Grid + Flexbox**: Layout moderno y flexible  

Para usar, simplemente modifica el JSON y pasa al prompt de generación.