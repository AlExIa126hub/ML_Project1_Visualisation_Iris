# Iris Dataset Visualisation

Machine Learning practical assignment focused on exploring and visualising Fisher’s Iris dataset using Python data analysis and visualisation libraries.

The project investigates the relationships between flower measurements and species categories through multiple 2D and 3D visualisations.

Dataset source:  
https://scikit-learn.org/stable/auto_examples/datasets/plot_iris_dataset.html


---

# Project Structure

```
iris-dataset-visualisation/
│
├── iris_visualisation.ipynb
└── README.md
```


---

# Project Overview

The goal of this project is to explore and visualise Fisher’s Iris dataset in order to better understand the relationships between different flower measurements and species classification.

The analysis focuses on visual exploration rather than predictive modelling. Various visualisation techniques are used to observe patterns in the dataset and determine whether the different species can be distinguished based on their physical characteristics.

The project follows three main stages:

1. Dataset exploration  
2. Feature engineering  
3. 2D and 3D visualisation  


---

# Dataset

The Iris dataset is one of the most widely used datasets in machine learning and statistics. It contains measurements of iris flowers belonging to three different species:

- Setosa  
- Versicolor  
- Virginica  

Each observation includes the following features:

- sepal length  
- sepal width  
- petal length  
- petal width  

The dataset also includes the **species label**, which indicates the class of each flower.


---

# Feature Engineering

In addition to the original features, two new variables were created to better capture the overall size of different flower parts.

Petal area was approximated as:

```
petal_area = petal_length * petal_width
```

Sepal area was approximated as:

```
sepal_area = sepal_length * sepal_width
```

These engineered features provide additional insight into how the size of petals and sepals varies between species.


---

# Exploratory Data Analysis

The dataset was first explored using basic inspection methods to understand its structure and contents.

The analysis then focused on visualising the distribution of each feature using histograms and density plots.

Key questions explored include:

- how each feature is distributed  
- how feature distributions differ between species  
- whether certain measurements separate species more clearly than others  

The visualisations show that **petal measurements tend to provide stronger separation between species than sepal measurements**.


---

# 2D Visualisations

Several types of 2D plots were used to analyse relationships between variables.

### Histograms
- Distribution of sepal length, sepal width, petal length and petal width  
- Distribution of engineered features (petal area and sepal area)

### Species-based distributions
- Histograms coloured by species to observe class separation

### Scatter plots
- Sepal length vs sepal width  
- Petal length vs petal width  
- Petal length vs sepal length  
- Petal width vs sepal width  
- Petal area vs sepal area  

These plots help reveal how different species cluster in the feature space.


---

# 3D Visualisations

To further explore the dataset, several 3D visualisations were created.

Two different approaches were used.

### Static 3D plots (Matplotlib)

A 3D scatter plot was created where:

- axes represent different flower measurements  
- point size reflects sepal width  
- colour indicates species  

This allows multiple dimensions of the dataset to be visualised simultaneously.

### Interactive 3D plots (Plotly)

Interactive 3D scatter plots were generated to allow dynamic exploration of the dataset.

Examples include:

- petal length vs petal width vs sepal length  
- sepal area vs petal area vs petal length  
- sepal area vs petal area vs sepal length  

Interactive visualisations make it easier to rotate and inspect clusters corresponding to the different species.


---

# Technologies Used

- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Plotly  
- Jupyter Notebook  


---

# Running the Project

Install dependencies:

```
pip install pandas numpy matplotlib seaborn plotly
```

Launch Jupyter Notebook:

```
jupyter notebook
```

Open and run:

```
iris_visualisation.ipynb
```


---

# Dataset

Iris Dataset (Scikit-learn)

https://scikit-learn.org/stable/auto_examples/datasets/plot_iris_dataset.html
