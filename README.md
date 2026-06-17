# 🗼 Pharus · Biblioteca

Biblioteca interactiva en español con **resúmenes accionables de 151 libros y 49 estudios científicos** (200 recursos) sobre hábitos, productividad, aprendizaje, creatividad, psicología de las decisiones, relaciones, propósito y salud cerebral. Construida como páginas HTML autocontenidas, sin dependencias externas.

**Pharus** (faro, en latín) es la identidad visual de la biblioteca: un diseño basado en un **faro y conexiones neuronales**. El faro guía la lectura, y las ideas de los libros se entrelazan como una red de neuronas. La portada muestra el logo **Pharus** como título principal sobre una red neuronal animada con el haz de luz del faro, y la insignia **BYMCYL** queda anclada en una esquina.

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

## 🗼 El diseño Pharus (faro + conexiones neuronales)

- **Estética de faro**: paleta de océano nocturno (azules profundos) con el haz ámbar del faro como acento. La portada (hero) tiene una **red neuronal animada** y dos **haces de luz** que barren suavemente desde el faro.
- **Logo Pharus** como título principal (`assets/pharus-dark.png` en tema oscuro: estrella/brújula dorada con el wordmark *Pharus*; `assets/pharus.png` en tema claro).
- **Logo BYMCYL** (`assets/bymcyl-dark.png` / `assets/bymcyl.png`): insignia compacta fijada en una esquina, que también cambia según el tema.
- **Conmutador de vistas** bajo la portada: **📚 Biblioteca · 🧭 Secuencias · 🕸️ Mapa de conexiones · ✨ Constelación**.

### 📚 Descubrimiento dinámico (vista por defecto)
La biblioteca abre con un **feed de descubrimiento** en lugar de una rejilla estática:
- **🔦 El faro ilumina**: un recurso destacado rotativo (uno por día, con botón «Otro» para barajar) con resumen, guía y acceso directo.
- **Chips de intención**: «Crear un hábito», «Concentrarme», «Dormir mejor», «Calmar la ansiedad»… que lanzan una búsqueda temática.
- **Carruseles horizontales**: «Continúa donde lo dejaste», «Tus favoritos», «Para empezar», «Descubre algo nuevo» (barajado), «Ciencia que puedes aplicar hoy» y una fila por cada área, con «Ver todos →».
- En cuanto buscas, filtras u ordenas, el feed da paso a la **rejilla clásica** con el contador de resultados.

### 🧭 Secuencias curadas
Rutas de lectura **en orden**, no listados sueltos: por ejemplo *«Quiero mejores hábitos»* propone 5 lecturas encadenadas. Cada secuencia (hábitos, foco, aprendizaje, calma y propósito, relaciones, decisiones, cuerpo y cerebro, creatividad) muestra sus pasos numerados con una línea de progreso que se va encendiendo conforme marcas cada lectura como leída.

### 🕸️ Mapa de conexiones
Un mapa **agrupado por áreas**: los 200 recursos se organizan en 8 clústeres etiquetados (uno por categoría) dispuestos en círculo, mucho más claro que un grafo suelto. Pasa el cursor o toca un recurso para **iluminar solo sus conexiones** (las demás se atenúan) y ver un **panel lateral** con sus relacionados; vuelve a tocarlo —o usa «Abrir ficha»— para ver su resumen. La **leyenda es interactiva**: pulsa un área para aislarla, y «↺ Ver todo» restablece. Las conexiones entre lecturas ya completadas brillan en dorado.

### ✨ Constelación = cerebro de conocimiento
Las 200 lecturas se distribuyen formando la **silueta de un cerebro** (dos hemisferios con su fisura central) y se enlazan entre sí como una **red neuronal** (cada neurona unida a sus vecinas más cercanas). Cada neurona se **enciende y titila** al marcar su lectura como leída, y las conexiones entre neuronas encendidas se iluminan en dorado: el cerebro «cobra vida» a medida que avanzas. Pulsa cualquier neurona para abrir su ficha.

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

**Identidad visual** (en `assets/`): `pharus-dark.png` y `pharus.png` (logo principal *Pharus* — estrella/brújula con wordmark — en versión para tema oscuro y claro, usado como título del hero), `bymcyl-dark.png` y `bymcyl.png` (insignia *BYMCYL* de la esquina, en sus dos temas), `logo.svg` (logotipo clásico con icono de libro + chispa de idea), `favicon.svg` (favicon de pestaña, presente en la biblioteca y en las guías) y `og-image.svg` (tarjeta para compartir, referenciada en las metaetiquetas Open Graph/Twitter de `index.html`). Nota: algunas redes no renderizan `og:image` en SVG; para esos casos conviene exportar una versión PNG (1200×630).

## ⚠️ Nota

Los resúmenes son síntesis orientativas con fines educativos: no sustituyen la lectura de las obras originales ni asesoramiento profesional. Donde la evidencia científica tiene matices o controversias (replicación, tamaños de efecto), se indica expresamente en cada ficha.
