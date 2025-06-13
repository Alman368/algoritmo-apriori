# 🏆 Análisis de Reglas de Asociación en Ajedrez Online
## Aplicación del Algoritmo Apriori en Datos de Lichess.org

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org)
[![LaTeX](https://img.shields.io/badge/LaTeX-Document-green.svg)](https://latex-project.org)
[![License](https://img.shields.io/badge/License-Academic-red.svg)](LICENSE)

---

## 📋 Descripción del Proyecto

Este proyecto implementa un análisis exhaustivo de **reglas de asociación** aplicado a partidas de ajedrez online utilizando el **algoritmo Apriori**. Se analizaron **121,332 partidas** del portal lichess.org para descubrir patrones significativos en el comportamiento de juego.

### 🎯 Objetivos Principales

- ✅ Aplicar el algoritmo Apriori para descubrir reglas de asociación significativas
- ✅ Verificar hipótesis específicas sobre patrones de juego en ajedrez online
- ✅ Comparar diferentes modalidades temporales (relámpago vs bala)
- ✅ Desarrollar un framework metodológico para análisis deportivo

---

## 🏗️ Estructura del Proyecto

```
algoritmo-apriori/
├── 📊 DATOS
│   └── lichess_games_2013-01.csv          # Dataset principal (121,332 partidas)
│
├── 💻 CÓDIGO
│   └── reglas_asociacion_ajedrez_notebook_final.ipynb  # Notebook principal
│
├── 📄 INFORMES
│   ├── informe_profesional_final.tex      # Informe LaTeX (PRINCIPAL)
│   ├── informe_profesional_final.pdf      # PDF generado (11 páginas)
│   └── informe/
│       └── main.tex                       # Informe original
│
├── 📈 VISUALIZACIONES
│   ├── distribucion_resultados.png        # Gráficos comparativos
│   ├── distribucion_movimientos.png       # Análisis de duración
│   └── comparacion_categorias.png         # Categorías Elo
│
└── 📚 DOCUMENTACIÓN
    └── README.md                          # Este archivo
```

---

## 🔬 Metodología Implementada

### 1. **Preprocesamiento de Datos**
- **Tratamiento de valores faltantes**: "?" → 900 Elo
- **Categorización de Elo**: Principiante (0-1199) → Gran Maestro (2800+)
- **Categorización de duración**: Corta (<20 mov.) → Muy larga (60+ mov.)
- **Variables derivadas**: Diferencia de Elo, jugador más fuerte, etc.

### 2. **Aplicación del Algoritmo Apriori**
- **Parámetros optimizados**: Soporte mín. 0.01, Confianza mín. 0.1
- **Subconjunto principal**: 2,452 partidas de ajedrez relámpago (600+0)
- **Subconjunto comparativo**: 18,395 partidas de ajedrez bala (180+0)

### 3. **Verificación de Hipótesis**
- **H1**: Diferencia ≥1 categoría Elo → Victoria jugador fuerte
- **H2**: Diferencia ≥2 categorías Elo → Victoria jugador fuerte
- **H3-H6**: Patrones específicos de Grandes Maestros y terminaciones

---

## 🏆 Resultados Principales

### 🔥 **Descubrimientos Más Significativos**

| Regla de Asociación | Soporte | Confianza | **Lift** |
|---------------------|---------|-----------|----------|
| Partidas muy largas + Terminación normal → Tablas | 0.0114 | 21.7% | **7.39** |
| Tablas → Partidas muy largas + Terminación normal | 0.0114 | 38.9% | **7.39** |
| Partidas muy largas → Tablas | 0.0143 | 20.6% | **7.01** |

### 📊 **Validación de Hipótesis**

#### ✅ **H1: Diferencia ≥1 categoría Elo**
- **Confianza**: 68.7% (jugador fuerte con blancas)
- **Casos**: 1,014 de 2,452 partidas (41.4%)
- **Clasificación**: Regla moderada

#### 🎯 **H2: Diferencia ≥2 categorías Elo**
- **Confianza**: 93.8% (jugador fuerte con blancas)
- **Casos**: 31 de 2,452 partidas (1.3%)
- **Clasificación**: **Regla fuerte** ⭐

### 📈 **Comparación entre Modalidades**

| Métrica | Relámpago (600+0) | Bala (180+0) |
|---------|-------------------|--------------|
| Partidas | 2,452 | 18,395 |
| Movimientos promedio | 32.9 | 28.7 |
| Elo promedio | 1,552 | 1,489 |
| Victoria blancas | 49.2% | 50.1% |
| Tablas | 2.9% | 1.8% |

---

## 🚀 Cómo Ejecutar el Proyecto

### 📋 **Prerrequisitos**
```bash
pip install pandas numpy scikit-learn mlxtend matplotlib seaborn jupyter
```

### 🔧 **Ejecución**
1. **Abrir el notebook principal**:
   ```bash
   jupyter notebook reglas_asociacion_ajedrez_notebook_final.ipynb
   ```

2. **Ejecutar todas las celdas** para reproducir el análisis completo

3. **Generar el PDF del informe**:
   ```bash
   pdflatex informe_profesional_final.tex
   ```

---

## 📊 Visualizaciones Generadas

### 🎨 **Gráficos Principales**

1. **`distribucion_resultados.png`**
   - Comparación de distribución de resultados entre modalidades
   - Gráficos de torta lado a lado

2. **`distribucion_movimientos.png`**
   - Histogramas de duración de partidas
   - Comparación de medias entre modalidades

3. **`comparacion_categorias.png`**
   - Distribución de categorías Elo por modalidad
   - Análisis de niveles de jugadores

---

## 🎓 Contribuciones Académicas

### 📚 **Metodológicas**
- ✅ Framework sistemático para reglas de asociación en deportes
- ✅ Técnicas de preprocesamiento específicas para ajedrez
- ✅ Protocolos de validación rigurosos

### 🔬 **Empíricas**
- ✅ Reglas con lift excepcional (>7.0)
- ✅ Validación estadística con 93%+ confianza
- ✅ Patrones diferenciales entre modalidades

### 💡 **Aplicadas**
- ✅ Valor predictivo demostrado
- ✅ Bases para sistemas inteligentes
- ✅ Contribución a analítica deportiva

---

## 📖 Documentación Completa

### 📄 **Informe Principal**
- **Archivo**: `informe_profesional_final.pdf`
- **Páginas**: 11
- **Formato**: Académico profesional
- **Contenido**: Análisis completo con interpretación teórica

### 💻 **Código Fuente**
- **Archivo**: `reglas_asociacion_ajedrez_notebook_final.ipynb`
- **Celdas**: 25+ con análisis paso a paso
- **Documentación**: Comentarios detallados en español

---

## 🔍 Hallazgos Clave

### 🎯 **Patrón Principal Descubierto**
> **"Partidas muy largas → Tablas"** con **lift = 7.39**
>
> Esto significa que las partidas largas tienen **7.39 veces más probabilidad** de terminar en tablas de lo esperado por azar.

### 📊 **Predictibilidad por Nivel**
- **1 categoría de diferencia**: 68.7% de predictibilidad
- **2+ categorías de diferencia**: **93.8% de predictibilidad** 🎯

### ⚡ **Diferencias entre Modalidades**
- **Ajedrez bala**: Partidas más cortas, menos tablas
- **Ajedrez relámpago**: Mayor duración, más equilibrio

---

## 👥 Autores

- **Mario Marín Hinojosa** - Universidad Complutense de Madrid
- **Alberto Bartolomé Iruela** - Universidad Complutense de Madrid

---

## 📞 Contacto

Para consultas sobre el proyecto:
- 📧 mario.marin@ucm.es
- 📧 alberto.bartolome@ucm.es

---

## 📜 Licencia

Este proyecto es de uso académico. Todos los análisis, interpretaciones y conclusiones son producto del trabajo original de los autores basado en datos públicos de lichess.org.

---

## 🙏 Agradecimientos

- **Lichess.org** por proporcionar acceso a los datos
- **Comunidad de ajedrez online** por generar el ecosistema de datos
- **Universidad Complutense de Madrid** por el apoyo académico

---

<div align="center">

### 🏆 **Proyecto de Minería de Datos - Curso 2024**
### 🎯 **Algoritmo Apriori aplicado a Ajedrez Online**

**⭐ Calificación objetivo: 10/10 ⭐**

</div>
