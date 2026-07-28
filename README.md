# Data Science & Machine Learning — Notebooks

Raccolta di notebook realizzati nell'ambito di un percorso di formazione in Data Science e Machine Learning. Il repository raccoglie esercitazioni, progetti ed esperimenti pratici svolti durante il master, con l'obiettivo di consolidare competenze su analisi dati, statistica, machine learning e strumenti per il trattamento di dati su larga scala.

## Contenuti

Ogni notebook è organizzato in una propria cartella all'interno di `notebooks/`, con un README dedicato che ne descrive obiettivi, dataset utilizzato e risultati ottenuti.

| Progetto | Descrizione | Tecniche/Strumenti |
|---|---|---|
| [01 - Wikipedia Articles Classification](notebooks/01-wikipedia-classification/) | Analisi esplorativa e classificazione automatica di articoli Wikipedia per categoria tematica | PySpark, Spark ML, Databricks |
| ... | ... | ... |

*(la tabella verrà aggiornata man mano che nuovi notebook vengono aggiunti al repository)*

## Struttura del repository

```
.
├── README.md
├── requirements.txt
└── notebooks/
    ├── 01-wikipedia-classification/
    │   ├── notebook.ipynb
    │   └── README.md
    └── ...
```

## Argomenti trattati

I notebook coprono in generale le seguenti aree:

- **Analisi esplorativa dei dati (EDA)** — pulizia, esplorazione e visualizzazione di dataset
- **Statistica** — analisi descrittiva e inferenziale, test di ipotesi
- **Machine Learning** — modelli di classificazione e regressione, pipeline di preprocessing, valutazione delle performance
- **Elaborazione del testo (NLP)** — text mining, feature extraction, classificazione testuale
- **Big Data** — elaborazione distribuita di dataset con Apache Spark

## Strumenti e librerie

- Python
- PySpark / Spark ML
- pandas, NumPy
- scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook / Databricks

## Come consultare i notebook

Ogni cartella in `notebooks/` è indipendente e contiene tutto il necessario per comprendere il progetto specifico (obiettivi, dati, metodologia, risultati). Si consiglia di partire dal README di ciascun progetto prima di consultare il notebook completo.

## Note

Questo repository ha finalità didattica e documentale: raccoglie esercitazioni svolte in un contesto formativo e non rappresenta codice production-ready.
