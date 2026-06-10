# ⚛️ Hábitos Atómicos — Guía Didáctica Interactiva

Guía interactiva en español basada en el libro **_Hábitos Atómicos_ (Atomic Habits)** de **James Clear**, construida como una sola página HTML sin dependencias externas.

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

## 📚 Contenido

La guía está organizada en **12 módulos** con seguimiento de progreso automático (guardado en `localStorage`):

| # | Módulo | Temas |
|---|--------|-------|
| 0 | Introducción | Qué significa "atómico", mapa del libro |
| 1 | Fundamentos: el 1% | Interés compuesto, meseta del potencial latente, sistemas vs. metas |
| 2 | Identidad y hábitos | Las 3 capas del cambio, hábitos basados en identidad, "votos" |
| 3 | El bucle del hábito | Señal → Anhelo → Respuesta → Recompensa |
| 4 | 1ª Ley: Hazlo obvio | Scorecard, intenciones de implementación, apilamiento, diseño del entorno |
| 5 | 2ª Ley: Hazlo atractivo | Dopamina, agrupamiento de tentaciones, el poder de la tribu |
| 6 | 3ª Ley: Hazlo sencillo | Movimiento vs. acción, ley del mínimo esfuerzo, regla de los 2 minutos |
| 7 | 4ª Ley: Hazlo satisfactorio | Recompensa inmediata, rastreador de hábitos, "nunca falles dos veces" |
| 8 | Romper malos hábitos | La inversión de las 4 leyes + diagnóstico interactivo |
| 9 | Temas avanzados | Genes y juego correcto, regla Ricitos de Oro, aburrimiento, revisión |
| 10 | Herramientas prácticas | Scorecard editable, rastreador semanal, plantilla de plan de 4 leyes |
| 11 | Quiz final | 10 preguntas con retroalimentación inmediata |

## 🧪 Elementos interactivos

- **Calculadora del interés compuesto** del 1% diario
- **Tarjetas volteables** (flip cards) del bucle del hábito
- **Constructor de declaración de identidad**
- **Apilador de hábitos** (habit stacking)
- **Diagnóstico de malos hábitos** con plan de inversión generado
- **Tarjeta de puntuación de hábitos** editable y persistente
- **Rastreador semanal de hábitos** funcional
- **Generador de plan de las 4 leyes**
- **Quiz de 10 preguntas** con puntuación y retroalimentación
- **Barra de progreso** y módulos completados persistentes

## 🛠️ Tecnología

HTML + CSS + JavaScript vanilla en un solo archivo. Diseño oscuro, responsivo (escritorio y móvil), sin frameworks ni CDN.
