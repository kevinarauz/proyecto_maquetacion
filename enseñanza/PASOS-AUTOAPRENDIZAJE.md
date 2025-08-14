# Guía de Pasos - Portal de Autoaprendizaje Técnico

## 🎯 Objetivo
Crear portales web personalizados para dominar cualquier tecnología, herramienta o lenguaje de programación.

## 📋 Flujo Completo (4 Pasos)

### **PASO 1: INVESTIGACIÓN Y DESCUBRIMIENTO** 🔍
**Objetivo**: Recopilar TODAS las fuentes sobre la tecnología objetivo

**Qué hacer**:
- Buscar documentación oficial
- Recopilar tutoriales de calidad
- Encontrar guías, ejemplos y casos de uso
- Descargar PDFs, artículos técnicos
- Guardar transcripciones de videos
- Revisar repositorios de GitHub relevantes

**Resultado**: Carpeta con todos los recursos encontrados

---

### **PASO 2: EXTRACCIÓN CON NOTEBOOKLLM** 📚
**Objetivo**: Extraer y organizar todo el conocimiento técnico

**Qué hacer**:
1. Subir todas las fuentes a NotebookLLM
2. Usar el prompt: `notebook-llm-course-discovery-prompt.txt`
3. Dejar que NotebookLLM procese y organice toda la información

**Resultado**: Documento completo con conocimiento estructurado

---

### **PASO 3: GENERACIÓN CON GEMINI** 🚀
**Objetivo**: Convertir la información en un portal web funcional

**Qué hacer**:
1. Copiar la información extraída por NotebookLLM
2. Usar el prompt: `json-structure-prompt.txt`
3. Pegar la información + prompt en Gemini
4. Gemini genera un archivo HTML completo

**Resultado**: Portal web personalizado (`index.html`)

---

### **PASO 4: CAPACITACIÓN PERSONAL** 🎓
**Objetivo**: Aprender a través del portal generado

**Qué hacer**:
- Abrir el portal en tu navegador
- Seguir el roadmap de aprendizaje
- Practicar con los comandos y ejemplos
- Realizar los proyectos propuestos
- Usar como referencia continua

**Resultado**: Dominio de la tecnología estudiada

---

## 🗂️ Archivos Necesarios

### En la carpeta `enseñanza/`:
- `notebook-llm-course-discovery-prompt.txt` - Para extraer conocimiento
- `json-structure-prompt.txt` - Para generar el portal HTML

### Herramientas:
- **NotebookLLM** - Para procesar fuentes y extraer información
- **Gemini** - Para generar el portal web final
- **Navegador** - Para usar el portal generado

---

## ✅ Consejos de Éxito

1. **Investigación exhaustiva**: Mientras más fuentes, mejor portal
2. **Calidad de fuentes**: Prioriza documentación oficial y recursos reconocidos
3. **Paciencia**: Deja que NotebookLLM procese toda la información
4. **Iteración**: Puedes regenerar el portal si encuentras más información

---

## 🎯 Ejemplos de Tecnologías Ideales

- **Lenguajes**: Python, JavaScript, Go, Rust
- **Frameworks**: React, Vue, Django, FastAPI
- **Herramientas**: Docker, Kubernetes, Git, AWS CLI
- **Bases de datos**: PostgreSQL, MongoDB, Redis
- **DevOps**: Terraform, Ansible, GitHub Actions

¡Crea tu propio manual personalizado para cualquier tecnología que quieras dominar!