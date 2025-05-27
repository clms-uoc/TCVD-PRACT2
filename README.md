# TCVD-PRACT2

> CODE OWNER: Alexandre Sánchez (alexsanchezcasals@uoc.edu), Miguel Aloy (aloy793@hotmail.com)

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
├── dataset/                                        # carpeta amb els conjunts de dades
│   ├── glassdoor_jobs_original.csv                 # Dades del dataset original en brut recollides de Glassdoor
│   ├── glassdoor_jobs_processed.csv                # Dades del dataset original després de processades i netejades
│   ├── supervised-job_description_sample.csv       # Subconjunt del dataset de Kaggle per entrenar models supervisats
│   └── non-supervised-job_description_sample.csv   # Subconjunt del dataset de Kaggle per entrenar models no supervisats
│   └── hipotesis_test-job_description_sample.csv   # Subconjunt del dataset de Kaggle per executar el test d'hipotesi
│
├── source/                                         # scripts amb els algorismes i processament
│   ├── data_processing.ipynb                       # Script de preprocesament de les dades originals. No usat en els algorismes finals
│   ├── non-supervised_algorithm.ipynb              # Implementació d’un algorisme no supervisat (ex: KMeans) per agrupar perfils professionals
│   └── supervised_algorithm.ipynb                  # Implementació dels models de regressió per predir el salari
│   └── test_hipotesi.ipynb                         # Aplicació del test d'hipotesi
│
├── .gitignore                                      # Fitxer de configuració per ignorar arxius al repositori Git
├── .gitattributes                                  # Fitxer de configuració per afegir fitxers grans mitjançant Git LFS
├── LICENSE                                         # Informació sobre la llicència
├── README.md                                       # Documentació general del projecte
└── mapa_coropletic_ofertes_per_pais.png            # Visualització dinàmica de l'algorisme supervisat, afegida com a imatge separada
```


## 🔧 Requisits

### 📊 No supervisat:
```
- pandas
- re
- sklearn
- matplotlib
- seaborn
- rapidfuzz
- itertools
```

### 📈 Supervisat:
```
- polars
- pathlib
- plotly
- pandas
- matplotlib
- wordcloud
- sentence_transformers
- scikit-learn
- xgboost
```


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
