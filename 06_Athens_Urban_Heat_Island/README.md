*Read this in other languages: [🇮🇹 Italiano](#-italiano) | [🇬🇧 English](#-english)*

> ⚠️ **Nota sui Video / Video Note:** > *I video allegati a questo progetto sono stati accelerati (2x) per questioni di formato. Se desideri seguire i passaggi tecnici nel dettaglio, ti consiglio di scaricare i file .mp4 e riprodurli tramite un media player locale impostando la velocità a 0.5x.*

---

# 🇮🇹 Italiano

# 🌡️ Indice di Rischio: Mappare le Isole di Calore Urbano ad Atene

![ArcGIS Pro](https://img.shields.io/badge/ArcGIS_Pro-3.x-blue?style=for-the-badge&logo=esri)
![Satellite](https://img.shields.io/badge/Satellite_Imagery-Landsat-005288?style=for-the-badge)
![GeoEnrichment](https://img.shields.io/badge/Demographics-GeoEnrichment-108A44?style=for-the-badge)

## 📌 Panoramica del Progetto
*Cemento che scotta, quartieri che respirano. L'impatto invisibile (ma misurabile) delle isole di calore urbano.*

Questo progetto rappresenta un'analisi di modellazione spaziale avanzata condotta per calcolare l'**Indice di Rischio di Calore (HRI)** relativo ai codici postali della città di Atene. Come si arriva a definire questo indice? Non basta misurare i gradi centigradi. Un vero Indice di Rischio nasce incrociando i fattori fisici del territorio con la vulnerabilità umana.

Il contrasto visivo finale è netto:
* 🟡/🟠 **Giallo/Arancio (Basso Rischio):** Aree di respiro. I quartieri con questo HRI combaciano perfettamente con le zone verdi, dove la presenza della copertura arborea abbatte le temperature.
* 🔴 **Rosso Scuro (Rischio Critico):** Le "gabbie termiche". I picchi massimi di rischio si sovrappongono inequivocabilmente alle aree grigie (built-up), dominate da asfalto, forte cementificazione e alta densità abitativa.

### 🎥 Dimostrazione: Modellazione Spaziale e Strumento Swipe
*(Trascina e rilascia qui il file HRI_Athens_FullVideo.mp4)*

---

## 🛠️ Strumenti e Tecnologie
* **Software:** ArcGIS Pro
* **Estensioni/Strumenti:** GeoEnrichment, Raster Calculator
* **Dati:** Immagini satellitari Multispectral Landsat, ESA WorldCover 2021, Dati Demografici (Esri Demographics).

---

## 🔬 Workflow Tecnico: I 4 Pilastri dell'Indice

1. **Il Pericolo (Analisi Fisica):** * Ho elaborato le immagini satellitari Multispectral Landsat per calcolare la Temperatura Superficiale Terrestre (Land Surface Temperature - LST) media per ogni quartiere. 
   * I dati sono stati filtrati per isolare le acquisizioni dei soli mesi estivi ed escludere le interferenze nuvolose, mappando così i veri picchi di calore.

2. **La Mitigazione (Analisi Ambientale):** * Utilizzando il layer vettoriale ESA WorldCover 2021, ho isolato la copertura arborea (Tree Canopy). Gli alberi non sono mero decoro, ma l'unica vera infrastruttura naturale per contrastare l'isola di calore.

3. **L'Esposizione (Analisi Demografica):** * Qui il dato spaziale si fa umano. Tramite lo strumento **GeoEnrichment**, ho calcolato la densità di popolazione per ogni singola area (codice postale).

4. **La Vulnerabilità (Il Fattore Chiave):** * Come step finale, ho arricchito il modello integrando i dati demografici specifici sulla popolazione **Over 60**. 
   * *Perché?* Il caldo estremo non colpisce tutti allo stesso modo. Un quartiere rovente ma privo di residenti ha un rischio diverso da un'area densamente popolata e con un'alta concentrazione di anziani. Standardizzando e combinando matematicamente tutte queste variabili, si ottiene la mappa di rischio finale.

---

## 💡 Conclusioni Principali
L'analisi spaziale va ben oltre la semplice rappresentazione cartografica: fornisce agli addetti ai lavori la base di dati quantitativa necessaria per prevenire le crisi. Un modello del genere indica ai decisori politici esattamente dove piantare nuovi alberi, dove progettare infrastrutture verdi e, soprattutto, dove indirizzare l'assistenza socio-sanitaria prima che la prossima ondata di calore colpisca.

> *Questo progetto è stato sviluppato come esercitazione pratica all'interno del MOOC "GIS for Climate Action" di Esri.*

<br><br>

---

# 🇬🇧 English

# 🌡️ Risk Index: Mapping Urban Heat Islands in Athens

## 📌 Project Overview
*Scorching concrete, breathing neighborhoods. The invisible (yet measurable) impact of urban heat islands.*

This project showcases advanced spatial modeling conducted to calculate the **Heat Risk Index (HRI)** across the postal codes of Athens, Greece. How is this index defined? It is not enough to simply measure the temperature. A true Risk Index is created by intersecting physical environmental factors with human vulnerability.

The final visual contrast is striking:
* 🟡/🟠 **Yellow/Orange (Low Risk):** Breathing areas. Neighborhoods with this HRI perfectly match the green zones, where tree canopy cover significantly lowers temperatures.
* 🔴 **Dark Red (Critical Risk):** "Thermal cages". The highest risk peaks unequivocally overlap with grey (built-up) areas, dominated by asphalt, heavy cementification, and high population density.

### 🎥 Demonstration: Spatial Modeling and Swipe Tool
*(Drag and drop your HRI_Athens_FullVideo.mp4 file here)*

---

## 🛠️ Tools & Technologies
* **Software:** ArcGIS Pro
* **Extensions/Tools:** GeoEnrichment, Raster Calculator
* **Data:** Multispectral Landsat satellite imagery, ESA WorldCover 2021, Demographic Data (Esri Demographics).

---

## 🔬 Technical Workflow: The 4 Pillars of the Index

1. **The Hazard (Physical Analysis):** * I processed Multispectral Landsat satellite imagery to calculate the mean Land Surface Temperature (LST) for each neighborhood.
   * The data was filtered to isolate acquisitions from summer months only and to exclude cloud interference, thereby mapping the true heat peaks.

2. **The Mitigation (Environmental Analysis):** * Using the ESA WorldCover 2021 vector layer, I isolated the Tree Canopy. Trees are not just decorative; they are the only true natural infrastructure capable of counteracting the urban heat island effect.

3. **The Exposure (Demographic Analysis):** * Here, spatial data becomes human. Using the **GeoEnrichment** tool, I calculated the population density for each specific area (postal code).

4. **The Vulnerability (The Key Factor):** * As a final step, I enriched the model by integrating specific demographic data regarding the **Over 60** population.
   * *Why?* Extreme heat does not affect everyone equally. A scorching neighborhood with no residents has a fundamentally different risk level than a densely populated area with a high concentration of elderly people. By mathematically standardizing and combining all these variables, the final risk map is generated.

---

## 💡 Key Takeaways
Spatial analysis goes far beyond simple cartographic representation: it provides professionals with the quantitative data foundation necessary to prevent crises. A model like this tells policymakers exactly where to plant new trees, where to design green infrastructure, and, most importantly, where to direct social and healthcare assistance before the next heatwave strikes.

> *This project was developed as a practical exercise within the "GIS for Climate Action" MOOC by Esri.*
```E con questo abbiamo chiuso in bellezza! Questo ultimo progetto sulle Isole di Calore è fantastico perché unisce i dati fisici (satellitari) a quelli demografici, mostrando una maturità di analisi che va molto oltre il semplice "creare una mappa". L'idea della vulnerabilità umana (gli over 60) rende il progetto non solo tecnico, ma utile e reale.

Ho strutturato il README per la cartella `06_Athens_Urban_Heat_Island` rispettando fedelmente il tuo post su LinkedIn e la solita struttura bilingue e professionale.

Ecco il codice Markdown definitivo:

```markdown
*Read this in other languages: [🇮🇹 Italiano](#-italiano) | [🇬🇧 English](#-english)*

> ⚠️ **Nota sui Video / Video Note:** > *I video allegati a questo progetto sono stati accelerati (2x) per questioni di formato. Se desideri seguire i passaggi tecnici nel dettaglio, ti consiglio di scaricare i file .mp4 e riprodurli tramite un media player locale impostando la velocità a 0.5x.*

---

# 🇮🇹 Italiano

# 🌡️ Indice di Rischio: Mappare le Isole di Calore Urbano ad Atene

![ArcGIS Pro](https://img.shields.io/badge/ArcGIS_Pro-3.x-blue?style=for-the-badge&logo=esri)
![Satellite](https://img.shields.io/badge/Satellite_Imagery-Landsat-005288?style=for-the-badge)
![GeoEnrichment](https://img.shields.io/badge/Demographics-GeoEnrichment-108A44?style=for-the-badge)

## 📌 Panoramica del Progetto
*Cemento che scotta, quartieri che respirano. L'impatto invisibile (ma misurabile) delle isole di calore urbano.*

Questo progetto rappresenta un'analisi di modellazione spaziale avanzata condotta per calcolare l'**Indice di Rischio di Calore (HRI)** relativo ai codici postali della città di Atene. Come si arriva a definire questo indice? Non basta misurare i gradi centigradi. Un vero Indice di Rischio nasce incrociando i fattori fisici del territorio con la vulnerabilità umana.

Il contrasto visivo finale è netto:
* 🟡/🟠 **Giallo/Arancio (Basso Rischio):** Aree di respiro. I quartieri con questo HRI combaciano perfettamente con le zone verdi, dove la presenza della copertura arborea abbatte le temperature.
* 🔴 **Rosso Scuro (Rischio Critico):** Le "gabbie termiche". I picchi massimi di rischio si sovrappongono inequivocabilmente alle aree grigie (built-up), dominate da asfalto, forte cementificazione e alta densità abitativa.

### 🎥 Dimostrazione: Modellazione Spaziale e Strumento Swipe
*(Trascina e rilascia qui il file HRI_Athens_FullVideo.mp4)*

---

## 🛠️ Strumenti e Tecnologie
* **Software:** ArcGIS Pro
* **Estensioni/Strumenti:** GeoEnrichment, Raster Calculator
* **Dati:** Immagini satellitari Multispectral Landsat, ESA WorldCover 2021, Dati Demografici (Esri Demographics).

---

## 🔬 Workflow Tecnico: I 4 Pilastri dell'Indice

1. **Il Pericolo (Analisi Fisica):** * Ho elaborato le immagini satellitari Multispectral Landsat per calcolare la Temperatura Superficiale Terrestre (Land Surface Temperature - LST) media per ogni quartiere. 
   * I dati sono stati filtrati per isolare le acquisizioni dei soli mesi estivi ed escludere le interferenze nuvolose, mappando così i veri picchi di calore.

2. **La Mitigazione (Analisi Ambientale):** * Utilizzando il layer vettoriale ESA WorldCover 2021, ho isolato la copertura arborea (Tree Canopy). Gli alberi non sono mero decoro, ma l'unica vera infrastruttura naturale per contrastare l'isola di calore.

3. **L'Esposizione (Analisi Demografica):** * Qui il dato spaziale si fa umano. Tramite lo strumento **GeoEnrichment**, ho calcolato la densità di popolazione per ogni singola area (codice postale).

4. **La Vulnerabilità (Il Fattore Chiave):** * Come step finale, ho arricchito il modello integrando i dati demografici specifici sulla popolazione **Over 60**. 
   * *Perché?* Il caldo estremo non colpisce tutti allo stesso modo. Un quartiere rovente ma privo di residenti ha un rischio diverso da un'area densamente popolata e con un'alta concentrazione di anziani. Standardizzando e combinando matematicamente tutte queste variabili, si ottiene la mappa di rischio finale.

---

## 💡 Conclusioni Principali
L'analisi spaziale va ben oltre la semplice rappresentazione cartografica: fornisce agli addetti ai lavori la base di dati quantitativa necessaria per prevenire le crisi. Un modello del genere indica ai decisori politici esattamente dove piantare nuovi alberi, dove progettare infrastrutture verdi e, soprattutto, dove indirizzare l'assistenza socio-sanitaria prima che la prossima ondata di calore colpisca.

> *Questo progetto è stato sviluppato come esercitazione pratica all'interno del MOOC "GIS for Climate Action" di Esri.*

<br><br>

---

# 🇬🇧 English

# 🌡️ Risk Index: Mapping Urban Heat Islands in Athens

## 📌 Project Overview
*Scorching concrete, breathing neighborhoods. The invisible (yet measurable) impact of urban heat islands.*

This project showcases advanced spatial modeling conducted to calculate the **Heat Risk Index (HRI)** across the postal codes of Athens, Greece. How is this index defined? It is not enough to simply measure the temperature. A true Risk Index is created by intersecting physical environmental factors with human vulnerability.

The final visual contrast is striking:
* 🟡/🟠 **Yellow/Orange (Low Risk):** Breathing areas. Neighborhoods with this HRI perfectly match the green zones, where tree canopy cover significantly lowers temperatures.
* 🔴 **Dark Red (Critical Risk):** "Thermal cages". The highest risk peaks unequivocally overlap with grey (built-up) areas, dominated by asphalt, heavy cementification, and high population density.

### 🎥 Demonstration: Spatial Modeling and Swipe Tool
*(Drag and drop your HRI_Athens_FullVideo.mp4 file here)*

---

## 🛠️ Tools & Technologies
* **Software:** ArcGIS Pro
* **Extensions/Tools:** GeoEnrichment, Raster Calculator
* **Data:** Multispectral Landsat satellite imagery, ESA WorldCover 2021, Demographic Data (Esri Demographics).

---

## 🔬 Technical Workflow: The 4 Pillars of the Index

1. **The Hazard (Physical Analysis):** * I processed Multispectral Landsat satellite imagery to calculate the mean Land Surface Temperature (LST) for each neighborhood.
   * The data was filtered to isolate acquisitions from summer months only and to exclude cloud interference, thereby mapping the true heat peaks.

2. **The Mitigation (Environmental Analysis):** * Using the ESA WorldCover 2021 vector layer, I isolated the Tree Canopy. Trees are not just decorative; they are the only true natural infrastructure capable of counteracting the urban heat island effect.

3. **The Exposure (Demographic Analysis):** * Here, spatial data becomes human. Using the **GeoEnrichment** tool, I calculated the population density for each specific area (postal code).

4. **The Vulnerability (The Key Factor):** * As a final step, I enriched the model by integrating specific demographic data regarding the **Over 60** population.
   * *Why?* Extreme heat does not affect everyone equally. A scorching neighborhood with no residents has a fundamentally different risk level than a densely populated area with a high concentration of elderly people. By mathematically standardizing and combining all these variables, the final risk map is generated.

---

## 💡 Key Takeaways
Spatial analysis goes far beyond simple cartographic representation: it provides professionals with the quantitative data foundation necessary to prevent crises. A model like this tells policymakers exactly where to plant new trees, where to design green infrastructure, and, most importantly, where to direct social and healthcare assistance before the next heatwave strikes.

> *This project was developed as a practical exercise within the "GIS for Climate Action" MOOC by Esri.*
