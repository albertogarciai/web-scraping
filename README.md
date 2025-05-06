# 📊 Análisis de Datos Climáticos y Web Scraping Meteorológico

[![Author](https://img.shields.io/badge/author-albertogarciai-blue)](https://github.com/albertogarciai)

## Descripción del Proyecto

Este repositorio contiene dos componentes principales orientados al análisis y obtención de datos meteorológicos históricos:

- **`datos_climaticos_limpios_20250224_010353.csv`**:  
  Un conjunto de datos limpios y estructurados con registros mensuales de temperaturas (media, mínima y máxima) y precipitaciones totales desde 1974 hasta la actualidad.

- **`web_scraping.ipynb`**:  
  Un notebook en Jupyter que implementa un sistema automatizado de scraping para recopilar datos climáticos históricos desde el portal [tutiempo.net](https://www.tutiempo.net). Incluye técnicas modernas como:

  - Requests + BeautifulSoup para la recolección de datos.
  - Gestión de pausas automáticas para evitar bloqueos.
  - Visualización de los datos usando Matplotlib, Seaborn y Plotly.
  - Modelado predictivo simple usando regresión lineal para explorar tendencias.

## Estructura del Dataset

| Columna               | Descripción                         |
|-----------------------|-------------------------------------|
| Fecha                 | Fecha del registro (año y mes)      |
| Ano                   | Año del registro                    |
| Mes                   | Mes del registro                    |
| Temp Media            | Temperatura media mensual (°C)      |
| Temp Minima          | Temperatura mínima mensual (°C)     |
| Temp Maxima          | Temperatura máxima mensual (°C)     |
| Precipitaciones Totales | Total de precipitaciones (mm)    |

## Objetivos

- Proveer un dataset limpio de referencia sobre condiciones climáticas históricas.
- Automatizar la recolección de nuevos datos mediante técnicas de scraping.
- Visualizar tendencias a largo plazo para explorar posibles efectos del cambio climático.

## Cómo usar este repositorio

### 📥 Clonar el repositorio

```bash
git clone https://github.com/albertogarciai/clima-historico.git
cd clima-historico
```

### 📦 Requisitos

Instala las dependencias necesarias:

```bash
pip install -r requirements.txt
```

### 🚀 Ejecutar el Web Scraping

Abre el archivo `web_scraping.ipynb` en Jupyter Notebook o VSCode y ejecuta todas las celdas para descargar y procesar datos meteorológicos.

### 📊 Analizar los datos

El archivo CSV se puede cargar fácilmente con Pandas para su análisis:

```python
import pandas as pd

df = pd.read_csv("datos_climaticos_limpios_20250224_010353.csv")
print(df.head())
```

### 📈 Visualizar tendencias

El notebook incluye ejemplos de cómo graficar las temperaturas y precipitaciones para analizar tendencias a largo plazo.

## Licencia

Este proyecto está licenciado bajo la licencia MIT. Consulta el archivo `LICENSE` para obtener más detalles.

## Autor

Creado con pasión por [albertogarciai](https://github.com/albertogarciai).  
Si te resulta útil este repositorio, ¡no dudes en dar una ⭐️!