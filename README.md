# Educational Knowledge Graph Project

## Overview
This project focuses on building a **Knowledge Graph** from unstructured educational text data. The goal is to extract key concepts and model relationships between them using Python.

The system processes raw text documents, identifies important concepts using TF-IDF, and constructs a graph that visually represents how these concepts are connected.
---
### Run Online (No Setup Required)

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bless01/KDD_Group7/blob/main/project_knowledge_graph.ipynb)
---
## Methodology
1. **Text Preprocessing**  
   Clean text by lowercasing and removing noise.

1. **Sentence Segmentation**  
   Split text into sentences to capture context.

1. **Concept Extraction (TF-IDF)**  
   Extract key terms and bigrams based on importance.

1. **Concept Cleaning**  
   Remove irrelevant or inconsistent terms.

1. **Relationship Identification**  
   Link concepts appearing in the same sentence.

1. **Graph Construction (NetworkX)**  
   Build a graph where nodes are concepts and edges show relationships.

1. **Visualization**  
   Display the graph with node importance and connections.

---

## Objectives
- Convert unstructured text into structured knowledge
- Extract meaningful concepts using NLP techniques
- Build a graph representation of concept relationships
- Visualize concept importance and connections

---

## Technologies Used
- Python
- NetworkX (graph construction)
- Scikit-learn (TF-IDF vectorization)
- Matplotlib (visualization)
- Collections & Itertools (data processing)

---

## Project Pipeline

### 1. Data Collection
Text documents are stored in a `data/` folder and loaded into the system.

### 2. Text Cleaning
- Convert text to lowercase
- Remove special characters
- Normalize spacing

### 3. Sentence Splitting
Documents are split into sentences for relationship detection.

### 4. Concept Extraction (TF-IDF)
- Bigrams are extracted (e.g., "machine learning")
- Top concepts are selected based on importance.

### 5. Concept Cleaning
- Fix inconsistent terms (e.g., "science computer" → "computer science")
- Remove irrelevant phrases

### 6. Relationship Building
- Concepts appearing in the same sentence are connected
- Relationship strength is based on co-occurrence frequency

### 7. Knowledge Graph Construction
- Nodes represent concepts
- Edges represent relationships between concepts
- Node size reflects importance

### 8. Visualization
- Network graph showing concept relationships
- Pie chart showing concept distribution

---

## Results

## Project Structure
- data/ → dataset files  
- knowledge_graph.ipynb → main notebook  
- knowledge_graph.png → output visualization  
- README.md → project documentation

---

### Knowledge Graph
- "Machine Learning" appears as the central concept
- Strong connections with:
  - Artificial Intelligence
  - Data Science
  - Ethical Concerns
  - Recommendation Systems

### Concept Distribution
- Balanced distribution across major topics
- Reflects diversity of concepts in the dataset

---

## How to Run the Project

Follow these steps to run the project locally:

```bash
1. Install dependencies:
pip install networkx matplotlib scikit-learn pandas

2. Open Jupyter Notebook or JupyterLab
3. Open knowledge_graph.ipynb
4. Run all cells to generate the knowledge graph and visualizations
