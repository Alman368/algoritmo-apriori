# 📝 Changelog

Todos los cambios notables en este proyecto serán documentados en este archivo.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
y este proyecto adhiere a [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2024-01-XX

### ✨ Añadido
- Implementación inicial del algoritmo Apriori para análisis de partidas de ajedrez
- Análisis completo de dataset lichess.org con 121,332 partidas
- Sistema de categorización automática de variables (Elo, duración, etc.)
- Verificación estadística de 6 hipótesis específicas sobre patrones de juego
- Comparación entre modalidades de ajedrez rápido (600+0) y blitz (60+0)
- Visualizaciones interactivas de resultados y patrones
- Documentación completa con README profesional
- Estructura de proyecto organizada con carpetas dedicadas

### 🔧 Características Técnicas
- Preprocesamiento avanzado de datos con manejo de valores faltantes
- Implementación optimizada de Apriori con umbrales configurables
- Cálculo de métricas de asociación (soporte, confianza, lift)
- Sistema de interpretación automática de reglas
- Generación automática de reportes y visualizaciones

### 📊 Resultados Principales
- Descubrimiento de regla con lift 7.39: "Partidas muy largas → Tablas"
- Validación de hipótesis con 93.7% de confianza para diferencias de Elo
- Identificación de patrones diferenciales entre modalidades de juego
- Análisis de 9,346+ reglas de asociación en ajedrez rápido
- Análisis de 9,423+ reglas de asociación en ajedrez blitz

### 📁 Estructura
- `/data/` - Dataset original de lichess.org
- `/src/` - Scripts y módulos auxiliares (futuro)
- `/docs/` - Documentación adicional
- `/images/` - Visualizaciones generadas
- Notebook principal: `chess_association_analysis.ipynb`
- Configuración: `requirements.txt`, `.gitignore`
- Documentación: `README.md`, `CONTRIBUTING.md`, `LICENSE`

---

## 🚀 Próximas Versiones

### [1.1.0] - Planificado
- [ ] Análisis de aperturas específicas (códigos ECO)
- [ ] Implementación de algoritmos adicionales (FP-Growth)
- [ ] Dashboard interactivo con Streamlit/Dash
- [ ] API REST para consulta de patrones

### [1.2.0] - Planificado
- [ ] Análisis temporal de evolución de patrones
- [ ] Integración con múltiples datasets de ajedrez
- [ ] Sistema de recomendaciones basado en patrones
- [ ] Módulo de predicción de resultados

---

## 📋 Tipos de Cambios

- **✨ Añadido** para nuevas funcionalidades
- **🔧 Cambiado** para cambios en funcionalidades existentes
- **❌ Depreciado** para funcionalidades que serán removidas
- **🗑️ Removido** para funcionalidades removidas
- **🐛 Arreglado** para correcciones de bugs
- **🔒 Seguridad** para vulnerabilidades
