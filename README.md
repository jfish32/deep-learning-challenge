# deep-learning-challenge

Alphabet Soup Charity Analysis

Overview

The purpose of this analysis is to attempt to create a neural network model to predict if a campaign was successful or not based on a list of features.  During optimization, I played with the number of nodes, the amount of hidden layers as well as adding and subtracting features in an attempt to achieve over 75% accuracy.

Results

DATA PREPROCESSING

-The variable that was the target for our model was ‘IS_SUCCESFUL’ just meaning was that specific campaign successful or not.

-The variables that I originally used as features are Application_Type, Affiliation, Classification, Use_Case, Organization, Status, Income_Amt, Special_Considerations and Ask_amt.

-Variables that can be removed are for sure EIN because that is just an identifier, we could also remove the NAME as it slows down the model and doesn’t help us predict if a campaign is successful or not.

COMPILING, TRAINING AND EVALUATION
-In my optimization attempt I selected 100,100 and 50 neurons for my 3 hidden layers.  I then used ‘relu’ activation for my first and third layers and a ‘swish’ activation for my second.  I googled swish and it said it can sometimes outperform relu so I gave it a shot.  

-Upon many optimization attempts I was able to increase the accuracy and by the final epochs of training my models accuracy was at about 77%

-Steps taken to increase model performance were adding and dropping features, adding an additional hidden layer, increasing the neurons, changing the activation (I tried relu,tanh and swish).

SUMMARY

I think my model ended up doing an okay job of predicting if a campaign were to be successful based on the features provided.  Perhaps a random forest model would be worth looking at to predict if this is successful or not.  This will help us narrow down which features matter more and can focus on those areas for future campaigns.
