# Document-Clustering-for-Topic-Modeling
This project performs document clustering and topic modeling on a collection of text documents. The primary techniques used are Latent Dirichlet Allocation (LDA) for topic modeling and K-means clustering for grouping similar documents.

Table of Contents
Introduction
Project Structure
Dependencies
Usage
Data Preparation
Preprocessing
LDA Topic Modeling
K-means Clustering
Visualizations
Results
License
Introduction
This project demonstrates how to preprocess a large collection of text documents, perform topic modeling using Latent Dirichlet Allocation (LDA), and cluster documents using K-means clustering. Visualizations are included to help interpret the results.

Project Structure
The repository contains the following files:

Document_Clustering.ipynb: Main script to run the entire pipeline from data loading to visualizations.
requirements.txt: List of Python dependencies required for the project.
README.md: Project documentation.
Dependencies
Install the required dependencies using the following command:

bash
Copy code
pip install -r requirements.txt
Usage
Data Preparation
Manually extract the contents of your dataset (e.g., twenty+newsgroups.zip) into a folder. The folder should contain subfolders, each representing a different topic, and each subfolder should contain text files.

Ensure the extracted folder path is set correctly in the script.

Preprocessing
The script preprocesses the documents by:

Tokenizing the text.
Removing stop words.
Lemmatizing the tokens.
LDA Topic Modeling
The script performs LDA topic modeling and computes coherence scores to determine the optimal number of topics. It then trains a final LDA model using the optimal number of topics.

K-means Clustering
The script uses TF-IDF to vectorize the documents and applies K-means clustering to group similar documents. It prints the top terms for each cluster.

Visualizations
The script provides the following visualizations:

Coherence scores for different numbers of topics.
LDA topic visualization using PyLDAvis.
K-means clustering visualization using PCA.
To run the script, use the following command:


Results
The results include:

Optimal number of topics for LDA.
Top terms for each topic.
Top terms for each K-means cluster.
Visualizations for LDA topics and K-means clusters.
License
This project is licensed under the MIT License.
