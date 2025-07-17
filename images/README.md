# 🖼️ Images Directory

Esta carpeta contiene todas las visualizaciones e imágenes generadas durante el análisis.

## 📊 Visualizaciones Principales

### 🎯 Análisis Comparativo
- `distribucion_resultados.png` - Comparación de resultados entre modalidades
- `distribucion_movimientos.png` - Histogramas de duración de partidas
- `comparacion_categorias.png` - Distribución de niveles Elo

### 📈 Patrones de Asociación
- `top_rules_comparison.png` - Comparación de reglas más significativas
- `lift_distribution.png` - Distribución de valores lift
- `support_confidence_scatter.png` - Relación soporte vs confianza

### 🔍 Análisis Exploratorio
- `elo_distribution.png` - Distribución de puntuaciones Elo
- `timecontrol_breakdown.png` - Análisis de controles de tiempo
- `termination_patterns.png` - Patrones de finalización

## 🎨 Convenciones de Nomenclatura

```
{categoria}_{descripcion}_{modalidad}.{extension}

Ejemplos:
- analysis_elo_distribution_rapid.png
- rules_top10_blitz.png
- comparison_results_all.png
```

## 📐 Especificaciones Técnicas

- **Formato**: PNG (alta resolución), SVG (vectorial)
- **Resolución**: 300 DPI mínimo para publicación
- **Tamaño**: Optimizado para web (~1-5 MB)
- **Estilo**: Consistente con paleta del proyecto

## 🔧 Generación Automática

Las imágenes se generan automáticamente ejecutando:
```bash
jupyter notebook chess_association_analysis.ipynb
```

## 📁 Organización

```
images/
├── analysis/           # Análisis exploratorio
├── rules/             # Visualizaciones de reglas
├── comparisons/       # Análisis comparativos
└── exports/           # Versiones para publicación
```

## 🚀 Herramientas Utilizadas

- **matplotlib** - Gráficos base
- **seaborn** - Visualizaciones estadísticas
- **plotly** - Gráficos interactivos (futuro)

## 📄 Licencia

Las visualizaciones están bajo la misma licencia MIT del proyecto.
