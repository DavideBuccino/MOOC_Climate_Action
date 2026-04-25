*Read this in other languages: [🇮🇹 Italiano](#-italiano) | [🇬🇧 English](#-english)*

> ⚠️ **Nota sui Video / Video Note:** > *I video allegati a questo progetto sono stati accelerati (2x) per questioni di formato. Se desideri seguire i passaggi tecnici nel dettaglio, ti consiglio di scaricare i file .mp4 e riprodurli tramite un media player locale impostando la velocità a 0.5x.*

---

# 🇮🇹 Italiano

# 🌽 Machine Learning e Sicurezza Alimentare: Previsione dell'Idoneità Agricola in Africa

![ArcGIS Pro](https://img.shields.io/badge/ArcGIS_Pro-3.x-blue?style=for-the-badge&logo=esri)
![Spatial ML](https://img.shields.io/badge/Machine_Learning-Spatial_ML-FF6F00?style=for-the-badge)
![MaxEnt](https://img.shields.io/badge/Algorithm-MaxEnt-108A44?style=for-the-badge)

## 📌 Panoramica del Progetto
*"Questo piccolo errore ci è costato sette anni".* ⏳

Citando il film *Interstellar*, non avrò perso sette anni, ma il mio PC se l'è decisamente vista brutta! Durante la fase di campionamento spaziale per questo progetto, dovevo generare 100.000 punti casuali per addestrare l'algoritmo. Per un banale errore di battitura, ne ho creati **1.000.000**. Risultato? Ore di calcoli con il processore al 100%.

Questo imprevisto mi ha insegnato una grande lezione pratica sul Machine Learning spaziale: *decuplicare i dati in ingresso non decuplica necessariamente l'accuratezza, ma spesso rischia solo di saturare la capacità computazionale*. Una presa di consapevolezza fondamentale sull'ottimizzazione dei dati.

Al netto degli imprevisti, il cuore di questo progetto è vitale: **la modellazione predittiva per la sicurezza alimentare**. Il mais è la base alimentare per milioni di persone in Africa Subsahariana. Tramite strumenti di Spatial Machine Learning, ho mappato come lo stress termico e le precipitazioni altereranno le aree idonee alla coltivazione di questa coltura da qui ai prossimi 50 anni.

### 🎥 Dimostrazione: Addestramento e Previsione (MaxEnt)
*(Trascina e rilascia qui il file Progetto Africa - Full Video.mp4)*

---

## 🛠️ Strumenti e Tecnologie
* **Software:** ArcGIS Pro
* **Algoritmi ML:** Maximum Entropy (MaxEnt) tramite lo strumento *Presence-only Prediction*.
* **Dati:** Dati Raster Multidimensionali (proiezioni climatiche globali fino al 2090 estratte dall'ArcGIS Living Atlas), Dati di presenza storica delle colture.

---

## 🔬 Workflow Tecnico

1. **Preparazione dei Dati (Sampling):** * Estrazione delle variabili raster bioclimatiche (precipitazioni, stress termico) da set di dati multidimensionali.
   * Generazione di punti casuali di campionamento (il famoso milione!) utilizzati come "sonde" spaziali per incrociare i dati di presenza storica del mais con decine di parametri climatici sottostanti.

2. **Addestramento dell'Algoritmo (MaxEnt):** * Utilizzo dello strumento **Presence-only Prediction (Previsione basata solo sulla presenza)** per dare in pasto i dati di training al modello. 
   * L'algoritmo ha "imparato" in modo autonomo le relazioni complesse e non lineari tra le variabili ambientali fornite e l'habitat ideale della coltura.

3. **Previsione e Scenari Futuri:** * Applicazione del modello addestrato ai layer raster contenenti gli scenari climatici futuri (fino al 2090).
   * Generazione della mappa di output finale, interrogabile dinamicamente tramite lo strumento di scorrimento (**Swipe**).
      * 🟢 **Verde (Alta idoneità):** La "zona di comfort", temperature ottimali e stress idrico assente.
      * 🟡 **Giallo (Bassa idoneità):** Aree diventate ostili a causa dello stress termico o piogge insufficienti.

## 💡 Conclusioni Principali
Le conseguenze di questa "migrazione agricola" forzata dai cambiamenti climatici sarebbero devastanti. Pensate a territori dove l'acqua è già scarsa: se il clima sposterà l'area ideale del mais a centinaia di chilometri di distanza, interi sistemi di irrigazione, logistica e filiere andranno smantellati e ricostruiti altrove. 
L'analisi spaziale non serve solo a colorare poligoni, ma fornisce ai decisori politici gli strumenti predittivi necessari per prevenire crisi umanitarie.

> *Questo progetto è stato sviluppato come esercitazione pratica all'interno del MOOC "GIS for Climate Action" di Esri.*

<br><br>

---

# 🇬🇧 English

# 🌽 Machine Learning & Food Security: Predicting Crop Suitability in Africa

## 📌 Project Overview
*"This little maneuver's gonna cost us 51 years."* ⏳

Quoting *Interstellar*, I might not have lost decades, but my PC definitely had a rough time! During the spatial sampling phase of this project, I was supposed to generate 100,000 random points to train the algorithm. Due to a simple typo, I created **1,000,000**. The result? Hours of intense computation with my processor maxed out.

This unexpected event taught me a valuable practical lesson about Spatial Machine Learning: *multiplying input data tenfold doesn't necessarily multiply accuracy; it often just risks saturating computational capacity*. A fundamental realization about data optimization.

Anecdotes aside, the core of this project is vital: **predictive modeling for food security**. Maize is the staple food for millions of people in Sub-Saharan Africa. Using Spatial Machine Learning tools, I mapped how thermal stress and changing precipitation patterns will alter the areas suitable for this crop over the next 50 years.

### 🎥 Demonstration: Training and Prediction (MaxEnt)
*(Drag and drop your Progetto Africa - Full Video.mp4 file here)*

---

## 🛠️ Tools & Technologies
* **Software:** ArcGIS Pro
* **ML Algorithms:** Maximum Entropy (MaxEnt) via the *Presence-only Prediction* tool.
* **Data:** Multidimensional Raster Data (global climate projections up to 2090 extracted from ArcGIS Living Atlas), Historical crop presence data.

---

## 🔬 Technical Workflow

1. **Data Preparation (Sampling):** * Extraction of bioclimatic raster variables (precipitation, thermal stress) from multidimensional datasets.
   * Generation of random sampling points (the famous million!) used as spatial "probes" to cross-reference historical maize presence data with dozens of underlying climate parameters.

2. **Algorithm Training (MaxEnt):** * Utilized the **Presence-only Prediction** tool to feed the training data into the model. 
   * The algorithm autonomously "learned" the complex, non-linear relationships between the provided environmental variables and the crop's ideal habitat.

3. **Future Prediction Scenarios:** * Applied the trained model to raster layers containing future climate scenarios (up to 2090).
   * Generated the final output map, dynamically explorable using the **Swipe** tool.
      * 🟢 **Green (High Suitability):** The "comfort zone", optimal temperatures, and zero water stress.
      * 🟡 **Yellow (Low Suitability):** Areas turned hostile due to heat stress or insufficient rainfall.

## 💡 Key Takeaways
The consequences of this climate-driven "agricultural migration" would be devastating. Consider regions where water is already scarce: if the climate shifts the ideal maize-growing area hundreds of kilometers away, entire irrigation systems, logistics networks, and supply chains will need to be dismantled and rebuilt elsewhere. 
Spatial analysis is not just about coloring polygons; it provides policymakers with the predictive tools necessary to prevent humanitarian crises.

> *This project was developed as a practical exercise within the "GIS for Climate Action" MOOC by Esri.*
