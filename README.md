# Deep-learning-challenge

**Background**

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

**EIN** and **NAME**—Identification columns
**APPLICATION_TYPE**—Alphabet Soup application type
**AFFILIATION**—Affiliated sector of industry
**CLASSIFICATION**—Government organization classification
**USE_CASE**—Use case for funding
**ORGANIZATION**—Organization type
**STATUS**—Active status
**INCOME_AMT**—Income classification
**SPECIAL_CONSIDERATIONS**—Special considerations for application
**ASK_AMT**—Funding amount requested
**IS_SUCCESSFUL**—Was the money used effectively

**Overview of the analysis: Explain the purpose of this analysis**

Results: Using bulleted lists and images to support your answers, address the following questions:

**Data Preprocessing**

1. What variable(s) are the target(s) for your model?
- The target variable is the 'IS_SUCCESSFUL' column from application_df

2. What variable(s) are the features for your model?
- The feature variables are every other column from application_df --> this was defined by dropping the 'IS_SUCCESSFUL' column from the original dataframe
- 
3. What variable(s) should be removed from the input data because they are neither targets nor features?
- Both 'EIN' and 'NAME' columns were dropped/removed, because they were neither targets nor features for the dataset.
- 
**Compiling, Training, and Evaluating the Model**

1. How many neurons, layers, and activation functions did you select for your neural network model, and why?
- In the first attempt, i used 8 hidden_nodes_layer1 and 5 hidden_nodes_layer2 -- these were just random guesses from which to iterate upon in the second try.
2. Were you able to achieve the target model performance?
- I'm not sure if I was able to achieve the 75% model accuracy target.

3. What steps did you take in your attempts to increase model performance?
- I added more layers, removed more columns, added additional hidden nodes, and switched up the activation functions associated with each layer in an attempt to achieve higher model accuracy.
- 
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

Overall, I think the deep learning model was around 73% accurate in predicting the classification problem. Using a model with greater correlation between input and output would likely result in higher prediction accuracy. This could be achieved by doing additional data cleanup up front, as well as by using a model with different activation functions and iterating until higher accuracy is reached.

The Google Colab notebook/Jupyter notebook files are in the Starter_Code folder.
