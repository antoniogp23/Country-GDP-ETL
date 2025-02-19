# ETL Pipeline for Country GDP Data
## Description
This project implements an ETL (Extract, Transform, Load) pipeline to collect country GDP data from Wikipedia. The data is processed and stored in a CSV file and an SQLite database for further analysis.
## Process Overview
The ETL pipeline follows these steps:

1. **Extract**:
- Fetches the GDP data from a Wikipedia page.
- Parses the HTML content using BeautifulSoup.
- Extracts country names and their corresponding GDP values in millions of USD.

2. **Transform:**
- Cleans the GDP values by removing commas and converting them to float.
- Converts GDP values from millions to billions of USD.
- Renames the column from GDP_USD_millions to GDP_USD_billions.

3. **Load:**
- Saves the processed data into a CSV file.
- Loads the data into an SQLite database.
- Runs a query to display countries with a GDP of at least 100 billion USD.

## Files Included
- `etl_script.py`: The Python script that executes the ETL process.
- `Countries_by_GDP.csv`: Output CSV file containing the processed data.
- `World_Economies.db`: SQLite database storing the country GDP data.
- `etl_project_log.txt`: Log file recording the progress of the ETL process.

## Dependencies
The script requires the following Python libraries:
- `requests`
- `beautifulsoup4`
- `pandas`
- `numpy`
- `sqlite3`

Ensure you have these installed before running the script.
### Acknowledgments
This project was inspired by the "Data Engineering" course by IBM on Coursera. The concepts and techniques used in this script were learned through this course.

---

# Pipeline ETL para Datos del PIB por País

## Descripción

Este proyecto implementa un pipeline ETL (Extraer, Transformar, Cargar) para recopilar datos del PIB de los países desde Wikipedia. Los datos se procesan y almacenan en un archivo CSV y en una base de datos SQLite para su posterior análisis.

## Resumen del Proceso

El pipeline ETL sigue estos pasos:

1. **Extracción:**
   - Obtiene los datos del PIB de una página de Wikipedia.
   - Analiza el contenido HTML usando BeautifulSoup.
   - Extrae los nombres de los países y sus valores de PIB en millones de USD.

2. **Transformación:**
   - Limpia los valores del PIB eliminando comas y convirtiéndolos en números flotantes.
   - Convierte los valores del PIB de millones a miles de millones de USD.
   - Cambia el nombre de la columna de `GDP_USD_millions` a `GDP_USD_billions`.

3. **Carga:**
   - Guarda los datos procesados en un archivo CSV.
   - Carga los datos en una base de datos SQLite.
   - Ejecuta una consulta para mostrar los países con un PIB de al menos 100 mil millones de USD.

## Archivos Incluidos

- `etl_script.py`: El script de Python que ejecuta el proceso ETL.
- `Countries_by_GDP.csv`: Archivo CSV de salida con los datos procesados.
- `World_Economies.db`: Base de datos SQLite que almacena los datos del PIB por país.
- `etl_project_log.txt`: Archivo de registro que documenta el progreso del proceso ETL.

## Dependencias

El script requiere las siguientes bibliotecas de Python:

- `requests`
- `beautifulsoup4`
- `pandas`
- `numpy`
- `sqlite3`

Asegúrate de tenerlas instaladas antes de ejecutar el script.

### Agradecimientos
Este proyecto fue inspirado por el curso "Data Engineering" de IBM en Coursera. Los conceptos y técnicas utilizados en este script fueron aprendidos a través de este curso.
