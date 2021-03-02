# NLP-news-funniness


## Part 1 Implementation
To access part 1 implementation, please refer to the file Part1_combined.ipynb

Collab Link: [Part 1](https://colab.research.google.com/github/TerrenceCKCHAN/NLP-news-funniness/blob/main/Part1_combined.ipynb)

The file comes with three models and three different embeddings to choose from. It shows the train, validation and test loss as well as graphs showing the losses vs epochs during training.

To run different models, please change the 
model_to_run parameter, with 0 = BiLSTM, 1 = BiLSTM-Attention, 2 = FFN

To run different embeddings, please change the parameter
picked_embeddings, with 0 = pre-made glove, 1 = custom word2vec, 2 = custom fasttext

These parameters are set in the last "Hyperparameters and data loading" cell.

After running the file once, subsequent embeddings and models can be tested just by changing the relevant numbers in the cell, and then running the "Hyperparameters and data loading" cells and all cells below it. There is no need to run the "Set up" cells more than once.
The file works best when run with a GPU runtime. 

Please make sure that the following files are in the same working directory as the colab:
	-test.csv
	-train.csv 
	-dev.csv
You might need to manually upload some of the files. File uploading can be done with the "upload to session storage" button in the files tab of Google Colab. 
The GloVe data is imported in the code itself, but for expediency's sake, the glove.6B.100.txt file can also be uploaded directly. 
The word embeddings do not need to be uploaded: these are generated in the code itself. 

## Part 2 Implementation
To access part 2 implementation, please refer to the file Part2_experiments.ipynb

Preprocessing (stemming and lemmatization) and models tested (linear regression, polynomial regression, SVR, random forest regression, lasso and ridge regression) are available under the corresponding headings in the notebook.

Before running model cells, run the cells included before the 'Approach 2: No pre-trained representations' heading.

Collab Link: [Part 2](https://colab.research.google.com/github/TerrenceCKCHAN/NLP-news-funniness/blob/main/Part2_experiments.ipynb)


