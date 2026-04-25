*Read this in other languages: [🇮🇹 Italiano](#-italiano) | [🇬🇧 English](#-english)*

> ⚠️ **Nota sul Video / Video Note:** > *I video allegati a questo progetto sono stati accelerati (2x) per questioni di formato. Se desideri seguire i passaggi nel dettaglio, ti consiglio di scaricare il file .mp4 e riprodurlo tramite un media player locale impostando la velocità a 0.5x.*
---

# 🇮🇹 Italiano

# 🚛 Ottimizzazione della Logistica Sostenibile (Last Mile Delivery)

![ArcGIS Pro](https://img.shields.io/badge/ArcGIS_Pro-3.x-blue?style=for-the-badge&logo=esri)
![Network Analyst](https://img.shields.io/badge/Network_Analyst-Extension-108A44?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-Scripting-3776AB?style=for-the-badge&logo=python&logoColor=white)

## 📌 Panoramica del Progetto
La lotta al cambiamento climatico inizia anche da un’attenta analisi dei percorsi e... da un'attenta analisi costi-benefici dei nostri crediti cloud! 💸🌍

Un’ottimizzazione intelligente dei percorsi può abbattere le emissioni di gas serra dei veicoli per le consegne fino al 30%. Per questo esercizio pratico, ho simulato una flotta aziendale impegnata nelle consegne dell'ultimo miglio (Last Mile Delivery), puntando alla massima efficienza logistica e alla minimizzazione dell'impronta di carbonio.

### 🎥 Dimostrazione del Ricalcolo dell'Itinerario
*(Trascina e rilascia qui il tuo file PercorsiOttimizzati.mp4)*

---

## 🛠️ Strumenti e Tecnologie
* **Software:** ArcGIS Pro, ArcGIS Online (Cloud Servers)
* **Estensioni:** Network Analyst
* **Linguaggi:** Python (Field Calculator)

---

## 🔬 Workflow Tecnico

1. **Geocodifica degli Indirizzi:**
   * Importazione del file grezzo `ProduceCustomers.csv`.
   * Conversione degli indirizzi testuali dei clienti in punti precisi sulla mappa, passaggio fondamentale per posizionare le fermate ("stops") dell'analisi.

2. **Configurazione dell'Infrastruttura di Rete:**
   * Impostazione dell'indirizzo della sede centrale come "Centro Operativo" (Depot). Questo nodo funge da punto di partenza e arrivo, coordinando l'intera flotta.
   * Utilizzo dell'ambiente **Python in ArcGIS Pro** per creare un campo calcolato nella tabella attributi degli ordini, inserendo uno script per regolare dinamicamente i tempi di scarico in base al volume/numero dei pacchi da consegnare.

3. **Risoluzione del Percorso (Last Mile Delivery):**
   * Configurazione del risolutore specifico per il "Last Mile Delivery" tramite **ArcGIS Network Analyst** per gestire i vincoli di flotte complesse (capacità dei veicoli, finestre temporali di consegna, numero massimo di fermate).
   * Esecuzione dell'algoritmo basato su cloud (utilizzando i crediti organizzativi Esri), che ha elaborato migliaia di variabili per individuare i percorsi ottimali, minimizzando i chilometri percorsi e le emissioni di CO2.

---

## 💡 Conclusioni Principali
Questo progetto evidenzia come i GIS non servano solo a visualizzare dati, ma siano strumenti operativi essenziali per le aziende. Ottimizzare una flotta tramite l'analisi di rete non significa solo risparmiare carburante e tempo, ma rappresenta una strategia concreta e misurabile per ridurre l'impatto ambientale della logistica aziendale.

> *Questo progetto è stato sviluppato come esercitazione pratica all'interno del MOOC "GIS for Climate Action" di Esri.*

<br><br>

---

# 🇬🇧 English

# 🚛 Sustainable Logistics Optimization (Last Mile Delivery)

## 📌 Project Overview
The fight against climate change also begins with careful route analysis and... a careful cost-benefit analysis of our cloud credits! 💸🌍

Intelligent route optimization can cut greenhouse gas emissions from delivery vehicles by up to 30%. For this practical exercise, I simulated a corporate fleet engaged in last-mile deliveries, aiming for maximum logistical efficiency and carbon footprint minimization.

### 🎥 Route Recalculation Demonstration
*(Drag and drop your PercorsiOttimizzati.mp4 file here)*

---

## 🛠️ Tools & Technologies
* **Software:** ArcGIS Pro, ArcGIS Online (Cloud Servers)
* **Extensions:** Network Analyst
* **Languages:** Python (Field Calculator)

---

## 🔬 Technical Workflow

1. **Address Geocoding:**
   * Imported the raw `ProduceCustomers.csv` file.
   * Converted textual customer addresses into precise points on the map, a crucial step to position the delivery "stops" for the analysis.

2. **Network Infrastructure Setup:**
   * Configured the headquarters address as the "Depot". This node acts as the starting and ending point, coordinating the entire fleet.
   * Leveraged the **Python environment within ArcGIS Pro** to create a calculated field in the orders attribute table, using a script to dynamically adjust unloading times based on the volume/number of packages to be delivered.

3. **Route Solving (Last Mile Delivery):**
   * Configured the specific "Last Mile Delivery" solver via **ArcGIS Network Analyst** to manage the constraints of complex fleets (vehicle capacity, delivery time windows, maximum number of stops).
   * Executed the cloud-based algorithm (utilizing Esri organizational credits), which processed thousands of variables to find the optimal paths, minimizing driven kilometers and CO2 emissions.

---

## 💡 Key Takeaways
This project highlights how GIS is not just for visualizing data, but is an essential operational tool for businesses. Optimizing a fleet through network analysis means more than just saving fuel and time; it represents a concrete, measurable strategy to reduce the environmental impact of corporate logistics.

> *This project was developed as a practical exercise within the "GIS for Climate Action" MOOC by Esri.*
