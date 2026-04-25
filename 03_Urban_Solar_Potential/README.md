*Read this in other languages: [🇮🇹 Italiano](#-italiano) | [🇬🇧 English](#-english)*

> ⚠️ **Nota sul Video / Video Note:** > *I video allegati a questo progetto sono stati accelerati (2x) per questioni di formato. Se desideri seguire i passaggi nel dettaglio, ti consiglio di scaricare il file .mp4 e riprodurlo tramite un media player locale impostando la velocità a 0.5x.*

---

# 🇮🇹 Italiano

# ☀️ Modellazione del Potenziale Solare Urbano

![ArcGIS Pro](https://img.shields.io/badge/ArcGIS_Pro-3.x-blue?style=for-the-badge&logo=esri)
![Spatial Analyst](https://img.shields.io/badge/Spatial_Analyst-Extension-108A44?style=for-the-badge)
![Green Energy](https://img.shields.io/badge/Green_Energy-Modeling-FFC107?style=for-the-badge)

## 📌 Panoramica del Progetto
La generazione di elettricità è responsabile di circa il 25% delle emissioni globali. Per questo, mappare il potenziale dei tetti delle nostre città per trasformarli in "centrali solari" non è più solo una visione, ma una necessità tecnica supportata dai dati.

In questo progetto ho mappato con estrema accuratezza il potenziale energetico solare degli edifici urbani. Non mi sono limitato a calcolare la semplice esposizione, ma ho modellato l'irraggiamento nell'arco di un intero anno, determinando le potenziali radiazioni solari in $kWh/m^2$ per ogni superficie e fornendo una base quantitativa solida per valutare la fattibilità di impianti fotovoltaici.

### 🎥 Dimostrazione: Analisi Temporale dell'Irraggiamento
*(Trascina e rilascia qui il tuo file RadiazioneSolare.mp4)*

---

## 🛠️ Strumenti e Tecnologie
* **Software:** ArcGIS Pro
* **Estensioni:** Spatial Analyst
* **Set di Dati:** Modello Digitale di Superficie (DSM) ad alta risoluzione, Building Footprints (Vettoriale).

---

## 🔬 Workflow Tecnico

1. **Elaborazione del Modello di Superficie (DSM):**
   * L'analisi si è basata su un Modello Digitale di Superficie (DSM) ad alta risoluzione, essenziale per ottenere una rappresentazione 3D fedele dell'area urbana, includendo l'altezza reale degli edifici e la presenza di alberi.

2. **Modellazione della Radiazione Solare (Raster Solar Radiation):**
   * Utilizzando l'estensione **Spatial Analyst** (set di strumenti *Radiazione Solare*), ho eseguito l'algoritmo calcolando l'insolazione per l'intero anno.
   * Il modello ha incrociato variabili cruciali come la pendenza dei tetti, l'orientamento e, soprattutto, l'ombreggiamento proiettato dinamicamente dagli edifici vicini o dalla vegetazione nelle diverse stagioni.
   * L'analisi è stata vincolata ("mascherata") esclusivamente alle impronte degli edifici (Building Footprints) per concentrare la potenza di calcolo solo sulle superfici utili (i tetti).

3. **Analisi Temporale (Temporal Profile):**
   * Come visibile nel video, ho sfruttato il **Cursore Temporale** per visualizzare la variazione dinamica della radiazione solare nei vari mesi.
   * Generando un grafico del **Profilo Temporale**, ho potuto estrarre i valori quantitativi specifici per le singole porzioni di tetto, distinguendo in modo netto le superfici ad alto rendimento dalle aree penalizzate dalle ombre.

---

## 💡 Conclusioni Principali
È evidente che i nostri tetti urbani potrebbero essere ottimizzati molto meglio e predisposti al fotovoltaico in modo sistematico. L'analisi spaziale dimostra che la tecnologia per farlo esiste già ed è straordinariamente potente, trasformando le superfici inutilizzate in asset strategici per la transizione energetica.

> *Questo progetto è stato sviluppato come esercitazione pratica all'interno del MOOC "GIS for Climate Action" di Esri.*

<br><br>

---

# 🇬🇧 English

# ☀️ Urban Solar Potential Modeling

## 📌 Project Overview
Electricity generation is responsible for approximately 25% of global emissions. Therefore, mapping the potential of our city rooftops to transform them into "solar power plants" is no longer just a vision, but a technical necessity supported by data.

In this project, I accurately mapped the solar energy potential of urban buildings. I didn't just calculate simple exposure; I modeled the irradiation over an entire year, determining the potential solar radiation in $kWh/m^2$ for each surface. This provides a solid quantitative basis for evaluating the feasibility of photovoltaic installations.

### 🎥 Demonstration: Temporal Analysis of Solar Irradiation
*(Drag and drop your RadiazioneSolare.mp4 file here)*

---

## 🛠️ Tools & Technologies
* **Software:** ArcGIS Pro
* **Extensions:** Spatial Analyst
* **Datasets:** High-resolution Digital Surface Model (DSM), Building Footprints (Vector).

---

## 🔬 Technical Workflow

1. **Digital Surface Model (DSM) Processing:**
   * The analysis relied on a high-resolution Digital Surface Model (DSM), which is essential for obtaining an accurate 3D representation of the urban area, including the true height of buildings and tree canopies.

2. **Solar Radiation Modeling (Raster Solar Radiation):**
   * Using the **Spatial Analyst** extension (*Solar Radiation* toolset), I executed the algorithm to calculate insolation over a full calendar year.
   * The model cross-referenced crucial variables such as roof slope, orientation, and, most importantly, the dynamic shading cast by neighboring buildings or vegetation across different seasons.
   * The analysis was constrained (using an Analysis Mask) specifically to the Building Footprints to focus the computational power solely on usable surfaces (the rooftops).

3. **Temporal Analysis (Temporal Profile):**
   * As shown in the video, I utilized the **Time Slider** to visualize the dynamic variation of solar radiation across different months.
   * By generating a **Temporal Profile** chart, I was able to extract specific quantitative values for individual roof sections, clearly distinguishing high-yield surfaces from areas penalized by shadows.

---

## 💡 Key Takeaways
It is clear that our urban rooftops could be much better optimized and systematically prepared for photovoltaics. Spatial analysis proves that the technology to do this already exists and is extraordinarily powerful, turning unused surfaces into strategic assets for the energy transition.

> *This project was developed as a practical exercise within the "GIS for Climate Action" MOOC by Esri.*
