# Optimize a Neural Network and Deep Learning Algorithm 

The purpose of this analysis is to create a model that will help a nonprofit foundation called AlphabetSoup. The model created will help choose applicants for funding that will have the best chance of sucess in their ventures. A model was created with a binary classifier that will predict whether applicants will be successful, if funded by AlphabetSoup.

<img width="1112" alt="image" src="https://github.com/diego-lazaro/deep_learning_challenge/assets/115186079/7551743b-7391-494a-9087-ca7ee4d6410f">


# Step 1: Data Preprocessing

The target variable for this model is the "IS_SUCCESSFUL" column. The features of the model are "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS" "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT". There were two dataset columns that had irrelevant data, which were "EIN" and "NAME." These columns were removed because they were NOT the target or feature variables needed for this model. The model revealed if the two columns were NOT dropped then the session would crash due to exceeding Google Colab's RAM usage limit.

<img width="674" alt="image" src="https://github.com/diego-lazaro/deep_learning_challenge/assets/115186079/332a2559-f371-4496-adfe-2c1daefd78be">


# Step 2: Compile, Train, and Evaluate the Model

The orginal model contained 3 layers with values of 7, 14, and 1 neuron in each layer. These were arbitrary numbers which were used as a starting point for the model. The target accuracy of at least 75% was not achieved by the orginal model with 100 epochs. 

# Step 3: Optimize the Model

The model was optimized twice by making adjustments to the layers. This was accomplished by adding another hidden layer, adding more neurons to each layer, adding more columns from the original data, using various amounts of epochs, and changing the binning and cutoff values to optimize the model and increase it's performance, but in the allotted time given my model was not able to reach the targeted 75% accuracy.

# Conclusion 

The most accurate model observed had only 3 hidden layers with 7, 14, and 1 neurons in each layer. This model had a cutoff value of 500 for application types and a cutoff of 100 for classification and ran over 100 epochs. This model achieved 73% accuracy. This was done by adding more layers and neurons, changing the epochs, and adding lower cutoffs for binning. By doing this, decreased the accuracy of the model. The model was adjusted by running the model with all of the original columns to the dataset but the session crashed. A new model with fewer features, similar layers and neurons, and higher cutoffs would most likely solve the classification problem.

<img width="440" alt="image" src="https://github.com/diego-lazaro/deep_learning_challenge/assets/115186079/18384160-3bb4-4b0b-8012-4a92a8dff5b7">
