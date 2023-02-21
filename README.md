# deep-learning-challenge

**Background**

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

**Overview**

The purpose of the analysis is to create a binary classifier, using the features in the given dataset, that can predict whether the applicants will be successful if funded by the Alphabet Soup.
Analyzed using the neural network model and based on the accuracy, further adjustments are made to optimize the performance of the model.
Results

**Data Preprocessing**

•	The target variable in the model is 'IS_SUCCESSFUL.'

•	 Dropping NAME and EIN ,below are the features used in the initial analysis of the model.
1.	APPLICATION_TYPE
2.	AFFILIATION
3.	CLASSIFICATION
4.	USE_CASE
5.	ORGANIZATION
6.	STATUS
7.	INCOME_AMT
8.	SPECIAL_CONSIDERATIONS
9.	ASK_AMT

•	 For Optimizing the model made some adjustments by adding and removing few features.
1.	STATUS-it had 34294 number of 1’s and 5 in number of 0’s.
2.	SPECIAL_CONSIDERATIONS-it had 34272 number of N values and 27 Y values.

![Values](https://user-images.githubusercontent.com/112193116/220407878-c572bc70-fdfa-4826-adc0-3e527ad57293.jpg)

The above two features were removed and added NAME feature

So, the final model had the following features.
1.	NAME
2.	APPLICATION_TYPE
3.	AFFILIATION
4.	CLASSIFICATION
5.	USE_CASE
6.	ORGANIZATION
7.	INCOME_AMT
8.	ASK_AMT

**Compiling, Training, and Evaluating the Model**

•	The initial analysis had 2 layers, with 80 neurons in first hidden layer and 30 neurons in the second hidden layer. The model used two different activation functions- relu and sigmoid.

![Initial_Analysis](https://user-images.githubusercontent.com/112193116/220407867-f0bd2ae9-60a3-4780-82f5-91bb35c00d47.jpg)

•	The target predictive accuracy was 73%

![Initial_Accuracy](https://user-images.githubusercontent.com/112193116/220409773-35ce6691-7b25-4e1a-942f-a967333c1702.png)
 
•	In order to increase the performance, further adjustments were made to optimize the model by removing the features “STATUS” and “SPECIAL_CONSIDERATIONS“ and added the feature “NAME”.
•	Created binning for the rare occurrences in the columns “AFFLIATION “and “NAME”.

![Affliation](https://user-images.githubusercontent.com/112193116/220407863-8f9c6b23-f14c-47c7-ab4e-88b45ddb72d0.jpg)

![Name](https://user-images.githubusercontent.com/112193116/220407873-ca4b96bf-ae48-4b13-8791-7b159781fab7.jpg)

•	Added more neurons to the hidden layers.
•	Used 3rd hidden layer.
•	Used different activation functions for the hidden layers.

![Optimized](https://user-images.githubusercontent.com/112193116/220407876-455e0cfd-b525-4adb-8ba0-54d745d5dfde.png)

•	The model exceeded the target performance of 75%.

![Accuracy](https://user-images.githubusercontent.com/112193116/220407860-178caf01-2917-4070-bc88-d53e68745500.png)
 

**SUMMARY**

The initial model could achieve the accuracy of 73%.To further improve the accuracy, the model was optimized and reached an accuracy of79%.This was achieved by considering the NAME column and adding binning to them, removing the SPECIAL_CONSIDERATIONS and STATUS columns as there were more variability in the values and finally adding more number of neurons, 3rd hidden layer and changing the activation functions.
As per the requirement, I tried using Logistic Regression and Random Forest Classifier to predict the accuracy and was able to get 78% accuracy in both the models.

![LogicalRegression](https://user-images.githubusercontent.com/112193116/220407872-3a47c11c-839e-40ce-846e-be2b55522c44.png)

![Randomforest](https://user-images.githubusercontent.com/112193116/220407877-51ac4fe4-60e8-4d17-b4b3-7c2178f669a7.png)

 
 


 

  
