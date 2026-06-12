# 📚 Biblioteca Práctica

Biblioteca interactiva en español con **resúmenes accionables de 58 libros y 8 estudios científicos** sobre hábitos, productividad, aprendizaje, psicología de las decisiones, relaciones, propósito y salud cerebral. Construida como páginas HTML autocontenidas, sin dependencias externas.

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
| `index.html` | **La biblioteca**: catálogo de 66 recursos (58 libros + 8 estudios) con resúmenes prácticos completos |
| `habitos-atomicos.html` | Guía interactiva completa de *Hábitos Atómicos* (James Clear) |
| `trabajo-profundo.html` | Guía interactiva completa de *Trabajo Profundo* (Cal Newport) |
| `aprendetelo.html` | Guía interactiva completa de *Apréndetelo / Make It Stick* (ciencia del aprendizaje) |
| `pensar-rapido.html` | Guía interactiva completa de *Pensar rápido, pensar despacio* (Daniel Kahneman) |
| `por-que-dormimos.html` | Guía interactiva completa de *Por qué dormimos* (Matthew Walker) |
| `meditaciones.html` | Guía interactiva completa de *Meditaciones* (Marco Aurelio y estoicismo práctico) |

## 📖 Contenido de la biblioteca

Cada recurso incluye: **idea central en una frase**, **ideas clave**, **plan de acción con checklist persistente**, **cita destacada**, **evidencia científica** (con matices y controversias señaladas honestamente), **recursos relacionados** y **notas personales**.

### Libros (58)

| Categoría | Libros |
|-----------|--------|
| 🔁 Hábitos | Hábitos Atómicos (Clear) · El poder de los hábitos (Duhigg) · Hábitos mínimos / Tiny Habits (Fogg) · Autocontrol / The Willpower Instinct (McGonigal) · El club de las 5 de la mañana (Sharma) · La magia del orden (Kondo) · Hazte la cama (McRaven) |
| 🎯 Productividad y foco | Trabajo Profundo (Newport) · Esencialismo (McKeown) · Los 7 hábitos de la gente altamente efectiva (Covey) · Organízate con eficacia / GTD (Allen) · Minimalismo digital (Newport) · Indistraíble (Eyal) · Cuatro mil semanas (Burkeman) |
| 🧠 Aprendizaje | Apréndetelo / Make It Stick (Brown, Roediger y McDaniel) · Mindset (Dweck) · Superaprendizaje / Ultralearning (Young) · Abre tu mente a los números (Oakley) · Amplitud / Range (Epstein) |
| 🧭 Psicología y decisiones | Pensar rápido, pensar despacio (Kahneman) · Influencia (Cialdini) · Grit (Duckworth) · Fluir (Csíkszentmihályi) · Sentirse bien / Feeling Good (Burns) · Drive (Pink) · Piénsalo otra vez / Think Again (Grant) · La psicología del dinero (Housel) · Aprenda optimismo (Seligman) · Tropezar con la felicidad (Gilbert) · El arte de no amargarse la vida (Santandreu) · Padre rico, padre pobre (Kiyosaki) · No me puedes lastimar / Can't Hurt Me (Goggins) |
| 🤝 Relaciones y comunicación | Cómo ganar amigos e influir sobre las personas (Carnegie) · Inteligencia emocional (Goleman) · Rompe la barrera del no (Voss) · El poder de los introvertidos / Quiet (Cain) · Frágil: el poder de la vulnerabilidad / Daring Greatly (Brown) |
| 🧘 Propósito y bienestar | El hombre en busca de sentido (Frankl) · Meditaciones (Marco Aurelio) · El obstáculo es el camino (Holiday) · La ciencia de la felicidad (Lyubomirsky) · La trampa de la felicidad (Harris) · Sé amable contigo mismo / Self-Compassion (Neff) · El poder del ahora (Tolle) · Los cuatro acuerdos (Ruiz) · Ikigai (García y Miralles) · La hipótesis de la felicidad (Haidt) · Mindfulness en la vida cotidiana (Kabat-Zinn) · Invicto (Vázquez) · Empieza con el porqué (Sinek) · Tus zonas erróneas (Dyer) · El sutil arte de que (casi) todo te importe un pimiento (Manson) |
| 💪 Cuerpo y cerebro | Por qué dormimos (Walker) · Spark: ejercicio y cerebro (Ratey) · Cómo hacer que te pasen cosas buenas (Rojas Estapé) · Generación dopamina (Lembke) · ¿Por qué las cebras no tienen úlcera? (Sapolsky) · Respira / Breath (Nestor) |

### Estudios científicos (8)

| Estudio | Tema |
|---------|------|
| Gollwitzer y Sheeran (2006) | Intenciones de implementación: planes «si-entonces» |
| Lally et al. (2010) | Cuánto tarda en formarse un hábito (66 días de media) |
| Roediger y Karpicke (2006) | El efecto test: recordar es estudiar |
| Cepeda et al. (2006) | Repaso espaciado: metaanálisis |
| Ericsson et al. (1993) | Práctica deliberada y rendimiento experto |
| Killingsworth y Gilbert (2010) | Una mente errante es una mente infeliz |
| Berman et al. (2008) | Beneficios cognitivos de la naturaleza |
| Hillman et al. (2008) | Ejercicio, cerebro y cognición |

## 🧪 Funciones interactivas

- **Búsqueda** por título, autor o contenido de las ideas
- **Filtros** por categoría (7), tipo (libro/estudio) y estado de lectura
- **Estados de lectura** (por leer / leyendo / leído) y **favoritos** ⭐
- **Checklists de acción** por recurso, con progreso persistente
- **Notas personales** por recurso con guardado automático
- **Estadísticas y barra de progreso** de la biblioteca
- Todo persiste en `localStorage` (sin cuentas ni servidores)

## 🎓 Guías interactivas completas (6)

Además de los resúmenes, seis libros tienen **guía didáctica profunda** enlazada desde su ficha: módulos navegables con progreso persistente, ejercicios interactivos y quiz final de 10 preguntas con retroalimentación.

- ⚛️ **Hábitos Atómicos** — calculadora del 1%, constructor de identidad, apilador de hábitos, rastreador semanal, diagnóstico de malos hábitos
- 🎯 **Trabajo Profundo** — clasificador de tareas, test de filosofías, constructor de rituales, marcador de horas profundas, planificador de bloques
- 📌 **Apréndetelo (Make It Stick)** — experimento de calibración, flashcards propias, planificador de repasos espaciados, plantilla Feynman, plan de estudio
- ⚖️ **Pensar rápido, pensar despacio** — test CRT, demos de anclaje y framing, corrector de estimaciones, pre-mortem, checklist antisesgos
- 😴 **Por qué dormimos** — calculadoras de cafeína y ciclos de sueño, checklist de higiene, autoevaluación orientativa
- 🏛️ **Meditaciones** — clasificador de la dicotomía del control, reformulador estoico, reencuadre de obstáculos, diario estoico persistente

## 🛠️ Tecnología

HTML + CSS + JavaScript vanilla, un archivo por página. Diseño oscuro, responsivo (escritorio y móvil), sin frameworks ni CDN.

## ⚠️ Nota

Los resúmenes son síntesis orientativas con fines educativos: no sustituyen la lectura de las obras originales ni asesoramiento profesional. Donde la evidencia científica tiene matices o controversias (replicación, tamaños de efecto), se indica expresamente en cada ficha.
