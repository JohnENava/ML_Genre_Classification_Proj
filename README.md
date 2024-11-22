# Music Genre Classifcation Project
Machine Learning Music Genre Classification Project

# Overview
This repository contains the files and code for our music genre classfication proejct. Using the GTZAN dataset, we set out to predict the genre of songs based on their audio features. From experimenting with a KNN model to fine-tuning an SVM classfier, this project reflects the combined efforts of our team. 

# Project Files

1. Features_30_sec.csv
   This file is part of the GTZAN dataset. It contains features extracted from 30-second-long songs, including mean and variance values for properties like spectral centroid, roll-off, and tempo. Each row corresponds to a sing song, and this strcuted data served as a strong frpoundation for training our model.

2. Features_3_sec.csv
   Also from the GTZAN dataset, this file splits songs into 3-second segments before extracting the same features as the 30-second file. By increasing the dataset size tenfold, this file provided us with more data for experimentation and training. With data, more is always better-or so we throught when starting this journey.

3. ML Song Classfication SVM.ipynb
   This notebook represents the final working model. Using an SVM classifier, we achieved an accruacy of 86%. Data prepocessing included balancing classes with SMOTE and scaling features for better perfroamcne. The SVM model captured the subleties of most genres, though it strugged with overlapping genres like "rock" and "disco."

4. MLSC_KNN_MSD.ipynb
   This notebook documents the early stages of our proejct. It features an attempt to classify genres using a KNN model with a subset of the Million Song Dataset. While this intital approach seemed promsing, the KNN model only achieved an accuracy as high as 22%. The dataset subset sourced from the Million Song Dataset, was valuable but lacked the diversity needed for accurate predictions. This notebook remains as a reflection of our early exploration.

5. README.md
   This file provides an overview of the project, its files, and its goals. This is the current file.

# The GTZAN Dataset
The GTZAN dataset was instrumental and a life saver to this project, providing the structured data we needed for genre classifcaiton. It consist of two CSV files:

1. Features_30_sec.csv: Features extracted from 30-second-long audio clips, with mean and variance values summarizing various properties of the songs.
2. Features_3_sec.csv: The same as above, but split into 3-second segments, effectively increasing the dataset size by tenfold. While this provided more data, it also introduced challenges in preprocessing and balancing.

These files gave our models the opportunity to learn pattersn in music, laying the groundwork for genre classification.

# The Journey
As a team, we wanted to explore how machine learning could interpret music genres, reflecting the diverse styels and emotions that music conveys.

We started with a KNN model using a subset of the Million Song Dataset. While it was a good introduction, the rsults-an acurracy of 22%-highlighted the need for better data and tools. Transitioning to the GTZAN dataset and refining our approach with SVM brought significant improvements, ahcieving 86% accuracy. Every step, even the setbacksm was a learning experience for the team.

# Challenges and Insights

Imbalanced Classes: Genres like "classical" were underrepresented, making it harder for the model to learn those patterns. Using SMOTE to balance the data improved the results significantly.

Feature Engineering: The mean and variance features from the GTZAN dataset provided a solid foundation, but their summarization limited the depth of analysis compared to raw audio data.

Model Selection: While KNN was a simple starting point, it became clear early on that it couldn’t capture the nuances of the dataset. The SVM model proved to be a better fit.

# Visualization and Resutls
Visualizing the data through PCA (Principal Component Analysis) revealed patterns and clusters that helped us understand the dataset better. Some genres, like "classical" and "metal," were easier to distinguish, while others, like "rock," overlapped heavily with similar genres. These visualizations guided our decisions and highlighted the strengths and weaknesses of our models.

# Acknowledgments
We’d like to thank the creators of the GTZAN and Million Song datasets for making such invaluable resources available to the research community. Their work has been the foundation for this project and many others like it.

