<div align="center">

# 📊 El Ecosistema de la Programación en España
### Evolución, Interés y Demanda Laboral (2021–2026)

[![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-3.0-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Plotly](https://img.shields.io/badge/Plotly-Interactive-3F4F75?logo=plotly&logoColor=white)](https://plotly.com/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![YouTube API](https://img.shields.io/badge/YouTube-Data%20API%20v3-FF0000?logo=youtube&logoColor=white)](https://developers.google.com/youtube/v3)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

*Análisis exploratorio de datos que triangula tres fuentes clave para descifrar el panorama tecnológico real en España.*

</div>

---

## 🎯 Objetivo

Este EDA investiga cómo ha evolucionado el ecosistema de los lenguajes de programación en España entre 2021 y 2026, cruzando **uso profesional**, **interés de aprendizaje** y **demanda laboral** para responder a preguntas como:

- ¿Qué lenguajes dominan realmente el mercado laboral español?
- ¿Coincide el "hype" en redes con la demanda real de empleo?
- ¿Cómo está transformando la IA las formas de aprender a programar?
- ¿Qué tecnologías están en auge y cuáles en declive?

---

## 📐 Fuentes de Datos

| Fuente | Descripción | Periodo |
|--------|-------------|---------|
| [**Stack Overflow Developer Survey**](https://survey.stackoverflow.co/) | Encuesta anual a desarrolladores: lenguajes usados/deseados, salarios, métodos de aprendizaje, sentimiento IA | 2021–2025 |
| [**Google Trends (YouTube)**](https://trends.google.es/) | Tendencias de búsqueda filtradas por España y categoría YouTube | 2021–2026 |
| **YouTube Data API v3** | Métricas de engagement (views, comentarios, duración) de vídeos técnicos seleccionados | 2026 |
| **LinkedIn Jobs / InfoJobs** | Muestreo directo de vacantes activas por lenguaje en España | Abril 2026 |

---

## 🔬 Análisis Realizados

### 1. Participación: España vs. Mundo
Evolución del volumen de respuestas españolas en Stack Overflow y su caída coincidiendo con la irrupción de los LLMs.

### 2. Geolocalización de Respuestas
Mapa interactivo (Plotly) de la distribución mundial de encuestados, evidenciando la hegemonía de EE.UU. e India.

### 3. El "Hype Ratio": Uso vs. Deseo
Comparativa de los lenguajes más usados frente a los más deseados. Métricas clave:
- **Emergentes** (alto Hype Ratio): Rust, Go, Dart
- **Consolidados** (ratio ≈ 1): JavaScript, Python, Java
- **En declive** (ratio bajo): PHP, Cobol

### 4. Evolución Temporal por Lenguaje (8 lenguajes)
Gráficos duales (valores absolutos + porcentuales) cruzando Stack Overflow con Google Trends para: **JavaScript, SQL, Python, HTML/CSS, TypeScript, Java, C# y PHP**.

### 5. Análisis Salarial
Heatmap de medianas salariales por lenguaje y año, utilizando la mediana para mitigar outliers.

### 6. Métodos de Aprendizaje Online
Categorización granular de 14 métodos de formación (vídeo, documentación, IA, tutoriales interactivos, gamificación, podcasts...) y su evolución temporal.

### 7. Engagement en YouTube
Análisis de ratio de interacción (comentarios/visitas) por lenguaje, con gráfico de burbujas que relaciona duración y participación.

### 8. Mapa Estratégico 2026: Demanda vs. Comunidad
Gráfico de dispersión que cruza ofertas de empleo reales en España con el engagement en YouTube, revelando la segmentación del mercado.

---

## 💡 Hallazgos Principales

### Mapa del Ecosistema

| Segmento | Lenguajes | Ofertas ES | Engagement | Perfil |
|----------|-----------|:----------:|:----------:|--------|
| **Dominio Corporativo** | Java, JavaScript, C# | ⬆️ Alto | ⬇️ Bajo | Consumo pragmático, orientado a productividad |
| **Comunidad Activa** | Python | ⬆️ Alto | ⬆️ **Muy alto** (5.81) | Participación activa, motor de IA/Data Science |
| **Nicho Resiliente** | PHP | ⬇️ Bajo | ➡️ Medio | Base autodidacta vocal, soporte social |
| **Emergentes** | Rust, Go, TypeScript | ⬇️ Bajo | ⬆️ Alto | Alto deseo con base de uso aún pequeña |

### Conclusiones Clave

1. **Dualidad Mercado-Comunidad** — Existe un desacoplamiento entre las tecnologías que generan más empleo (Java/JS) y las que generan más pasión (Python/IA). El éxito profesional reside en la hibridación estratégica.

2. **Migración de ecosistemas de aprendizaje** — La caída de búsquedas en YouTube responde a la aparición de nuevas plataformas basadas en IA (NotebookLM, Copilot) y certificaciones oficiales (Google Skills, Microsoft Learn, Exercism).

3. **La IA como catalizador, no sustituto** — La IA no está eliminando lenguajes, sino revalorizando a aquellos que sirven de puente (Python). El interés de aprendizaje hoy es un indicador adelantado de la demanda laboral de mañana.

4. **Madurez del sector en España** — Mercado dominado por backend robusto (Java) y web (JavaScript/TypeScript), pero las nuevas generaciones priorizan ecosistemas con mayor soporte comunitario.

> **Veredicto Final:** El éxito profesional en 2026 reside en la **Hibridación Estratégica**: combinar la solidez laboral de **Java y JavaScript** con la agilidad y potencia para IA que ofrece **Python**.

---

## 🗂️ Estructura del Proyecto

```
EDA-programacion-tendencias/
├── 📓 analisis-Stack-Overflow.ipynb   # Notebook principal del EDA
├── 📄 README.md
├── 🔑 .env                            # API Key de YouTube (no incluida)
├── 📁 data/                            # Datasets fuente (ver sección Datos)
│   ├── stack-overflow-developer-survey-2021.csv
│   ├── stack-overflow-developer-survey-2022.csv
│   ├── stack-overflow-developer-survey-2023.csv
│   ├── stack-overflow-developer-survey-2024.csv
│   ├── stack-overflow-developer-survey-2025.csv
│   └── tendencias_lenguajes.csv
├── 📁 export_csv/                      # Datos procesados para dashboards
│   ├── distribucion_geografica_encuestados.csv
│   ├── salarios_top_10_lenguajes.csv
│   ├── metodos_aprendizaje_online.csv
│   ├── evolucion_[lenguaje].csv        # Series temporales por lenguaje
│   └── ...
└── 📁 img/                             # Imágenes de apoyo
```

---

## ⚙️ Instalación y Ejecución

### Requisitos previos

- Python 3.11+
- Jupyter Notebook / VS Code con extensión Jupyter

### Instalación

```bash
# Clonar el repositorio
git clone https://github.com/jlalonsoredon/EDA-programacion-tendencias.git
cd EDA-programacion-tendencias

# Instalar dependencias
pip install pandas numpy matplotlib seaborn plotly pycountry google-api-python-client python-dotenv
```

### Configuración de la API de YouTube (opcional)

Las secciones de engagement requieren una API Key de YouTube Data API v3:

1. Crea un proyecto en [Google Cloud Console](https://console.cloud.google.com)
2. Habilita **YouTube Data API v3**
3. Genera una API Key
4. Crea un archivo `.env` en la raíz:
   ```
   API_KEY=tu_api_key_aqui
   ```

### Datos de Stack Overflow

Los archivos CSV superan el límite de 100 MB de GitHub y no están incluidos en el repositorio.

1. Ve a la sección [**Releases**](https://github.com/jlalonsoredon/EDA-programacion-tendencias/releases) de este repositorio y descarga los CSV
2. Colócalos en la carpeta `data/`

Alternativamente, descárgalos directamente desde [Stack Overflow](https://survey.stackoverflow.co/).

---

## 🛠️ Stack Tecnológico

| Librería | Uso |
|----------|-----|
| `pandas` / `numpy` | Manipulación y análisis de datos |
| `matplotlib` / `seaborn` | Visualizaciones estáticas (heatmaps, barras, líneas) |
| `plotly` | Visualizaciones interactivas (mapas, pie charts) |
| `pycountry` | Conversión de nombres de países a ISO-3 |
| `google-api-python-client` | Conexión con YouTube Data API v3 |
| `python-dotenv` | Gestión segura de credenciales |

---

## 👤 Autor

**Jose Luis Alonso** — [GitHub](https://github.com/jlalonsoredon)

---

<div align="center">

*Proyecto EDA realizado como parte del Bootcamp de Data Science en [The Bridge](https://www.thebridge.tech/) — Bilbao 2026*

</div>
