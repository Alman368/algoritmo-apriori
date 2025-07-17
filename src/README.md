# 🧩 Source Code Directory

Esta carpeta está reservada para módulos y scripts auxiliares del proyecto.

## 📋 Estructura Planificada

```
src/
├── preprocessing/
│   ├── __init__.py
│   ├── data_cleaner.py      # Funciones de limpieza de datos
│   └── categorizer.py       # Sistema de categorización automática
├── algorithms/
│   ├── __init__.py
│   ├── apriori_wrapper.py   # Wrapper optimizado para Apriori
│   └── rule_analyzer.py     # Análisis avanzado de reglas
├── visualization/
│   ├── __init__.py
│   ├── plotters.py          # Funciones de visualización
│   └── report_generator.py  # Generación automática de reportes
└── utils/
    ├── __init__.py
    ├── helpers.py           # Funciones auxiliares
    └── config.py            # Configuración del proyecto
```

## 🚀 Funcionalidades Futuras

### 📊 Preprocessing
- Limpieza automática de datasets de ajedrez
- Categorización inteligente de variables
- Detección y manejo de outliers
- Normalización de formatos de tiempo

### 🔍 Algorithms
- Implementación optimizada de Apriori
- Algoritmos alternativos (FP-Growth, Eclat)
- Evaluación automatizada de reglas
- Sistema de ranking de patrones

### 📈 Visualization
- Gráficos interactivos con Plotly
- Dashboards dinámicos
- Exportación automática de figuras
- Reportes PDF automatizados

### 🛠️ Utils
- Configuración centralizada
- Logging avanzado
- Validación de datos
- Helpers para análisis estadístico

## 🔧 Instalación de Dependencias

```bash
pip install -r requirements.txt
```

## 📝 Convenciones de Código

- **Estilo**: PEP 8
- **Docstrings**: Google Style
- **Type Hints**: Obligatorios para funciones públicas
- **Testing**: pytest para pruebas unitarias

## 🤝 Contribuciones

Ver [CONTRIBUTING.md](../CONTRIBUTING.md) para guías de contribución específicas a esta carpeta.
