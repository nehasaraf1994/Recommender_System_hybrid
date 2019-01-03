# Final Project - Amazon Clothes, Jewelry and Shoes Recommendation
final-project-amazon-movies-recommendation created by GitHub Classroom

This project implements two models: Content based model which has been implemented using Autoencoders and Random Forest Regression
The second approach used for building the recommendation engine is: Locality Sensitive Hashing + Neighborhood-based Collaborative Filtering.

The dataset used: Amazon Clothes, Jewelry and Shoes - ratings and items metadata.

The dataset should be downloaded from the link : http://jmcauley.ucsd.edu/data/amazon/ 
This is a public dataset but to get the full access to dataset, you should contact Julian McAuley(email : ude.dscu.gne@yeluacmj)

## Summary of the files uploaded:

D2v_final.model- Doc2Vec model trained on all textual information available in the item dataset using gensim library.

DeepLearning_recommendation_keras_create_model.ipynb - This file is used to train an auto encoder model on 60000 images from our item dataset, test if the latent space representation of images obtained at the encoder layer is effective and store the model.

DeepLearning_recommendation_keras_load_model- This file is used to obtain the latent space representation of all images in our item dataset using the stored encoder model and store it as content profile in a csv file. 

Encoder2.h5- Stored encoder model

Item_vector_image3.csv: This file contains the latent space representation of item images as a vector of length 16.

Item_vector2.csv: This file contains the latent space representation of all item text information as a vector of length 15.

Recommendation_system_content_subset1: This file is used to run our hybrid content-based recommendation system on our first subset.

Recommendation_system_content_subset2: This file is used to run our hybrid content-based recommendation system on our second subset.

Recommendation_system_content_subset3: This file is used to run our hybrid content-based recommendation system on our third subset.

Recommendation system_EDA: This file contains exploratory data analysis of our dataset.

Word-vec-create-model - This file is used to create a doc2vec model trained on all text information on items, test the effectiveness of the model created and store the model.

Word-vec-load-model- This file is used to obtain the latent space representation of all text information of items in our item dataset using the stored doc2vec model and store it as content profile in a csv file. 

LSH_spark - implements the LSH algorithm on the ratings dataset with the output of aprroximate neighbors of a user.

NeighborhoodBased - This file combines the LSH algorithm with the implementation of neighborhood-based model of collaborative filtering. 
