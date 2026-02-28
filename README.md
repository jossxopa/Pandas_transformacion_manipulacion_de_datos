# Transformación y Manipulación de Datos con Pandas 🐼

Este proyecto presenta un flujo de trabajo completo para la limpieza, transformación y estructuración de datos utilizando la librería **Pandas** en Python. El notebook se enfoca en procesar datos complejos de hosting (alojamientos) que inicialmente se encuentran en formatos anidados y con tipos de datos inconsistentes.

## 🚀 Contenido del Proyecto

El notebook [cite: 210] aborda los siguientes desafíos técnicos:

### 1. Extracción y Normalización de Datos
* **Carga de JSON:** Importación de datos desde archivos `.json` con estructuras anidadas[cite: 210].
* **Aplanamiento (Flattening):** Uso de `pd.json_normalize` para convertir diccionarios anidados dentro de columnas en un DataFrame estructurado de 13 columnas[cite: 227, 264].

### 2. Limpieza de Datos y Preprocesamiento
* **Manejo de Índices:** Reestablecimiento de índices para asegurar la unicidad de cada registro tras la expansión de datos[cite: 47].
* **Tratamiento de Caracteres Especiales:** Uso de **Expresiones Regulares (Regex)** para eliminar símbolos de moneda (`$`), comas y otros caracteres no deseados en columnas financieras[cite: 115, 156].
* **Normalización de Texto:** Conversión de descripciones a minúsculas y eliminación de ruido visual[cite: 156].

### 3. Ingeniería de Tipos de Datos
* **Conversión de Tipos:** Transformación de columnas `object` a tipos numéricos adecuados (`int64`, `float64`) para permitir cálculos estadísticos[cite: 96, 105].
* **Manejo de Fechas:** Conversión de cadenas de texto a objetos `datetime64` para análisis temporal[cite: 200, 207].
* **Optimización con Apply y Map:** Aplicación de funciones lambda para procesar múltiples columnas simultáneamente[cite: 115].

### 4. Análisis de Texto (Tokenización)
* **Tokenización:** División de descripciones textuales en unidades mínimas (tokens) para preparar los datos para posibles modelos de lenguaje o análisis de frecuencia[cite: 167, 174].

## 🛠️ Tecnologías Utilizadas

* **Python 3**
* **Pandas:** Manipulación de estructuras de datos.
* **Numpy:** Soporte para operaciones numéricas y tipos de datos avanzados[cite: 97].
* **Google Colab:** Entorno de desarrollo.

## 📈 Resultados
Al finalizar el proceso, los datos pasan de ser un conjunto de strings y diccionarios anidados a un DataFrame limpio, con tipos de datos correctos y listo para la fase de Análisis Exploratorio de Datos (EDA) o Modelado.

---
*Este proyecto fue desarrollado por Juan José Romero Xopa como parte de un proceso de aprendizaje en ciencia de datos.*
