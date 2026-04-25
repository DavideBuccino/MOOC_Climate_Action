*Read this in other languages: [🇮🇹 Italiano](#-italiano) | [🇬🇧 English](#-english)*

> ⚠️ **Nota sui Video / Video Note:** > *I video allegati a questo progetto sono stati accelerati (2x) per questioni di formato. Se desideri seguire i passaggi tecnici nel dettaglio, ti consiglio di scaricare i file .mp4 e riprodurli tramite un media player locale impostando la velocità a 0.5x.*

---

# 🇮🇹 Italiano

# 🌊 Digital Twin 3D e Analisi dell'Innalzamento del Livello del Mare a Miami Beach

![ArcGIS Pro](https://img.shields.io/badge/ArcGIS_Pro-3.x-blue?style=for-the-badge&logo=esri)
![3D Analyst](https://img.shields.io/badge/3D_Analyst-Extension-108A44?style=for-the-badge)
![Web Scene](https://img.shields.io/badge/ArcGIS_Online-3D_Web_Scene-orange?style=for-the-badge)

## 📌 Panoramica del Progetto
Questo progetto end-to-end si divide in due fasi fondamentali: alzare "letteralmente" il livello dei dati per costruire un ambiente 3D e, successivamente, interrogare questo modello per simulare futuri scenari di rischio climatico.

L'obiettivo è modellare e misurare l'impatto reale dell'innalzamento del livello del mare sulla costa di Miami Beach per gli anni 2030, 2050 e 2090, basandosi sugli scenari climatici previsionali del NOAA (National Oceanic and Atmospheric Administration).

🌐 **Esplora il risultato finale:** 👉 **[Web Scene Interattiva di Miami Beach](https://arcg.is/1qyv0r0)**

---

## 🛠️ Strumenti e Tecnologie
* **Software:** ArcGIS Pro, ArcGIS Online
* **Estensioni:** 3D Analyst
* **Dati:** Impronte Edifici (Vettoriali), Dati Raster NOAA (tramite ArcGIS Living Atlas), Rule Packages (.rpk), Layer Multipatch.

---

## 🔬 Parte 1: Costruzione del "Digital Twin" 3D

Prima di passare all'analisi, ho dedicato la prima fase alla transizione da una semplice mappa 2D a un "Gemello Digitale" 3D realistico della città.

### 🎥 Setup dell'Ambiente 3D
*(Trascina e rilascia qui il file Video Miami Lezione 3 - prima parte.mp4)*

### Workflow di Modellazione:
1. **Estrusione dei Volumi:** Tramite lo strumento **Join Field**, ho unito la tabella contenente i valori esatti dell'altezza dei palazzi al layer spaziale 2D, estrudendo i poligoni in base alle loro altezze assolute reali.
2. **Realismo Architettonico:** Ho perfezionato il modello importando un **layer multipatch** per ricreare le inclinazioni esatte dei tetti. Successivamente, ho applicato un **Rule Package (.rpk)** per generare in modo procedurale le texture fotorealistiche delle facciate (es. le vetrate dei grattacieli).
3. **Ambiente e Illuminazione:** Ho curato l'ambiente circostante applicando una simbologia procedurale "Acque Tropicali" al mare (regolando direzione e moto ondoso). Ho impostato il fuso orario locale (UTC -5:00) per simulare dinamicamente i riflessi della luce e le ombre nelle diverse ore del giorno tramite il **Cursore Temporale**.

---

## 🔬 Parte 2: Analisi del Rischio di Allagamento (2030-2090)

Un modello 3D esprime il suo vero potenziale solo quando viene interrogato spazialmente. In questa fase ho valutato l'impatto delle acque basandomi sullo scenario intermedio-alto del NOAA.

### 🎥 Analisi Spaziale e Valutazione del Rischio
*(Trascina e rilascia qui il file Video Miami Lezione 3 - seconda parte.mp4)*

### Workflow di Analisi:
1. **Preparazione Dati Scenari:** Ho estratto dall'ArcGIS Living Atlas i layer raster previsionali per il 2030, 2050 e 2090. Tramite un'elaborazione in **Batch (Raster to Polygon)**, li ho convertiti in poligoni per renderli compatibili con le geometrie degli edifici.
2. **Intersezione Spaziale:** Utilizzando lo strumento **Seleziona per Posizione (Select by Location)**, ho individuato esattamente quali edifici intersecheranno le aree allagate nei diversi scenari.
3. **Arricchimento Dati:** Sfruttando lo strumento **Calcola Campo (Calculate Field)**, ho registrato nella tabella attributi l'anno stimato di inondazione per ogni singolo edificio.
4. **Simbologia e Validazione:** Ho classificato gli edifici con una scala cromatica (Verde = Sicuro, Giallo/Rosso = A rischio). Utilizzando lo strumento **Profilo di Elevazione**, ho tracciato sezioni trasversali della città per validare il modello, confermando che i palazzi "verdi" poggiano su quote altimetriche che li mettono al riparo dalle acque.

## 💡 Conclusioni Principali
Il vero valore di un'analisi spaziale complessa risiede nella sua accessibilità. Pubblicando la **Web Scene** su ArcGIS Online, i risultati non rimangono confinati nel software desktop, ma diventano uno strumento di comunicazione e pianificazione potente per decisori politici e cittadini che possono navigare il modello direttamente dal browser.

> *Questo progetto è stato sviluppato come esercitazione pratica all'interno del MOOC "GIS for Climate Action" di Esri.*

<br><br>

---

# 🇬🇧 English

# 🌊 3D Digital Twin and Sea Level Rise Analysis in Miami Beach

## 📌 Project Overview
This end-to-end project is divided into two crucial phases: "literally" raising the level of the data to build a 3D environment, and subsequently interrogating this model to simulate future climate risk scenarios.

The goal is to model and measure the real impact of sea level rise on the coast of Miami Beach for the years 2030, 2050, and 2090, based on NOAA (National Oceanic and Atmospheric Administration) climate forecast scenarios.

🌐 **Explore the final result:** 👉 **[Interactive Miami Beach Web Scene](https://arcg.is/1qyv0r0)**

---

## 🛠️ Tools & Technologies
* **Software:** ArcGIS Pro, ArcGIS Online
* **Extensions:** 3D Analyst
* **Data:** Building Footprints (Vector), NOAA Raster Data (via ArcGIS Living Atlas), Rule Packages (.rpk), Multipatch Layers.

---

## 🔬 Part 1: Building the 3D "Digital Twin"

Before moving on to the analysis, the first phase was dedicated to the transition from a simple 2D map to a realistic 3D "Digital Twin" of the city.

### 🎥 3D Environment Setup
*(Drag and drop your Video Miami Lezione 3 - prima parte.mp4 file here)*

### Modeling Workflow:
1. **Volume Extrusion:** Using the **Join Field** tool, I joined a table containing the exact height values of the buildings to the 2D spatial layer, extruding the polygons based on their true absolute heights.
2. **Architectural Realism:** I refined the model by importing a **multipatch layer** to recreate exact roof pitches. Next, I applied a **Rule Package (.rpk)** to procedurally generate photorealistic textures for the facades (e.g., skyscraper glass).
3. **Environment & Lighting:** I enhanced the surrounding environment by applying a procedural "Tropical Water" symbology to the sea (adjusting wave direction and motion). I set the local time zone (UTC -5:00) to dynamically simulate light reflections and shadows at different times of the day using the **Time Slider**.

---

## 🔬 Part 2: Flood Risk Analysis (2030-2090)

A 3D model reveals its true potential only when it is spatially interrogated. In this phase, I evaluated the water impact based on the NOAA intermediate-high scenario.

### 🎥 Spatial Analysis and Risk Assessment
*(Drag and drop your Video Miami Lezione 3 - seconda parte.mp4 file here)*

### Analysis Workflow:
1. **Scenario Data Prep:** I extracted the forecast raster layers for 2030, 2050, and 2090 from the ArcGIS Living Atlas. Using a **Batch processing (Raster to Polygon)** tool, I converted them into polygons to make them compatible with the building geometries.
2. **Spatial Intersection:** Using the **Select by Location** tool, I pinpointed exactly which buildings will intersect the flooded areas across the different scenarios.
3. **Data Enrichment:** Leveraging the **Calculate Field** tool, I recorded the estimated inundation year for each individual building within the attribute table.
4. **Symbology & Validation:** I classified the buildings using a color scale (Green = Safe, Yellow/Red = At Risk). Using the **Elevation Profile** tool, I drew cross-sections of the city to validate the model, visually confirming that the "green" buildings sit at slightly higher elevations, keeping them safe from rising waters.

## 💡 Key Takeaways
The true value of complex spatial analysis lies in its accessibility. By publishing the **Web Scene** to ArcGIS Online, the results are not confined to desktop software; they become a powerful communication and planning tool for policymakers and citizens alike, who can explore the model directly in their browser.

> *This project was developed as a practical exercise within the "GIS for Climate Action" MOOC by Esri.*
