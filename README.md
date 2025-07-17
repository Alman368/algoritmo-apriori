# ♟️ Chess Association Rules Mining

> **Descubriendo patrones ocultos en partidas de ajedrez usando el algoritmo Apriori**

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org)
[![Pandas](https://img.shields.io/badge/Pandas-2.0+-green.svg)](https://pandas.pydata.org)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Paper](https://img.shields.io/badge/Paper-PDF-red.svg)](docs/informe.pdf)

## 📋 Descripción

Este proyecto implementa el **algoritmo Apriori** para descubrir reglas de asociación en un extenso dataset de partidas de ajedrez de lichess.org. A través del análisis de más de 120,000 partidas, identificamos patrones significativos que revelan relaciones entre variables como el nivel de los jugadores, duración de las partidas y resultados.

### 🎯 Objetivos

- **Implementación práctica del algoritmo Apriori** para minería de reglas de asociación
- **Análisis de patrones de juego** en diferentes modalidades de ajedrez
- **Verificación de hipótesis** sobre factores que influyen en el resultado de las partidas
- **Comparación entre modalidades** de ajedrez rápido (600+0) y blitz (60+0)

## 🚀 Características Principales

- ✅ **Preprocesamiento avanzado** de datos con categorización inteligente
- ✅ **Implementación del algoritmo Apriori** con métricas de soporte, confianza y lift
- ✅ **Análisis comparativo** entre diferentes controles de tiempo
- ✅ **Verificación estadística** de hipótesis específicas
- ✅ **Visualizaciones interactivas** de los resultados
- ✅ **Documentación completa** con interpretación de resultados
- ✅ **Informe académico** detallado en formato PDF

## 📊 Dataset

**Fuente:** lichess.org - Partidas de enero 2013
**Tamaño:** 121,332 partidas
**Variables:** 11 columnas incluyendo Elo, resultado, control de tiempo, apertura, etc.

### Variables Analizadas

| Variable | Descripción | Categorización |
|----------|-------------|----------------|
| **Elo** | Puntuación de los jugadores | Principiante, Intermedio, Avanzado, Experto, Maestro, GM |
| **Duración** | Número de movimientos | Corta (<20), Media (20-39), Larga (40-59), Muy larga (60+) |
| **Control de tiempo** | Tiempo asignado por jugador | 600+0 (Rápido), 60+0 (Blitz) |
| **Resultado** | Resultado de la partida | 1-0, 0-1, 1/2-1/2 |

## 🔧 Instalación

1. **Clona el repositorio:**
```bash
git clone https://github.com/tu-usuario/chess-association-rules.git
cd chess-association-rules
```

2. **Instala las dependencias:**
```bash
pip install -r requirements.txt
```

3. **Ejecuta el notebook:**
```bash
jupyter notebook chess_association_analysis.ipynb
```

## 📈 Resultados Principales

### 🏆 Reglas de Asociación Descubiertas

| Regla | Soporte | Confianza | Lift | Interpretación |
|-------|---------|-----------|------|----------------|
| `Partidas muy largas → Tablas` | 0.014 | 0.486 | 7.01 | **Fuerte asociación** |
| `Diferencia ≥2 categorías Elo → Victoria jugador fuerte` | 0.006 | 0.937 | 4.42 | **Predictor robusto** |
| `Jugadores principiantes → Mayor frecuencia de derrotas por tiempo` | 0.089 | 0.312 | 2.87 | **Patrón consistente** |

### 📊 Hallazgos Clave

- **Efecto de la diferencia de nivel:** Cuando hay 2+ categorías de diferencia en Elo, el jugador más fuerte gana en el 93.7% de los casos
- **Duración y resultado:** Las partidas muy largas (60+ movimientos) terminan en tablas 7 veces más frecuentemente que el promedio
- **Control de tiempo:** El ajedrez blitz muestra patrones diferentes al ajedrez rápido, con mayor frecuencia de derrotas por tiempo

## 🧪 Metodología

### 1. Preprocesamiento
- Limpieza y normalización de datos
- Categorización de variables continuas
- Creación de variables derivadas

### 2. Aplicación de Apriori
- Configuración de umbrales mínimos de soporte
- Generación de itemsets frecuentes
- Extracción de reglas de asociación

### 3. Evaluación
- Cálculo de métricas (soporte, confianza, lift)
- Validación estadística de hipótesis
- Interpretación de resultados

## 📁 Estructura del Proyecto

```
chess-association-rules/
├── 📄 README.md                          # Este archivo
├── 📓 chess_association_analysis.ipynb   # Notebook principal
├── 📋 requirements.txt                   # Dependencias
├── 📄 informe.tex                        # Código fuente LaTeX del informe
├── 📂 data/
│   ├── README.md                         # Documentación del dataset
│   └── lichess_games_2013-01.csv        # Dataset original
├── 📂 src/                               # Scripts auxiliares (futuro)
│   └── README.md
├── 📂 docs/                              # Documentación y reportes
│   ├── README.md                         # Guías y referencias
│   └── informe.pdf                       # 📑 Informe académico completo
└── 📂 images/                            # Visualizaciones generadas
    └── README.md
```

## 📑 Documentación Adicional

- **🔬 [Informe Académico Completo](docs/informe.pdf)** - Análisis detallado con metodología, resultados y conclusiones (11 páginas)
- **💻 [Notebook Interactivo](chess_association_analysis.ipynb)** - Implementación paso a paso del análisis
- **📊 [Documentación del Dataset](data/README.md)** - Especificación completa de los datos

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Haz fork del proyecto
2. Crea una rama para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. Commit tus cambios (`git commit -am 'Añade nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

## 📚 Referencias

- **Algoritmo Apriori:** Agrawal, R., & Srikant, R. (1994)
- **Dataset:** lichess.org - Plataforma de ajedrez online
- **Librerías:** pandas, mlxtend, scikit-learn, matplotlib, seaborn

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 👤 Autor

**Tu Nombre**
- GitHub: [@tu-usuario](https://github.com/tu-usuario)
- LinkedIn: [tu-perfil](https://linkedin.com/in/tu-perfil)

---

⭐ **¡Dale una estrella si te gusta el proyecto!** ⭐
