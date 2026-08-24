# Lateral Practicum

A progressive ML/AI curriculum covering Python fundamentals through modern LLM-based applications.

---

## Assignments

| # | Notebook | Summary |
|---|----------|---------|
| 01 | [Python OOP & CLI Programming](Assignment%2001%20-%20Python%20OOP%20%26%20CLI%20Programming.ipynb) | Builds a command-line To-Do app using Python classes (`Task`, `Repo`, `CLI`) to practise object-oriented design patterns and interactive CLI development. |
| 02 | [Exploratory Data Analysis & Visualization](Assignment%2002%20-%20Exploratory%20Data%20Analysis%20%26%20Visualization.ipynb) | Analyses the NYC Airbnb 2019 dataset with in-depth EDA, statistical summaries, and rich visualisations including maps, distributions, and top-listing rankings. |
| 03 | [Data Wrangling & Feature Engineering](Assignment%2003%20-%20Data%20Wrangling%20%26%20Feature%20Engineering.ipynb) | Works with the Titanic training dataset to practise data cleaning, missing-value handling, and feature engineering as preparation for modelling. |
| 04 | [Regression & Statistical Analysis](Assignment%2004%20-%20Regression%20%26%20Statistical%20Analysis.ipynb) | Explores the California Housing Prices dataset through distribution histograms, correlation analysis, and regression modelling to predict median house values. |
| 05 | [Classification Algorithms](Assignment%2005%20-%20Classification%20Algorithms.ipynb) | Applies Logistic Regression, Decision Tree, Random Forest, and SVM to the Cleveland Heart Disease dataset, comparing model performance after thorough data preprocessing and imputation. |
| 05b | [Classification with Categorical Features](Assignment%2005b%20-%20Classification%20with%20Categorical%20Features.ipynb) | A variant of Assignment 05 focusing on encoding and handling categorical variables in the Heart Disease dataset before classification. |
| 06 | [Classification & Hyperparameter Tuning](Assignment%2006%20-%20Classification%20%26%20Hyperparameter%20Tuning.ipynb) | Classifies poisonous vs. edible mushrooms (UCI) with multiple classifiers and fine-tunes the best model using Grid Search cross-validation. |
| 07 | [Unsupervised Learning & Clustering](Assignment%2007%20-%20Unsupervised%20Learning%20%26%20Clustering.ipynb) | Segments Mall Customers using KMeans, DBSCAN, GMM, Mean Shift, and Agglomerative Clustering, evaluating results with silhouette and Davies–Bouldin scores. |
| 07b | [Clustering on Credit Card Data](Assignment%2007b%20-%20Clustering%20on%20Credit%20Card%20Data.ipynb) | Repeats the clustering workflow on the CC GENERAL credit-card dataset to reinforce unsupervised learning techniques on a different domain. |
| 08a | [Neural Networks — Regression](Assignment%2008a%20-%20Neural%20Networks%20Regression.ipynb) | Trains Keras neural networks to predict building heating and cooling loads (UCI Energy Efficiency), with K-Fold cross-validation and an Adam vs. SGD optimiser comparison. |
| 08b | [Neural Networks — Classification](Assignment%2008b%20-%20Neural%20Networks%20Classification.ipynb) | Uses a Keras neural network to classify wine quality (UCI Wine), extending deep-learning skills to a multi-class classification task. |
| 09a | [Convolutional Neural Networks from Scratch](Assignment%2009a%20-%20Convolutional%20Neural%20Networks%20from%20Scratch.ipynb) | Designs and trains a custom CNN with PyTorch Lightning to classify plant images, covering dataset pipelines, augmentation transforms, and training callbacks. |
| 09b | [Transfer Learning & Layer Freezing](Assignment%2009b%20-%20Transfer%20Learning%20%26%20Layer%20Freezing.ipynb) | Applies transfer learning on a pretrained backbone for plant classification by selectively freezing layers and fine-tuning the classifier head. |
| 09c | [CNN Architecture Comparison](Assignment%2009c%20-%20CNN%20Architecture%20Comparison.ipynb) | Benchmarks multiple CNN architectures on the same plant dataset to compare accuracy, training time, and generalisation. |
| 09d | [EfficientNet-B1 Fine-Tuning](Assignment%2009d%20-%20EfficientNet-B1%20Fine-Tuning.ipynb) | Fine-tunes EfficientNet-B1 for plant image classification, leveraging a state-of-the-art architecture with compound scaling for high accuracy. |
| 10 | [Large Language Models & AI Agents](Assignment%2010%20-%20Large%20Language%20Models%20%26%20AI%20Agents.ipynb) | Builds a LangGraph-powered AI botanist agent that uses tool-calling, web search (Tavily), and an EfficientNet plant classifier to generate structured plant-care cards. |
| 10b | [LLM Agents v2](Assignment%2010b%20-%20LLM%20Agents%20v2.ipynb) | A revised iteration of the LLM agent pipeline with refinements to prompts, graph nodes, and validation logic. |
| 11 | [Retrieval-Augmented Generation (RAG)](Assignment%2011%20-%20Retrieval-Augmented%20Generation.ipynb) | Implements a full RAG system using LanceDB vector storage, sentence-transformer embeddings, and LangChain, evaluated with the RAGas framework. |

---

## Final App — Plant Care Card

The capstone project combines everything from the curriculum into a production-ready **CNN + RAG pipeline** that:

- 📸 Accepts a plant photo and classifies it using a fine-tuned **EfficientNet-B1** model (Assignment 09d)
- 🔍 Retrieves relevant care information via **RAG** with LanceDB + sentence-transformers (Assignment 11)
- 🤖 Generates a structured **plant-care card** using a LangGraph AI agent (Assignment 10)
- 🌐 Serves everything through a **Streamlit** web interface, containerised with Docker

👉 **Source code**: [`Final_App/`](Final_App/)  
👉 **Original repo**: [github.com/stefansandru/plant-care-card](https://github.com/stefansandru/plant-care-card)
