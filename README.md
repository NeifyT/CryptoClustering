# Cryptocurrency Cluster

   ### CONTENTS
**[The Challenge](#the-challenge)**<br>
**[Starter Code](#starter-code)**<br>
**[Challenge Checklist](#challenge-checklist)**<br>
**[Running the Program](#running-the-program)**<br>
**[Notable Issues](#notable-issues)**<br>
**[Data Analysis Answers](#data-analysis-answers)**<br>

## The Challenge

Create an unsupervised machine learning model, by grouping cryptocurrencies, that could be used to assemble investment portfolios based on the profitability of those cryptocurrencies. *The greater challenge for me will be to suspend my personal belief that cryptocurrencies and their associated blockchain technology are the biggest scam of our time. Hence the output of this program should **not** be taken as investment advice nor used to facilitate any actual trading of cryptocurrencies.*

## Starter Code

The starter code for this challenge consists of a notebook file (.ipynb) which will run in Jupyter, Jupyter Lab, or VS Code with Jupyter extensions and a data (.CSV) file with information of cryptocurrencies. The notebook contains code commenting to match the workflow of the challenge, questions for answering, initial code to import packages, read and display the initial data set, and expected cell outputs.

## Challenge Checklist

With the greater complexity of this challenge I will simplify my usual checklist style to only the main process flow and notable grading criteria.

### Workflow

- [x] Prepare the data by scaling and setting the index.
- [x] Find the best value for K-Means (‘k’ number of clusters) of the scaled data
- [x] Cluster the scaled data into ‘k’ clusters
- [x] Use Principal Component Analysis (PCA) to find and reduce data to three components stored in a new DataFrame
- [x] Find the best value for K-Means of the PCA data
- [x] Cluster the PCA data into ‘k’ clusters
- [x] Weight the PCA data
- [x] Answer applicable data analysis questions in the notebook file

### Notable Grading Criteria

- [x] Utilize Python specific coding conventions and formatting
- [x] Utilize software source control Git and repository GitHub
- [x] Add additional commenting such that other developers can follow my logic beyond just the workflow outline (which I will do with a double hash [##] and docstrings)

## Notable Issues

As I happen to work on this code within three different Python environments, I noted that the KMeans algorithm returned different inertia values depending on which version of scikit-learn was installed. Because of this issue, I saved the cell outputs in the notebook so any review of the Elbow Curve plot and best ‘k’ analysis would make sense within the context I ran the notebook. Different versions of scikit-learn could perhaps be evaluated with a different best ‘k’.

## Running the Program

The program folder contains the completed notebook which can be run cell by cell from and results displayed in Jupyter, Jupyter Lab, or VS Code with Jupyter extensions.

```
Crypto_Clustering.ipynb
```

The outputs for all cells in the notebook have been saved specifically to retain the best ‘k’ analysis. The notebook cells could be run from top to bottom. Outputs will closely resemble those displayed in the original starter code file, but may vary slightly.

I decided to add an additional function with logic that could be used to  automate the decision for the best K-Means number of clusters, based on the elbow method but without needing an expert to read a plot.

## Data Analysis Answers

Answers to the questions will be saved within the notebook in their associated markdown cells.