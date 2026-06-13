# 📚 Biblioteca Práctica

Biblioteca interactiva en español con **resúmenes accionables de 151 libros y 49 estudios científicos** (200 recursos) sobre hábitos, productividad, aprendizaje, creatividad, psicología de las decisiones, relaciones, propósito y salud cerebral. Construida como páginas HTML autocontenidas, sin dependencias externas.

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
| `index.html` | **La biblioteca**: catálogo completo con resúmenes prácticos (autocontenido, sin dependencias externas) |
| `guias/<id>.html` | **Una guía práctica interactiva por recurso** (197 archivos individuales y autocontenidos) |
| `habitos-atomicos.html` | Guía interactiva ampliada de *Hábitos Atómicos* (James Clear) |
| `por-que-dormimos.html` | Guía interactiva ampliada de *Por qué dormimos* (Matthew Walker) |
| `meditaciones.html` | Guía interactiva ampliada de *Meditaciones* (Marco Aurelio y estoicismo práctico) |
| `assets/data.js` | Catálogo (`CATS` + `LIBRARY`) usado como fuente para regenerar las guías |
| `tools/gen-guias.js` | Script que genera los archivos de `guias/` a partir del catálogo (`node tools/gen-guias.js`) |

## 📖 Contenido de la biblioteca

Cada recurso incluye: **idea central en una frase**, **ideas clave**, **plan de acción con checklist persistente**, **cita destacada**, **evidencia científica** (con matices y controversias señaladas honestamente), **recursos relacionados** y **notas personales**.

### Catálogo por categorías (200 recursos)

| Categoría | Recursos | Algunos títulos |
|-----------|----------|-----------------|
| 🔁 Hábitos | 14 | Hábitos Atómicos · El poder de los hábitos · Tiny Habits · La magia del orden · El efecto compuesto · Mañanas milagrosas |
| 🎯 Productividad y foco | 26 | Trabajo Profundo · Esencialismo · GTD · Cuatro mil semanas · Lo único · Hyperfocus · Crea tu segunda mente · La mente organizada |
| 🧠 Aprendizaje | 24 | Apréndetelo · Mindset · Range · Peak (Ericsson) · ¿Cómo aprendemos? (Dehaene) · Fluent Forever · Cómo leer un libro |
| 🎨 Creatividad | 12 | El camino del artista · Roba como un artista · La guerra del arte · Originales · El hábito creativo · Las buenas ideas |
| 🧭 Psicología y decisiones | 38 | Pensar rápido, pensar despacio · Nudge · Antifrágil · Ruido · El cisne negro · Superpronosticadores · Subliminal · Algoritmos para vivir |
| 🤝 Relaciones y comunicación | 23 | Cómo ganar amigos · Conversaciones difíciles · Obtenga el sí · Comunicación no violenta · Abrázame fuerte · El cerebro del niño |
| 🧘 Propósito y bienestar | 41 | El hombre en busca de sentido · Meditaciones · El arte de la buena vida · La trampa de la felicidad · 12 reglas para vivir · Una mente liberada |
| 💪 Cuerpo y cerebro | 22 | Por qué dormimos · Spark · Outlive · En defensa de la comida · La digestión es la cuestión · Comer, moverse, dormir |

### Estudios científicos destacados (49)

Desde los clásicos (la curva del olvido de Ebbinghaus 1885, intenciones de implementación de Gollwitzer, la práctica deliberada de Ericsson, el test de la golosina de Mischel, elogiar la inteligencia de Mueller–Dweck, la disonancia cognitiva de Festinger) hasta hallazgos aplicables hoy mismo: la mera presencia del móvil reduce tu capacidad cognitiva (Ward 2017), qué técnicas de estudio funcionan (Dunlosky 2013), recuperar vence a los mapas conceptuales (Karpicke 2011), escribir la lista de tareas ayuda a dormir (Scullin 2018), hablar con desconocidos (Epley 2014), relaciones y mortalidad (Holt-Lunstad 2010), ¿puede el ejercicio compensar 8 h sentado? (Ekelund 2016), metas específicas y difíciles (Locke–Latham), tres cosas buenas (Seligman 2005) o ¿el dinero da la felicidad? (Killingsworth–Kahneman 2023). Cada ficha incluye referencia completa, diseño del estudio, cómo aplicarlo y, cuando procede, sus controversias y réplicas.

