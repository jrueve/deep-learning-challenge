# Overview of the analysis: Explain the purpose of this analysis.

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

# Results: Using bulleted lists and images to support your answers, address the following questions:

# Data Preprocessing

What variable(s) are the target(s) for your model?

The target variable is the 'IS_SUCCESSFUL' column from application_df

What variable(s) are the features for your model?

The feature variables are every other column from application_df --> this was defined by dropping the 'IS_SUCCESSFUL' column from the original dataframe

What variable(s) should be removed from the input data because they are neither targets nor features?

Both 'EIN' and 'NAME' columns were dropped/removed, because they were neither targets nor features for the dataset.

# Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?

Each model, after applying neural networks, consisted of a total of two layers at 4 and 8. these were just random guesses from which to iterate upon in the second try.

Were you able to achieve the target model performance?

No at first, but when optimized then yes.
A two-layer training model generated 249 parameters. The initial attempt achieved 72% accuracy, which fell slightly short of the desired 75%. The three-layer training model generated 2,001 parameters, and achieved 78.8% accuracy.

What steps did you take in your attempts to increase model performance?

Removed more columns, incorporated the "NAME" column in the dataset, and added one more layer.

Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

Multiple layers allow deep learning models to learn the process of prediction and classification by progressively refining and filtering input information through these layers. The model was 78.8% accurate, and could be improved with better data cleanup and different activation functions.