# Neural_Network_Charity_Analysis

## Overview:

This week we are tasked with using machine learning and neural networks to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

All work was conducted on a CSV containing more that 34,000 organizations that have received funding from Alphabet Soup over the years.


## Results: Using bulleted lists and images to support your answers, address the following questions.

   - Data Preprocessing

     - My model used the `y = application_df.IS_SUCCESSFUL`, since we are checking if the applicant was successful if funded by Alphabet Soup.

     - My model used the `X = application_df.drop(columns="IS_SUCCESSFUL")` as the feature.

     - I dropped the EIN and NAME columns as they were not useful for this model.

   - Compiling, Training, and Evaluating the Model

     - I selected layers one 100 neurons, two 80 neurons, four 30 neurons, and five 10 neurons.  Layers one, and two are ReLU activation.  With layers four, and five as Sigmoid activation.  These were finaly selected after some trial and error to determine the best accuracy and performance.  The accurace improved to 72.7% and the taking 377ms/epoch.

     - I was not able to achieve the target model performance as I went from an accuracy of 72.42% to 72.70%

     - The small amount of accuracy increase was done by changing the number of neurons in each layer and also adding and removing layers, while also removing additional columns and trying different configurations.  My final attempt was the best attempt that I had recieved.  Below are the images of the unoptimized and optimized models.

![This is an image](https://github.com/BMoreland20/Neural_Network_Charity_Analysis/blob/main/Resources/unoptimized_model.2.png)

![This is an image](https://github.com/BMoreland20/Neural_Network_Charity_Analysis/blob/main/Resources/optimized_model.2.png)

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.