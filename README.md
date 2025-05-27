# TCVD-PRACT2

> CODE OWNER: Alexandre Sánchez, Miguel Aloy

> disclaimer: Hem observat que el mapa coroplètic no renderitzava correctament dins del notebook al repositori, per això s'ha inclòs com a imatge separada

Repositori per a la pràctica 2 de **Tipologia i Cicle de Vida de les Dades** del *Màster Universitari en Ciència de Dades* de la **Universitat Oberta de Catalunya (UOC)**.

## :scroll: Dataset utilitzat

El conjunt de dades original es pot descarregar a través de:

https://www.kaggle.com/datasets/ravindrasinghrana/job-description-dataset?resource=download&select=job_descriptions.csv


## 🧠 Descripció

Aquest projecte té com a objectiu analitzar, transformar i aplicar tècniques d'aprenentatge automàtic (tant supervisat com no supervisat) i una prova d'hipòtesi sobre un conjunt de dades reals d'ofertes de treball. Les dades contenen informació detallada de les feines, com el títol, descripció, habilitats requerides, país, preferències, experiència, entre d’altres.

Els objectius inclouen:
- La neteja del conjunt de dades.
- L’anàlisi exploratòria de les variables disponibles.
- L’aplicació de models de regressió supervisats per predir el salari.
- L’experimentació amb tècniques no supervisades per fer agrupacions per tipus de feina.

El conjunt de dades es troba disponible a [Kaggle: Job Description Dataset](https://www.kaggle.com/datasets/ravindrasinghrana/job-description-dataset?resource=download&select=job_descriptions.csv).


## 📦 Contingut

Estructura de carpetes del projecte:

```
TCVD-PRACT2/
│
├── dataset/
│   ├── glassdoor_jobs_original.csv
│   ├── glassdoor_jobs_processed.csv
│   └── supervised-job_description_sample.csv
│
├── source/
│   ├── data_processing.ipynb              # Neteja, codificació i visualitzacions
│   ├── non-supervised_algorithm.ipynb     # Algorismes no supervisats (clustering, etc.)
│   └── supervised_algorithm.ipynb         # Models supervisats (regressió de salaris)
│
├── .gitignore
├── .gitattributes
├── LICENSE
├── README.md
└── mapa_coropletic_ofertes_per_pais.png
```


## 🔧 Requisits

### 📊 No supervisat:
- pandas
- re
- sklearn
- matplotlib
- seaborn
- rapidfuzz
- itertools

### 📈 Supervisat:
- polars
- pathlib
- plotly
- pandas
- matplotlib
- wordcloud
- sentence_transformers
- scikit-learn
- xgboost


## ⚙️ Execució

L’execució està estructurada dins de cada notebook. A cada fitxer `.ipynb` trobaràs:
- Una secció de càrrega i preparació de dades
- El preprocesament específic (textual o estructurat)
- L’execució pas a pas dels algorismes corresponents
- L’anàlisi dels resultats i visualitzacions

No és necessari cap script principal: pots obrir cada notebook individualment i executar-lo des del teu entorn Jupyter o editor compatible.

## 📄 Llicència

Aquest treball està protegit sota la llicència **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)**.

> Pots compartir i adaptar el contingut amb atribució, però **no per a ús comercial**.

Més informació: https://creativecommons.org/licenses/by-nc/4.0/