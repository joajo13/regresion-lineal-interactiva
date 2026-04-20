# Regresión Lineal con Gradient Descent

Visualizador interactivo de **regresión lineal** entrenada con **descenso de gradiente**, en una sola página HTML. Pensado para entender de verdad qué hace el optimizador, no sólo ver la recta final.

**Demo en vivo:** https://joajo13.github.io/regresion-lineal-interactiva/

## Qué tiene

- Canvas interactivo: clickeá para agregar puntos y la recta se ajusta sola.
- Controles de **learning rate**, pasos manuales, reset y dataset de ejemplo.
- Métricas en tiempo real: pendiente (m), intercepto (b), loss (MSE) y gradientes ∂L/∂m y ∂L/∂b.
- Sección de teoría con derivadas, gradiente y un **visualizador del "tazón"** (curvas de nivel del error) donde se ve la flecha del gradiente apuntando cuesta arriba.
- Fórmulas renderizadas con KaTeX, tipografía JetBrains Mono para el código y Inter para el texto.

## Preview

![Sección principal](regresion-lineal-inicial.png)

![Después de converger](regresion-lineal-convergida.png)

![Teoría — gradiente y tazón](grad-section.png)

## Cómo correrlo local

No hay build. Abrí `index.html` en el browser y listo. Si preferís un server:

```bash
python -m http.server 8000
# o
npx serve .
```

## Stack

- HTML + CSS + JS vanilla, cero dependencias de build.
- [KaTeX](https://katex.org/) vía CDN para las fórmulas.
- Google Fonts (Inter + JetBrains Mono).

## Licencia

MIT.
