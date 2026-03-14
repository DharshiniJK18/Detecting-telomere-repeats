#  Telomere Repeat Identification and Genome Distribution Analysis

This project was **carried out under the supervision of Mr. Arun Arumugaperumal, Assistant Professor of Biotechnology**.
The work focuses on analyzing telomeric DNA repeat motifs and exploring their identification using computational and machine learning approaches.

---

## 📌 Project Overview

Telomeres are repetitive DNA sequences located at the ends of chromosomes that protect genetic material from degradation.
In humans, the canonical telomeric repeat motif is:

`TTAGGG`

This project combines **genomic sequence analysis** and **machine learning techniques** to:

* Identify telomere-associated DNA motifs across species
* Train machine learning models to classify telomeric motifs
* Visualize the distribution of repeat motifs across a chromosome

---

## 🧠 Conceptual Workflow

```
Telomere Motif Dataset
        │
        ▼
Machine Learning Classification
(Random Forest / KNN / Neural Network)
        │
        ▼
Motif Identification
        │
        ▼
Genome Scan (Chromosome 22)
        │
        ▼
Repeat Distribution Visualization
```

---

# 📂 Repository Structure

```
telomere-repeat-analysis/
│
├── telomere_motif_classifier_ml.ipynb
├── telomere_repeat_distribution_chr22.ipynb
├── telomere_motif_dataset.csv
├── chr22.fa
└── README.md
```

---

# 🔬 Files Explained

## telomere_motif_classifier_ml.ipynb

Machine learning notebook used to classify whether a DNA motif corresponds to a telomeric repeat.

### Steps performed

1. Load motif dataset
2. Preprocess features and labels
3. Split the dataset into training and testing sets
4. Train multiple machine learning models:

   * Random Forest
   * K-Nearest Neighbors (KNN)
   * Neural Network (MLPClassifier)
5. Evaluate model performance using confusion matrix and accuracy metrics.

---

## telomere_repeat_distribution_chr22.ipynb

Genome analysis notebook used to visualize motif distribution across chromosome sequences.

### Steps performed

1. Load chromosome FASTA sequence
2. Accept motif input from the user
3. Scan the sequence for motif occurrences
4. Divide the chromosome into windows of **1000 base pairs**
5. Count motif frequency in each window
6. Visualize distribution using a scatter plot.

Example input:

```
TTAGGG
```

Output: graphical representation of motif occurrences across chromosome 22.

---

## telomere_motif_dataset.csv

Dataset containing short DNA motifs across multiple species and their classification labels.

Example entries:

| Motif  | Species      | Label |
| ------ | ------------ | ----- |
| TTAGGG | Homo sapiens | Yes   |
| CCCTAA | Homo sapiens | Yes   |
| GAGTTG | Homo sapiens | No    |

---

# ⚙️ Requirements

Python 3.x

Install dependencies using:

```
pip install numpy pandas scikit-learn matplotlib biopython
```

Required libraries:

* NumPy
* Pandas
* Scikit-learn
* Matplotlib
* Biopython

---

# ▶️ Running the Project

### Clone the repository

```
git clone https://github.com/yourusername/telomere-repeat-analysis.git
cd telomere-repeat-analysis
```

### Run genome motif analysis

Open and run:

```
telomere_repeat_distribution_chr22.ipynb
```

Enter a motif such as `TTAGGG` when prompted.

---

### Train the machine learning model

Open and run:

```
telomere_motif_classifier_ml.ipynb
```

The notebook trains several classifiers and evaluates prediction performance.

---

#  Biological Background

Telomeres consist of repetitive DNA sequences that protect chromosome ends from degradation and genomic instability.
In humans, the telomeric repeat motif is:

```
TTAGGG
```

These repeats form protective caps at chromosome ends and play important roles in aging, genome stability, and cancer biology.

---


