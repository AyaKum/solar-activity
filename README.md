# Classifying Seismic Events Linked to Solar Activity: A Retrospective LSTM Approach Using Proton Density

This repository contains code and datasets used in the research project exploring the integration of **solar activity parameters** with **seismic data** for short-term earthquake forecasting.

📄 The methodology and results are published in:

> [*Classifying Seismic Events Linked to Solar Activity: A Retrospective LSTM Approach Using Proton Density*, *MDPI Athmosphere* (2024).](https://www.mdpi.com/3015642)

---

## 📂 Repository Structure

* **README.md** – Project description and usage instructions
* **declustered earthquake dataset.ipynb** – Notebook for preparing seismic dataset by declustering catalogs
* **soho dataset.ipynb** – Notebook for processing solar activity data from the SOHO satellite
* **sequence lstm 50 epoch.ipynb** – Main notebook with LSTM sequence model training and evaluation

---

## 🔍 Research Motivation

Earthquake prediction remains one of the grand challenges in geophysics. While seismic catalogs provide a historical record of events, they often lack predictive power when used alone. Solar activity (e.g., geomagnetic storms, solar wind parameters, and sunspot numbers) influences the Earth's ionosphere and may interact with seismogenic processes.

This project investigates whether deep learning can improve forecasting ability by combining:

* **Seismic data** (magnitude, time, depth, location)
* **Solar parameters** (SOHO satellite measurements of proton density)

---

## 🧠 Methods

* Data preprocessing:

  * Earthquake catalog declustering
  * Time-series alignment with solar datasets
* Model architecture:

  * LSTM-based neural network for temporal pattern recognition

---

## 📊 Results

* Details, figures, and discussion are available in the published article.

---

## 🚀 Getting Started

### Requirements

* Python 3.10+
* Jupyter Notebook
* Libraries:

  ```bash
  pip install numpy pandas matplotlib scikit-learn tensorflow keras
  ```

### Usage

1. Open notebooks in order:

   * `declustered earthquake dataset.ipynb`
   * `soho dataset.ipynb`
   * `sequence lstm 50 epoch.ipynb`
2. Run preprocessing and model training cells
3. Evaluate results

---

##  Citation

If you use this code or dataset, please cite:

```bibtex
@article{atmos15111290,
AUTHOR = {Altaibek, Aizhan and Nurtas, Marat and Zhantayev, Zhumabek and Zhumabayev, Beibit and Kumarkhanova, Ayazhan},
TITLE = {Classifying Seismic Events Linked to Solar Activity: A Retrospective LSTM Approach Using Proton Density},
JOURNAL = {Atmosphere},
VOLUME = {15},
YEAR = {2024},
NUMBER = {11},
ARTICLE-NUMBER = {1290},
URL = {https://www.mdpi.com/2073-4433/15/11/1290},
ISSN = {2073-4433},
ABSTRACT = {The influence of solar activity on seismic activity is a subject of debate. Previous studies have shown that there is sometimes a correlation and sometimes a contradiction between solar activity maxima and large earthquakes. Long-term memory neural network is used to study the relationship between solar activity and seismic activity. This study emphasizes retrospective classification rather than direct prediction, refining the LSTM architecture to maximize classification accuracy and processing data from the Solar and Heliospheric Observatory and the U.S. Geological Survey earthquake catalogs. A declustering technique is used to select large seismic events and weighted learning corrects for class imbalances. The LSTM model accurately classified earthquakes (84.47%) and proton density variations. The results support the theory that solar activity, in particular proton density, can anticipate earthquake events.},
DOI = {10.3390/atmos15111290}
}
```

---

## 📬 Contact

For questions or collaborations, please contact:
**Ayazhan Kumarkhanova** – [email:](kumarhanovaayazhan@gmail.com)
