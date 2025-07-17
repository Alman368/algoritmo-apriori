# 📊 Data Directory

Esta carpeta contiene los datasets utilizados en el análisis de reglas de asociación de ajedrez.

## 📁 Archivos

### `lichess_games_2013-01.csv`
- **Fuente**: lichess.org
- **Período**: Enero 2013
- **Tamaño**: ~11 MB
- **Registros**: 121,332 partidas
- **Formato**: CSV con 11 columnas

### 📋 Estructura del Dataset

| Columna | Tipo | Descripción |
|---------|------|-------------|
| `Site` | string | URL de la partida en lichess |
| `White` | string | Nombre del jugador con piezas blancas |
| `Black` | string | Nombre del jugador con piezas negras |
| `Result` | string | Resultado (1-0, 0-1, 1/2-1/2) |
| `WhiteElo` | string/int | Puntuación Elo del jugador blanco |
| `BlackElo` | string/int | Puntuación Elo del jugador negro |
| `TimeControl` | string | Control de tiempo (ej: 600+0, 60+0) |
| `ECO` | string | Código de apertura ECO |
| `Opening` | string | Nombre de la apertura |
| `Termination` | string | Tipo de finalización |
| `MovesCount` | int | Número total de movimientos |

### 🔍 Notas sobre los Datos

- **Valores faltantes**: Algunos Elo aparecen como "?" (tratados como 900)
- **Controles de tiempo**: Variedad de formatos, principales: 600+0, 60+0, 180+0
- **Calidad**: Dataset limpio sin valores nulos críticos
- **Origen**: Partidas reales de usuarios de lichess.org

### 🚀 Uso

```python
import pandas as pd
df = pd.read_csv('data/lichess_games_2013-01.csv')
```

### 📄 Licencia de Datos

Los datos son de dominio público, proporcionados por lichess.org bajo su política de datos abiertos.
