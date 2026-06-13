# 📚 Biblioteca Práctica

Biblioteca interactiva en español con **resúmenes accionables de 93 libros y 23 estudios científicos** (116 recursos) sobre hábitos, productividad, aprendizaje, creatividad, psicología de las decisiones, relaciones, propósito y salud cerebral. Construida como páginas HTML autocontenidas, sin dependencias externas.

## 🚀 Cómo usarla

Abre `index.html` en cualquier navegador moderno. No requiere servidor, instalación ni conexión a internet.

```bash
# Opción 1: abrir directamente el archivo
open index.html        # macOS
xdg-open index.html    # Linux

# Opción 2: servir localmente
python3 -m http.server 8000
# y visitar http://localhost:8000
```

## 🗂️ Estructura

| Archivo | Contenido |
|---------|-----------|
| `index.html` | **La biblioteca**: catálogo completo con resúmenes prácticos |
| `habitos-atomicos.html` | Guía interactiva completa de *Hábitos Atómicos* (James Clear) |
| `por-que-dormimos.html` | Guía interactiva completa de *Por qué dormimos* (Matthew Walker) |
| `meditaciones.html` | Guía interactiva completa de *Meditaciones* (Marco Aurelio y estoicismo práctico) |

## 📖 Contenido de la biblioteca

Cada recurso incluye: **idea central en una frase**, **ideas clave**, **plan de acción con checklist persistente**, **cita destacada**, **evidencia científica** (con matices y controversias señaladas honestamente), **recursos relacionados** y **notas personales**.

### Catálogo por categorías (116 recursos)

| Categoría | Recursos | Algunos títulos |
|-----------|----------|-----------------|
| 🔁 Hábitos | 12 | Hábitos Atómicos · El poder de los hábitos · Tiny Habits · La magia del orden · El efecto compuesto |
| 🎯 Productividad y foco | 16 | Trabajo Profundo · Esencialismo · GTD · Cuatro mil semanas · ¿Cuándo? · Descansa · La semana laboral de 4 horas |
| 🧠 Aprendizaje | 12 | Apréndetelo · Mindset · Range · Peak (Ericsson) · Los desafíos de la memoria · El arte de aprender |
| 🎨 Creatividad | 4 | El camino del artista · Roba como un artista · Libera tu magia · Caminar y creatividad (Oppezzo) |
| 🧭 Psicología y decisiones | 23 | Pensar rápido, pensar despacio · Influencia · Nudge · Antifrágil · Ruido · Decídete · Algoritmos para vivir · La psicología del dinero |
| 🤝 Relaciones y comunicación | 11 | Cómo ganar amigos · Conversaciones cruciales · Rompe la barrera del no · Apegados · Supercomunicadores · El arte de amar |
| 🧘 Propósito y bienestar | 25 | El hombre en busca de sentido · Meditaciones · Enquiridión · Séneca · La trampa de la felicidad · Agilidad emocional · Ikigai |
| 💪 Cuerpo y cerebro | 13 | Por qué dormimos · Spark · Outlive · ¿Por qué las cebras no tienen úlcera? · Generación dopamina · Respira |

### Estudios científicos destacados (23)

Desde los clásicos (intenciones de implementación de Gollwitzer, los 66 días de Lally, el efecto test de Roediger, la práctica deliberada de Ericsson) hasta hallazgos aplicables hoy mismo: la mera presencia del móvil reduce tu capacidad cognitiva (Ward 2017), el coste real de las interrupciones (Mark 2008), qué técnicas de estudio funcionan (Dunlosky 2013), gratitud experimental (Emmons 2003), relaciones y mortalidad (Holt-Lunstad 2010), dormir 6 horas sin notar el deterioro (Van Dongen 2003), ejercicio y depresión (Schuch 2018), hablarte por tu nombre (Kross 2014) o caminar para generar ideas (Oppezzo 2014). Cada ficha incluye referencia completa, diseño del estudio y cómo aplicarlo.

## 🧪 Funciones interactivas

- **Búsqueda** por título, autor o ideas, insensible a tildes y mayúsculas (atajo: tecla `/`)
- **Filtros** por categoría (8, con contador), tipo (libro/estudio) y estado de lectura
- **Ordenación** por título, autor o año, y botón 🎲 **recurso al azar**
- **Tema claro/oscuro** 🌗 con preferencia recordada
- **Estados de lectura** (por leer / leyendo / leído) y **favoritos** ⭐
- **Checklists de acción** por recurso con progreso persistente, y **notas personales** con autoguardado
- **Estadísticas** (leídos, leyendo, favoritos, acciones completadas) y barra de progreso
- **Copiar enlace directo** a cualquier recurso, y contador de resultados visibles
- **Exportar/importar** todos tus datos en JSON (estados, favoritos, checklists y notas)
- Todo persiste en `localStorage` (sin cuentas ni servidores)

## 🎓 Guías interactivas completas (3)

Además de los resúmenes, tres libros tienen **guía didáctica profunda** enlazada desde su ficha: módulos navegables con progreso persistente, ejercicios interactivos y quiz final de 10 preguntas con retroalimentación.

- ⚛️ **Hábitos Atómicos** — calculadora del 1%, constructor de identidad, apilador de hábitos, rastreador semanal, diagnóstico de malos hábitos
- 😴 **Por qué dormimos** — calculadoras de cafeína y ciclos de sueño, checklist de higiene (12 reglas), autoevaluación orientativa y plan de 7 días
- 🏛️ **Meditaciones** — clasificador de la dicotomía del control, reformulador estoico, reencuadre de obstáculos, diario estoico persistente

## 🛠️ Tecnología

HTML + CSS + JavaScript vanilla, un archivo por página. Diseño oscuro, responsivo (escritorio y móvil), sin frameworks ni CDN.

## ⚠️ Nota

Los resúmenes son síntesis orientativas con fines educativos: no sustituyen la lectura de las obras originales ni asesoramiento profesional. Donde la evidencia científica tiene matices o controversias (replicación, tamaños de efecto), se indica expresamente en cada ficha.
