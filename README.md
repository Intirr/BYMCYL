# 📚 Biblioteca Práctica

Biblioteca interactiva en español con **resúmenes accionables de 121 libros y 35 estudios científicos** (156 recursos) sobre hábitos, productividad, aprendizaje, creatividad, psicología de las decisiones, relaciones, propósito y salud cerebral. Construida como páginas HTML autocontenidas, sin dependencias externas.

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

### Catálogo por categorías (156 recursos)

| Categoría | Recursos | Algunos títulos |
|-----------|----------|-----------------|
| 🔁 Hábitos | 12 | Hábitos Atómicos · El poder de los hábitos · Tiny Habits · La magia del orden · El efecto compuesto |
| 🎯 Productividad y foco | 20 | Trabajo Profundo · Esencialismo · GTD · Cuatro mil semanas · Lo único · Haz tiempo · Hyperfocus · La semana laboral de 4 horas |
| 🧠 Aprendizaje | 18 | Apréndetelo · Mindset · Range · Peak (Ericsson) · ¿Cómo aprendemos? (Dehaene) · Maestría · Los desafíos de la memoria |
| 🎨 Creatividad | 9 | El camino del artista · Roba como un artista · La guerra del arte · Originales · Creatividad S.A. · Pájaro a pájaro · Enseña tu trabajo |
| 🧭 Psicología y decisiones | 31 | Pensar rápido, pensar despacio · Nudge · Antifrágil · Ruido · El cisne negro · Factfulness · Pensar en apuestas · Algoritmos para vivir |
| 🤝 Relaciones y comunicación | 16 | Cómo ganar amigos · Conversaciones cruciales · Comunicación no violenta · Gottman · Apegados · Supercomunicadores · Límites |
| 🧘 Propósito y bienestar | 33 | El hombre en busca de sentido · Meditaciones · Enquiridión · La trampa de la felicidad · Diseña tu vida · 10% más feliz · Ikigai |
| 💪 Cuerpo y cerebro | 17 | Por qué dormimos · Spark · Outlive · El cuerpo lleva la cuenta · Lifespan · La revolución de la glucosa · Respira |

### Estudios científicos destacados (35)

Desde los clásicos (intenciones de implementación de Gollwitzer, los 66 días de Lally, el efecto test de Roediger, la práctica deliberada de Ericsson, el test de la golosina de Mischel, la disonancia cognitiva de Festinger) hasta hallazgos aplicables hoy mismo: la mera presencia del móvil reduce tu capacidad cognitiva (Ward 2017), qué técnicas de estudio funcionan (Dunlosky 2013), las 36 preguntas para enamorarse (Aron 1997), relaciones y mortalidad (Holt-Lunstad 2010), dormir 6 horas sin notar el deterioro (Van Dongen 2003), una multa es un precio (Gneezy 2000), ¿el dinero da la felicidad? (Killingsworth–Kahneman 2023) o caminar para generar ideas (Oppezzo 2014). Cada ficha incluye referencia completa, diseño del estudio, cómo aplicarlo y, cuando procede, sus controversias y réplicas.

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

Además de los resúmenes, tres libros tienen **guía didáctica profunda** como página propia (`habitos-atomicos.html`, `por-que-dormimos.html`, `meditaciones.html`): módulos navegables con progreso persistente, ejercicios interactivos y quiz final de 10 preguntas con retroalimentación. Cada guía incluye un enlace «← Volver a la Biblioteca Práctica».

- ⚛️ **Hábitos Atómicos** — calculadora del 1%, constructor de identidad, apilador de hábitos, rastreador semanal, diagnóstico de malos hábitos
- 😴 **Por qué dormimos** — calculadoras de cafeína y ciclos de sueño, checklist de higiene (12 reglas), autoevaluación orientativa y plan de 7 días
- 🏛️ **Meditaciones** — clasificador de la dicotomía del control, reformulador estoico, reencuadre de obstáculos, diario estoico persistente

## 🛠️ Tecnología

HTML + CSS + JavaScript vanilla, un archivo por página. Diseño oscuro, responsivo (escritorio y móvil), sin frameworks ni CDN.

## ⚠️ Nota

Los resúmenes son síntesis orientativas con fines educativos: no sustituyen la lectura de las obras originales ni asesoramiento profesional. Donde la evidencia científica tiene matices o controversias (replicación, tamaños de efecto), se indica expresamente en cada ficha.
