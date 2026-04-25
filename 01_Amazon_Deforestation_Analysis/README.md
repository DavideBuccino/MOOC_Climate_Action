*Read this in other languages: [🇮🇹 Italiano](#-italiano) | [🇬🇧 English](#-english)*

---

# 🇮🇹 Italiano

# 🌳 Quantificare la Deforestazione Amazzonica in Rondônia (1992-2020)

![ArcGIS Pro](https://img.shields.io/badge/ArcGIS_Pro-3.x-blue?style=for-the-badge&logo=esri)
![Spatial Analyst](https://img.shields.io/badge/Spatial_Analyst-Extension-108A44?style=for-the-badge)
![Living Atlas](https://img.shields.io/badge/ArcGIS_Living_Atlas-Data-orange?style=for-the-badge)

## 📌 Panoramica del Progetto
Quanti chilometri quadrati di foresta amazzonica sono svaniti in Rondônia, uno dei fronti più caldi della deforestazione brasiliana, tra il 1992 e il 2020? 

Questo progetto esplora il disastroso "arco della deforestazione" andando oltre i semplici confronti visivi. Utilizzando dati satellitari storici e strumenti di analisi spaziale avanzata, ho quantificato l'area esatta di spazio verde convertita in terreni agricoli e tessuto urbano nel corso di quasi tre decenni.

### 🎥 Dimostrazione del Workflow e Risultati
*(Trascina e rilascia qui il tuo file .mp4)*

---

## 🛠️ Strumenti e Tecnologie
* **Software:** ArcGIS Pro
* **Estensioni:** Spatial Analyst, Image Analyst
* **Fonte Dati:** Dati della Climate Change Initiative dell'Agenzia Spaziale Europea (ESA) tramite **ArcGIS Living Atlas of the World** (Global Land Cover 1992-2020).

---

## 🔬 Workflow Tecnico

1. **Acquisizione Dati e Filtraggio:**
   * Importazione del raster multi-temporale della copertura del suolo globale (Global Land Cover) dall'ArcGIS Living Atlas.
   * Applicazione di **Query di Definizione (Definition Queries)** per isolare i dati specifici di copertura del suolo per gli anni 1992 e 2020.

2. **Calcolo dell'Area:**
   * Utilizzo della tabella degli attributi per calcolare l'area esatta in chilometri quadrati per ogni classificazione di copertura del suolo. 
   * Data la risoluzione spaziale del raster (dimensione dei pixel 300m x 300m), ho creato un nuovo campo `Area_SqKM` e applicato uno script di calcolo Python: `(!Count! * 90000) * 0.000001`.

3. **Analisi di Rilevamento dei Cambiamenti (Change Detection):**
   * Utilizzo dello strumento **Compute Change Raster** (Image Analyst) impiegando il metodo di *Differenza Categoriale*.
   * Questo ha generato un nuovo raster che evidenzia solo i pixel modificati, individuando con precisione le posizioni e le classificazioni in cui la foresta ("Closed to Open Canopy Broadleaved") è transitata principalmente in terreni coltivati ("Rainfed/Herbaceous Cropland") e aree urbane.

---

## 💡 Conclusioni Principali
Questa analisi dimostra che i dati spaziali sono molto più che semplici punti e poligoni su una mappa: rappresentano un potente radar per leggere la geopolitica e le dinamiche ambientali. Saper interrogare e standardizzare i dati raster fornisce basi solide e quantitative per analizzare seriamente le sfide più critiche del nostro pianeta.

> *Questo progetto è stato sviluppato come esercitazione pratica all'interno del MOOC "GIS for Climate Action" di Esri.*

<br><br>

---

# 🇬🇧 English

# 🌳 Quantifying Amazon Deforestation in Rondônia (1992-2020)

## 📌 Project Overview
How many square kilometers of the Amazon rainforest have vanished in Rondônia, one of Brazil's most intense deforestation fronts, between 1992 and 2020? 

This project explores the disastrous "arc of deforestation" by going beyond simple visual comparisons. Using historical satellite data and advanced spatial analysis, I quantified the exact area of green space converted into agricultural land and urban fabric over nearly three decades.

### 🎥 Workflow & Results Demonstration
*(Drag and drop your .mp4 file here)*

---

## 🛠️ Tools & Technologies
* **Software:** ArcGIS Pro
* **Extensions:** Spatial Analyst, Image Analyst
* **Data Source:** European Space Agency (ESA) Climate Change Initiative data via **ArcGIS Living Atlas of the World** (Global Land Cover 1992-2020).

---

## 🔬 Technical Workflow

1. **Data Acquisition & Filtering:**
   * Imported the multi-temporal global land cover raster from the ArcGIS Living Atlas.
   * Applied **Definition Queries** to isolate the specific land cover data for the years 1992 and 2020.

2. **Area Calculation:**
   * Utilized the attribute table to calculate the exact area in square kilometers for each land cover classification. 
   * Given the spatial resolution of the raster (300m x 300m pixel size), I created a new field `Area_SqKM` and applied a Python field calculation: `(!Count! * 90000) * 0.000001`.

3. **Change Detection Analysis:**
   * Deployed the **Compute Change Raster** tool (Image Analyst) using the *Categorical Difference* method.
   * This generated a new raster highlighting only the modified pixels, pinpointing the exact locations and classifications where "Closed to Open Canopy Broadleaved" (Forest) transitioned primarily into "Rainfed/Herbaceous Cropland" and urban areas.

---

## 💡 Key Takeaways
This analysis demonstrates that Spatial Data is more than just points and polygons on a map—it is a powerful radar for reading geopolitics and environmental dynamics. By standardizing and calculating raster data, we provide solid, quantitative foundations to analyze our planet's most critical challenges.

> *This project was developed as a practical exercise within the "GIS for Climate Action" MOOC by Esri.*
