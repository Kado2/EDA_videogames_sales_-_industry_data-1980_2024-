# 🎮 Video Games Sales & Industry Analysis (1980 - 2024)

*Available in two languages / Disponible en dos idiomas:*
🌍 [Versión en Español](./Version_en_esp) | 🌎 [English Version](./English_version)

---

## 📌 About the Project
This project analyzes a historical dataset of over 64,000 video games, spanning 40 years of the gaming industry. The raw data was extracted from the public dataset on **[Kaggle: Video Game Sales and Industry Data (1980-2024)](https://www.kaggle.com/datasets/bhushandivekar/video-game-sales-and-industry-data-1980-2024)**.

To ensure a rigorous analysis and avoid biased conclusions, the project was designed with a modular architecture. Data extraction, cleaning, and preparation were separated from the Exploratory Data Analysis (EDA). This allowed maximizing the available data volume based on the business objective of each stage. All code was developed and executed in **Google Colab**.

## 📂 Project Structure

The project is divided into three independent notebooks:

### 1. 🧹 Data Cleaning & Preparation
* **File:** `01_Data_Cleaning.ipynb`
* **Description:** Automated process consuming the Kaggle API. This file handles structural cleaning, missing values treatment, and data integrity validation. 
* **Key Finding:** A severe completeness deficit was detected in the `total_sales` variable (67% missing values). This drove the methodological decision to fork the analysis into two separate datasets to avoid losing representativeness.
* **Output:** The cleaned data is exported to cloud storage (Google Drive) for downstream consumption.

### 2. 🏭 Industry Landscape (Volume & Production)
* **File:** `02_Industry_Landscape.ipynb`
* **Description:** Uses 100% of the cleaned data (approx. 57k records). By not relying on sales metrics, this notebook freely explores global production trends: genre evolution over decades, console lifecycles, and the productive behavior of top publishers.

### 3. 💰 Sales Analysis (Market Metrics)
* **File:** `03_Sales_Analysis.ipynb`
* **Description:** Uses the data subset with valid sales volumes (approx. 18k records). Consciously isolated from years with higher statistical noise, this analysis focuses on commercial success metrics, regional breakdowns (North America, Europe, Japan), and the impact of individual titles on the global market.

## 🛠️ Tools & Technologies
* **Language:** Python
* **Core Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Environment:** Google Colab
* **Others:** 
    * **KaggleHub**
    * **`os` and `shutil` modules**

---

## 📌 Sobre el Proyecto
Este proyecto analiza un conjunto de datos histórico de más de 64,000 videojuegos, abarcando 40 años de la industria del gaming. Los datos originales fueron extraídos del dataset público en **[Kaggle: Video Game Sales and Industry Data (1980-2024)](https://www.kaggle.com/datasets/bhushandivekar/video-game-sales-and-industry-data-1980-2024)**.

Para garantizar un análisis riguroso y evitar conclusiones sesgadas, el proyecto fue diseñado con una arquitectura modular. Se separó la extracción, limpieza y preparación de los datos del análisis exploratorio (EDA), permitiendo aprovechar al máximo el volumen de datos disponible según el objetivo de negocio de cada etapa. Todo el código fue desarrollado y ejecutado en **Google Colab**.

## 📂 Estructura del Análisis

El proyecto está dividido en tres *notebooks* independientes:

### 1. 🧹 Data Cleaning (Limpieza y Preparación)
* **Archivo:** `01_Data_Cleaning.ipynb`
* **Descripción:** Proceso consumiendo la API de Kaggle. En este archivo se realiza la limpieza estructural, el tratamiento de valores nulos y la validación de la integridad de los datos. 
* **Hallazgo Clave:** Se detectó un déficit de completitud severo en la variable `total_sales` (67% de nulos). Esto motivó la decisión de bifurcar el análisis en dos para no perder representatividad.
* **Output:** Los datos limpios se exportan a un almacenamiento en la nube (Google Drive) para su consumo posterior.

### 2. 🏭 Panorama de la Industria (Volumen y Producción)
* **Archivo:** `02_Industry_Landscape.ipynb`
* **Descripción:** Utiliza el 100% de los datos limpios (aprox. 57k registros). Al no depender de las métricas de ventas, este cuaderno explora libremente las tendencias globales de producción: evolución de géneros a lo largo de las décadas, ciclo de vida de las consolas y el comportamiento productivo de los principales editores (*publishers*).

### 3. 💰 Análisis de Ventas (Métricas de Mercado)
* **Archivo:** `03_Sales_Analysis.ipynb`
* **Descripción:** Utiliza el subconjunto de datos con volumen de ventas válido (aprox. 18k registros). Aislado conscientemente de los años con mayor ruido estadístico, este análisis se enfoca en responder métricas de éxito comercial, análisis por regiones (Norteamérica, Europa, Japón) y el impacto de títulos individuales en el mercado global.

## 🛠️ Herramientas utilizadas
* **Lenguaje:** Python
* **Librerías principales:** Pandas, NumPy, Matplotlib, Seaborn
* **Entorno:** Google Colab
* **Otros:** 
    * **KaggleHub**
    * **Módulos `os` y `shutil`**
