## Predicting Author's Birth Year from Written Text Excerpts

Develop a model to predict the year the author was born in given an excerpt of the author's writing. 

Authors: Chester Ni, Colin Kavanagh, Darren Jiang, Jared Simpauco, Jack Howe

## General

This project focuses on creating a model to predict an author's birth year based solely on the style of their writing. The core objective is to establish if linguistic attributes in a text can reveal the period when the author was born.

To gather the data necessary for this project, we pulled data from Project Gutenberg, a non-profit online library of free eBooks. We used a combination of Gutendex, a third-party metadata API for Project Gutenberg, and webscraping off of Project Gutenberg's archive files. From there, we cleaned the text samples using regex, limited samples to certain range of lengths, and balanced out the number of samples based off of century to obtain our final dataset. 

Once the dataset was created, we tested a variety of machine learning models (SVM, KNN, XGBoost Regressor, Random Forest models, LSTM Neural Network Regressor) and evaluated them based on RMSE. The model with the lowest RMSE was chosen as the final model. 

## Data Instructions

The original project report is the file labeled `FinalProject.ipynb`. 

Our project data is stored as two .csv files in a .zip archive in the Project_Files folder. To get started, clone this repo and then extract the files within the data.zip archive and into a folder called "data" within the Project_Files folder. Our .gitignore file will ignore all .csv files, so these files will not be pushed to the repo.