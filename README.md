# 📚 Biblioteca Práctica

Biblioteca interactiva en español con **resúmenes accionables de libros y estudios científicos** sobre hábitos, productividad, aprendizaje, psicología de las decisiones y salud cerebral. Construida como páginas HTML autocontenidas, sin dependencias externas.

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
| `index.html` | **La biblioteca**: catálogo de 20 recursos con resúmenes prácticos completos |
| `habitos-atomicos.html` | Guía didáctica interactiva completa de *Hábitos Atómicos* (12 módulos, quiz, herramientas) |

## 📖 Contenido de la biblioteca

Cada recurso incluye: **idea central en una frase**, **ideas clave**, **plan de acción con checklist persistente**, **cita destacada**, **evidencia científica** (con matices y controversias señaladas honestamente), **recursos relacionados** y **notas personales**.

### Libros (12)

| Libro | Autor | Categoría |
|-------|-------|-----------|
| Hábitos Atómicos | James Clear | Hábitos |
| El poder de los hábitos | Charles Duhigg | Hábitos |
| Trabajo Profundo (Deep Work) | Cal Newport | Productividad y foco |
| Esencialismo | Greg McKeown | Productividad y foco |
| Apréndetelo (Make It Stick) | Brown, Roediger y McDaniel | Aprendizaje |
| Mindset: la actitud del éxito | Carol Dweck | Aprendizaje |
| Fluir (Flow) | Mihály Csíkszentmihályi | Psicología |
| Pensar rápido, pensar despacio | Daniel Kahneman | Psicología |
| Influencia | Robert Cialdini | Psicología |
| Grit | Angela Duckworth | Psicología |
| Por qué dormimos | Matthew Walker | Cuerpo y cerebro |
| Spark: ejercicio y cerebro | John Ratey | Cuerpo y cerebro |

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
- **Filtros** por categoría, tipo (libro/estudio) y estado de lectura
- **Estados de lectura** (por leer / leyendo / leído) y **favoritos** ⭐
- **Checklists de acción** por recurso, con progreso persistente
- **Notas personales** por recurso con guardado automático
- **Estadísticas y barra de progreso** de la biblioteca
- Todo persiste en `localStorage` (sin cuentas ni servidores)

## ⚛️ Guía completa de Hábitos Atómicos

La biblioteca enlaza a una guía didáctica profunda del libro de James Clear (`habitos-atomicos.html`) con 12 módulos, calculadora del 1%, constructor de identidad, apilador de hábitos, rastreador semanal, diagnóstico de malos hábitos y quiz final de 10 preguntas.

## 🛠️ Tecnología

HTML + CSS + JavaScript vanilla, un archivo por página. Diseño oscuro, responsivo (escritorio y móvil), sin frameworks ni CDN.

## ⚠️ Nota

Los resúmenes son síntesis orientativas con fines educativos: no sustituyen la lectura de las obras originales. Donde la evidencia científica tiene matices o controversias (replicación, tamaños de efecto), se indica expresamente en cada ficha.
