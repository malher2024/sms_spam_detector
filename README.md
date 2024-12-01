# sms_spam_detector

# Challenge Instructions
The starter files consist of the following files: **gradio_sms_text_classification.ipynb**, **sms_text_classification_solution.ipynb**, and **SMSSpamCollection.csv**.

# Create the SMS Classification Function
1. Using the code in the sms_text_classification_solution.ipynb file, create the sms_classification function in the gradio_sms_text_classification.ipynb by doing the following:
    - Set the features variable to the text message column of the DataFrame.
    - Set the target variable to the "label" column of the DataFrame.
    - Split data into training and testing and set the test_size to 33%.
    - Build a pipeline to transform the test set to compare to the training set.
    - Fit the model to the transformed training data and return model.

2. Load the SMSSpamCollection.csv into a DataFrame and call the sms_classification function with the DataFrame, and set the result to the "text_clf" variable.

# Create the SMS Prediction Function
Use the sms_prediction function to predict the classification of a new text by doing the following:

- Create a variable that will hold the prediction of a new text.
- Use a conditional statement that determines if the text message is "ham" or “spam”.
  - If the message is “ham”, the function should return the following message: f'The text message: "{text}", is not spam.'
  - If the message is spam, the function should return the following message: f'The text message: "{text}", is spam.'

# Create the Gradio Interface Application
1. Create a Gradio Interface application that takes a textbox for the inputs and has a textbox for the output. The textboxes should have labels that describe what each textbox contains.
2. Launch the application and provide the URL to share the application. Your application should look like the following:

3. Use the following text messages to test your application.

1. You are a lucky winner of $5000!  **Not Spam**
2. You won 2 free tickets to the Super Bowl. **Spam**
3. You won 2 free tickets to the Super Bowl. Text us to claim your prize. **Spam**
4. Thanks for registering. Text 4343 to receive free updates on medicare.  **Spam** 

