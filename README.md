# AudioBook-TensorFlow

Predicting Human behaviour is one of the hardest to predict but somehow I will be trying to predict the human behaviour using neural networks.

The given data from an Audiobook App. Logically, it relates to the audio versions of books ONLY. Each customer in the database has made a purchase at least once, that's why he/she is in the database. We want to create a machine learning algorithm based on our available data that can predict if a customer will buy again from the Audiobook company.

The targets(last column) are a Boolean variable (0 or 1). We are taking a period of 2 years in our inputs, and the next 6 months as targets. So, in fact, we are predicting if: based on the last 2 years of activity and engagement, a customer will convert in the next 6 months. 6 months sounds like a reasonable time. If they don't convert after 6 months, chances are they've gone to a competitor or didn't like the Audiobook way of digesting information. 

I have to remove the Column headers because we dont need any text in our data.

I have followed below steps :

Pre-Process the Data

    1.Balance the dataset
    
    2.Standardize the inputs using Sklearn preprocessing
    
    3.Shuffle the data
    
    4.Divide the dataset into train and test – prevent over fitting
    
    5.Save the data into tensor friendly format
    
    6.Used two hiddenlayers
    
    7.Used ADAM optimizer and sparse_categorical_crossentropy loss with accuracy as metrics
    
    8.Used "SOFTMAX" activation for output layer
    
 
 Able to predict with 88% accuracy whether a customer will convert and buy another time or not.
