# neural-network-challenge-2

Module 19 Challenge
Due Mar 25 by 11:59pm Points 100 
Background
You are tasked with creating a neural network that HR can use to predict whether employees are likely to leave the company. Additionally, HR believes that some employees may be better suited to other departments, so you are also asked to predict the department that best fits each employee. These two columns should be predicted using a branched neural network.

Repository: neural-network-challenge-2
Google Colab code: attrition.ipynb

Part 1: Preprocessing
Import the data and view the first five rows.
Determine the number of unique values in each column.
Create y_df with the attrition and department columns.
Create a list of at least 10 column names to use as X data. You can choose any 10 columns you’d like EXCEPT the attrition and department columns.
Create X_df using your selected columns. Show the data types for X_df.
Split the data into training and testing sets.
Convert your X data to numeric data types however you see fit. 
Add new code cells as necessary. 
Make sure to fit any encoders to the training data, and then transform both the training and testing data.
Create a StandardScaler, fit the scaler to the training data, and then transform both the training and testing data.
Create a OneHotEncoder for the department column, then fit the encoder to the training data and use it to transform both the training and testing data.
Create a OneHotEncoder for the attrition column, then fit the encoder to the training data and use it to transform both the training and testing data. 
Part 2: Create, Compile, and Train the Model
Find the number of columns in the X training data.
Create the input layer. Do NOT use a sequential model, as there will be two branched output layers.
Create at least two shared layers.
Create a branch to predict the department target column. Use one hidden layer and one output layer.
Create a branch to predict the attrition target column. Use one hidden layer and one output layer.
Create the model.
Compile the model.
Summarize the model.
Train the model using the preprocessed data.
Evaluate the model with the testing data.
Print the accuracy for both department and attrition. 
Part 3: Summary
Briefly answer the following questions in the space provided:
Is accuracy the best metric to use on this data? Why or why not?
What activation functions did you choose for your output layers, and why?
Can you name a few ways that this model could be improved? 

Hints and Considerations
Review previous modules if you need help with data preprocessing. Make certain that your training and testing data are preprocessed in the same ways. 
Scoring

Preprocessing (40 points)
Import the data. (5 points) Create y_df with the attrition and department columns. (5 points) Choose 10 columns for X. (5 points) Show the data types of the X columns. (5 points) Split the data into training and testing sets. (5 points) Encode all X data to numeric types. (5 points) Scale the X data. (5 points) Encode all y data to numeric types. (5 points) 
Model (40 points)
Find the number of columns in the X training data. (5 points) Create an input layer. (5 points) Create at least two shared hidden layers. (10 points) Create an output branch for the department column. (10 points) Create an output branch for the attrition column. (10 points) 
Summary (20 points)
Answer the questions briefly. (10 points) Show understanding of the concepts in your answers. (10 points)


Michigan State University College of Engineering AI Boot Camp, in partnership with edX.
Challenge Assignment
neural-network-challenge-1
Description
The files in this respository, including the Juptyer Notebook file containing the code and commentary, were used to meet the requirements of an AI Boot Camp Challenge Assignment within the curriculum of the Michigan State University College of Engineering AI Boot Camp, in partnership with edX. https://www.edx.org/boot-camps/ai/michigan-state-university-ai-boot-camp

Background of Challenge
You work at a company that specializes in student loan refinancing. If the company can predict whether a borrower will repay their loan, it can provide a more accurate interest rate for the borrower. Your team has asked you to create a model to predict student loan repayment.

The business team has given you a CSV file that contains information about previous student loan recipients. With your knowledge of machine learning and neural networks, you decide to use the features in the provided dataset to create a model that will predict the likelihood that an applicant will repay their student loans. The CSV file contains information about these students, such as their credit ranking.

Approach to Solving Challenge
Prepare the data for use on a neural network model.
To start, the script checks null values and zeros, datatypes. It also displays value counts for our y, dataframe shape, and column names. A correlation matrix is developed and displayed to enable the user to perform t-tests to evaluate if the featuure's means are statistically different. The user can drop a column in a pair of means which exhibit no statistical difference. As well, the user can drop other columns. In the example, we chose to drop three features with low standard deviations. This resulted in a modest improvement in accuracy. The code splits the preprocessed data into features (X) and target(y) datasets. It then splits the features and target datasets into training and testing datasets. Data contains only numererical data. There is no encoding function for categorical data in the script. The script uses scikit-learn's StandardScaler to scale the features data.

Compile and evaluate a model using a neural network.
The code creates a deep neural network by assigning number of input features, number of layers, number of neurons on each leayer suing Tensorflow's Keras. It initiates a sequential neural network model and define up to 3 hidden layers, capable of accepting standard activation functions. It compiles and fits the model using the binary_crossentropy loss function, the adam optimizer, and the accuracy evaluation metric. The user can view test data. This helps with evaluating the models loss and accuracy, which are displayed. The code can then save and export the model to a keras file.

Predict loan repayment success by using your neural network model.
The coad reloads our model and make predicitons on the testing data, saving predictions to a DataFrame. It can then display a classification report with the y test data and predictions.

Challenge Q&A - My answers to the three questions below can be at the end of the Jupyter Notebook.
1. Describe the data that you would need to collect to build a recommendation system to recommend student loan options for students. Explain why this data would be relevant and appropriate.
2. Based on the data you chose to use in this recommendation system, would your model be using collaborative filtering, content-based filtering, or context-based filtering? Justify why the data you selected would be suitable for your choice of filtering method.
3. Describe two real-world challenges that you would take into consideration while building a recommendation system for student loans. Explain why these challenges would be of concern for a student loan recommendation system.
ALSO ...
Editing this README
When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to makeareadme.com for this template.

Roadmap
There are no plans for releases in the future.

Contributing
I am open to contributions with improve the codes functionality and 'descriptiveness in the sense of education'. One way you can help is add to this read me by describing how people can get started and make changes to the project.

Support
No support is currently available for this project.

Authors and acknowledgment
Thank you to makeareadme.com for this template, and to Seth who shared it with me. We appreciate the help of AI ChatGPT tools to aid in rapid understanding of syntax for code we knew the purpose for, but that we did not a good grasp on syntax. We also appreciate the educational support of all the professionals enabling a whole lot of learning through this challenge and the boot camp.
