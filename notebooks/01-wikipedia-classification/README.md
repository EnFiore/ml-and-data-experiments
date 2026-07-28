# Analisi di Wikipedia con Spark
Progetto di analisi esplorativa e classificazione automatica di articoli Wikipedia, sviluppato in **PySpark** su **Databricks**.

## Obiettivi

1. **Analisi descrittiva dei contenuti (EDA)** — caratterizzare gli articoli suddivisi per categoria tematica (Cultura, Economia, Medicina, Tecnologia, Politica, Scienza, ecc.)
2. **Classificatore automatico** — addestrare un modello ML per predire la categoria di un articolo a partire dal testo
3. **Riconoscimento delle lingue** — identificare la lingua di ciascun articolo

## Struttura del notebook

### 1. Importazione del dataset
Caricamento del dataset e conversione in Spark DataFrame.

### 2. Analisi del dataset
- Ispezione tipi di dato e contenuto
- Gestione dei duplicati
- Distribuzione delle categorie (conteggio e occorrenze)
- Analisi della lunghezza degli articoli per categoria, incluse le distribuzioni

### 3. Sviluppo del classificatore automatico
- Creazione di una colonna unica di testo combinato a partire dai campi testuali del dataset
- Split train/test
- Pipeline di preprocessing e feature engineering (Spark ML)
- Addestramento e confronto di due modelli:
  - **Logistic Regression**
  - **Random Forest**

**Risultati:**

| Modello | Accuratezza |
|---|---|
| Logistic Regression | 0.80 |
| Random Forest | 0.53 |

La Logistic Regression ha ottenuto risultati nettamente migliori. Il Random Forest, pur essendo un metodo ensemble generalmente robusto, tende a soffrire su dati sparsi ad alta dimensionalità come i vettori bag-of-words derivati dal testo.

### 4. Riconoscimento delle lingue
Rilevamento automatico della lingua di ogni articolo tramite `langdetect`, con conteggio delle frequenze e word cloud riassuntiva delle 15 lingue rilevate.

## Tecnologie utilizzate
- PySpark / Spark ML
- Databricks
- WordCloud
- langdetect, langcodes

## Bibliografia
1. [Removing stopwords from text with Spark NLP](https://www.johnsnowlabs.com/text-cleaning-removing-stopwords-from-text-with-spark-nlp/)
2. [Multi class classification with PySpark](https://medium.com/data-science/multi-class-text-classification-with-pyspark-7d78d022ed35)
3. [Text language detection with Python](https://medium.com/@monigrancharov/text-language-detection-with-python-beb49d9667b3)