## 🧪 Funciones interactivas

- **Pantalla de bienvenida** que deja elegir entre **Modo Móvil** (una columna en tarjetas de lista, controles grandes, chips deslizables) y **Modo Escritorio** (rejilla amplia de varias columnas, ficha más ancha), con opción de autodetección; la elección se recuerda y se cambia con el botón 🖥️/📱 de la barra
- **Búsqueda** por título, autor o ideas, insensible a tildes y mayúsculas (atajo: tecla `/`)
- **Filtros** por categoría (8, con contador), tipo (libro/estudio) y estado de lectura
- **Orden por defecto «Destacados primero»**: las primeras filas muestran los recursos más conocidos de cada área (intercalados por categoría). También se puede ordenar por título, autor o año, y hay botón 🎲 **recurso al azar**
- **Tema claro/oscuro** 🌗 con preferencia recordada
- **Estados de lectura** (por leer / leyendo / leído) y **favoritos** ⭐
- **Checklists de acción** por recurso con progreso persistente, y **notas personales** con autoguardado
- **Estadísticas** (leídos, leyendo, favoritos, acciones completadas) y barra de progreso
- **Copiar enlace directo** a cualquier recurso, y contador de resultados visibles
- **Exportar/importar** todos tus datos en JSON (estados, favoritos, checklists y notas)
- **Diseño responsive**: en móvil, chips de categoría deslizables, controles a pantalla completa, objetivos táctiles amplios y campos a 16px (sin zoom forzado en iOS); en escritorio, hero con degradados, rejilla de hasta 4 columnas y tarjetas con franja de color por categoría
- Todo persiste en `localStorage` (sin cuentas ni servidores)

## 🎓 Guías prácticas

**Cada uno de los 200 recursos tiene su propia guía práctica interactiva**, como archivo individual y autocontenido en `guias/<id>.html` (197 archivos + las 3 guías ampliadas). Desde la ficha de la biblioteca, el botón **«📘 Abrir guía práctica»** abre la guía del recurso: una página navegable, temática por el color de su categoría, con módulos: Introducción, Ideas clave, Plan de acción (checklist persistente), Cita, La evidencia, Ficha del estudio (en los estudios científicos), Relacionados, Autoevaluación y Mis notas. El progreso, la checklist y las notas se guardan por recurso en `localStorage`. Para regenerarlas tras editar el catálogo: `node tools/gen-guias.js`.

### Tres guías ampliadas (artesanales)

Tres libros tienen además una **guía profunda hecha a mano** como página propia, con ejercicios interactivos a medida y quiz final de 10 preguntas:

- ⚛️ **Hábitos Atómicos** — calculadora del 1%, constructor de identidad, apilador de hábitos, rastreador semanal, diagnóstico de malos hábitos
- 😴 **Por qué dormimos** — calculadoras de cafeína y ciclos de sueño, checklist de higiene (12 reglas), autoevaluación orientativa y plan de 7 días
- 🏛️ **Meditaciones** — clasificador de la dicotomía del control, reformulador estoico, reencuadre de obstáculos, diario estoico persistente

## 🛠️ Tecnología

HTML + CSS + JavaScript vanilla, un archivo por página. Diseño oscuro, responsivo (escritorio y móvil), sin frameworks ni CDN.

**Identidad visual** (en `assets/`, todo SVG vectorial en la paleta de la app): `logo.svg` (logotipo con icono de libro + chispa de idea), `favicon.svg` (favicon de pestaña, presente en la biblioteca y en las guías) y `og-image.svg` (tarjeta para compartir, referenciada en las metaetiquetas Open Graph/Twitter de `index.html`). Nota: algunas redes no renderizan `og:image` en SVG; para esos casos conviene exportar una versión PNG (1200×630).

## ⚠️ Nota

Los resúmenes son síntesis orientativas con fines educativos: no sustituyen la lectura de las obras originales ni asesoramiento profesional. Donde la evidencia científica tiene matices o controversias (replicación, tamaños de efecto), se indica expresamente en cada ficha.
