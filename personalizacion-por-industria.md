# Personalización de Portales por Industria

## Cómo Usar el Sistema Universal

### Paso 1: Copiar el Prompt Base
Usa `universal-portal-prompt.txt` como instrucciones base para cualquier IA

### Paso 2: Personalizar el JSON
Modifica `portal-specifications.json` según tu industria usando las guías siguientes

### Paso 3: Generar Portal
```
[PROMPT_UNIVERSAL] + [JSON_PERSONALIZADO] = Portal Completo
```

## Templates por Industria

### 🎓 EDUCACIÓN/CAPACITACIÓN
**Archivo**: `portal-capacitacion-example.json`

**Elementos Clave**:
- Cursos y certificaciones destacadas
- Testimonios de estudiantes exitosos
- Estadísticas de graduados
- Planes de precios escalonados
- Área de recursos educativos

**Colores Recomendados**:
```json
"primary": "#6366f1",    // Violeta profesional
"secondary": "#8b5cf6",  // Púrpura educativo
"accent": "#06b6d4"      // Azul confianza
```

**Secciones Específicas**:
- Hero con benefits educativos
- Grid de cursos con ratings
- Stats de éxito (graduados, satisfacción)
- Pricing con badges "Popular"
- Testimonials con aumentos salariales

### 💻 PORTAL DE AUTOAPRENDIZAJE TÉCNICO
**Nuevo Tipo**: Portal personal para dominar tecnologías

**Elementos Clave**:
- Sección "¿Qué es?" con definición clara
- Roadmap de aprendizaje visual
- Comandos esenciales con ejemplos
- Proyectos prácticos por nivel
- Recursos y herramientas recomendadas
- Cheat sheet descargable

**Colores Recomendados**:
```json
"primary": "#2563eb",    // Azul tech
"secondary": "#7c3aed",  // Púrpura coding
"accent": "#10b981"      // Verde progreso
```

**Estructura Especial**:
```json
"sections": [
  {"id": "fundamentos", "title": "¿Qué es y por qué usarlo?"},
  {"id": "instalacion", "title": "Instalación y Configuración"},
  {"id": "comandos", "title": "Comandos Esenciales"},
  {"id": "proyectos", "title": "Proyectos Prácticos"},
  {"id": "recursos", "title": "Recursos y Herramientas"},
  {"id": "roadmap", "title": "Hoja de Ruta de Aprendizaje"}
]
```

### 🏢 CORPORATIVO/EMPRESA
**Personalizar JSON Base**:

**Elementos Clave**:
```json
"hero": {
  "title": "Soluciones Empresariales de Clase Mundial",
  "subtitle": "Transformamos negocios con tecnología innovadora"
}
```

**Colores Recomendados**:
```json
"primary": "#1e40af",    // Azul corporativo
"secondary": "#64748b",  // Gris profesional
"accent": "#dc2626"      // Rojo acción
```

**Secciones Específicas**:
- Services con iconos profesionales
- Case studies con resultados
- Team con liderazgo
- Partners/clients logos
- Contact con múltiples oficinas

### 🛒 E-COMMERCE
**Elementos Clave**:
```json
"sections": [
  {
    "type": "products",
    "layout": "grid",
    "columns": 4,
    "items": [
      {
        "name": "Producto",
        "price": "$99.99",
        "originalPrice": "$129.99",
        "discount": "23%",
        "rating": "4.8",
        "reviews": "234",
        "badge": "Bestseller"
      }
    ]
  }
]
```

**Colores Recomendados**:
```json
"primary": "#059669",    // Verde compra
"secondary": "#7c3aed",  // Púrpura premium
"accent": "#f59e0b"      // Naranja ofertas
```

### 🏥 SALUD/MEDICINA
**Elementos Clave**:
```json
"colors": {
  "primary": "#0ea5e9",    // Azul médico
  "secondary": "#22c55e",  // Verde salud
  "accent": "#f43f5e"      // Rojo urgencia
}
```

**Secciones Específicas**:
- Services médicos
- Staff con especialidades
- Testimonials de pacientes
- Emergency contact destacado
- Insurance/payment info

### 🍕 RESTAURANTE/FOOD
**Elementos Clave**:
```json
"colors": {
  "primary": "#dc2626",    // Rojo apetitoso
  "secondary": "#f59e0b",  // Amarillo cálido
  "accent": "#059669"      // Verde fresco
}
```

**Secciones Específicas**:
- Menu con categorías
- Gallery de platos
- Location/hours prominente
- Online ordering CTA
- Chef/story section

### 💼 SERVICIOS PROFESIONALES
**Elementos Clave**:
```json
"hero": {
  "title": "Servicios Profesionales de Confianza",
  "ctaButtons": [
    {
      "text": "Solicitar Consulta",
      "style": "primary"
    }
  ]
}
```

**Secciones Específicas**:
- Services con process
- Portfolio/case studies
- Credentials/certifications
- Consultation booking form
- FAQ section

### 🏠 INMOBILIARIA
**Elementos Clave**:
```json
"sections": [
  {
    "type": "properties",
    "items": [
      {
        "title": "Casa Moderna",
        "price": "$450,000",
        "location": "Zona Norte",
        "bedrooms": "3",
        "bathrooms": "2",
        "area": "180m²"
      }
    ]
  }
]
```

**Colores Recomendados**:
```json
"primary": "#1e40af",    // Azul confianza
"secondary": "#059669",  // Verde inversión
"accent": "#dc2626"      // Rojo urgencia
```

### 🎨 CREATIVOS/PORTFOLIO
**Elementos Clave**:
```json
"colors": {
  "primary": "#8b5cf6",    // Púrpura creativo
  "secondary": "#06b6d4",  // Azul inspiración
  "accent": "#f59e0b"      // Amarillo energía
}
```

**Secciones Específicas**:
- Portfolio gallery masonry
- Services creativos
- Process/workflow
- Client testimonials
- Contact con personality

## Modificaciones Rápidas por Sector

### Cambiar Industria
1. **Metadata**: Título, descripción, keywords
2. **Colors**: Paleta según sector
3. **Hero**: Propuesta de valor específica
4. **Sections**: Contenido relevante
5. **CTA**: Acciones principales del sector

### Templates de Títulos por Industria
```json
// Educación
"title": "Transforma tu Futuro con [Nombre]"

// Corporativo
"title": "Soluciones Empresariales que Impulsan Resultados"

// E-commerce
"title": "Descubre, Compra, Disfruta - Todo en un Lugar"

// Salud
"title": "Tu Salud es Nuestra Prioridad"

// Restaurante
"title": "Sabores Auténticos que Conquistan"

// Servicios
"title": "Expertos que Hacen la Diferencia"
```

### CTAs por Industria
```json
// Educación
"ctaButtons": [
  { "text": "Comenzar Curso", "style": "primary" },
  { "text": "Ver Demo", "style": "secondary" }
]

// Corporativo
"ctaButtons": [
  { "text": "Solicitar Propuesta", "style": "primary" },
  { "text": "Agendar Reunión", "style": "secondary" }
]

// E-commerce
"ctaButtons": [
  { "text": "Comprar Ahora", "style": "primary" },
  { "text": "Ver Ofertas", "style": "secondary" }
]
```

## Proceso de Personalización

### 1. Identificar Sector
- Analiza tu audiencia objetivo
- Define propuesta de valor única
- Identifica competencia directa

### 2. Adaptar JSON
- Copia template base más cercano
- Modifica metadata y colores
- Personaliza secciones principales
- Ajusta CTAs y formularios

### 3. Contenido Específico
- Usa terminología del sector
- Incluye beneficios relevantes
- Agrega proof points específicos
- Personaliza testimonials

### 4. Optimizar por Conversión
- CTAs claros y específicos
- Formularios mínimos necesarios
- Proof social relevante
- Urgencia/escasez si aplica

## Ejemplos de Uso

### Comando para IA:
```
[COPIA PROMPT UNIVERSAL COMPLETO]

Genera un portal web para [INDUSTRIA] usando estas especificaciones JSON personalizadas:

[PEGA TU JSON MODIFICADO]
```

### Resultado:
Portal completo con:
- ✅ Diseño adaptado al sector
- ✅ Contenido relevante
- ✅ Colores apropiados
- ✅ CTAs específicos
- ✅ Secciones optimizadas