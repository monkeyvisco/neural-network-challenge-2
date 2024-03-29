# Michigan State University College of Engineering AI Boot Camp, in partnership with edX.
# Challenge Assignment

# neural-network-challenge-2

## Contact Info
Author / Quite-Junior-Developer / 20+ yrs Experience 

## Description
The files in this respository, including the Juptyer Notebook file containing the code and commentary, were used to meet the requirements of an AI Boot Camp Challenge Assignment within the curriculum of the Michigan State University College of Engineering AI Boot Camp, in partnership with edX.
https://www.edx.org/boot-camps/ai/michigan-state-university-ai-boot-camp

## Background of Challenge
You are tasked with creating a neural network that HR can use to predict whether employees are likely to leave the company. Additionally, HR believes that some employees may be better suited to other departments, so you are also asked to predict the department that best fits each employee. These two columns should be predicted using a branched neural network.

## Approach to Solving Challenge

### Prepare the data for use on a neural network model.
To start, the script checks null values and zeros, datatypes.
It also displays value counts for our y, dataframe shape, and column names.
A correlation matrix is developed and displayed to enable the user to perform t-tests to evaluate if the featuure's means are statistically different.
The user can drop a column in a pair of means which exhibit no statistical difference.
As well, the user can drop other columns.  In the example, we chose to drop three features with low standard deviations.  This resulted in a modest improvement in accuracy.
The code splits the preprocessed data into features (X) and target(y) datasets.
It then splits the features and target datasets into training and testing datasets.
Data contains only numererical data.  There is no encoding function for categorical data in the script.
The script uses scikit-learn's StandardScaler to scale the features data.

### Compile and evaluate a model using a neural network.
The code creates a deep neural network by assigning number of input features, number of layers, number of neurons on each leayer suing Tensorflow's Keras.
It initiates a sequential neural network model and define up to 3 hidden layers, capable of accepting standard activation functions.
It compiles and fits the model using the binary_crossentropy loss function, the adam optimizer, and the accuracy evaluation metric.
The user can view test data.  This helps with evaluating the models loss and accuracy, which are displayed.
The code can then save and export the model to a keras file.

### Predict loan repayment success by using your neural network model.
The coad reloads our model and make predicitons on the testing data, saving predictions to a DataFrame.
It can then display a classification report with the y test data and predictions.

## Challenge Q&A - My answers to the three questions below can be at the end of the Jupyter Notebook.

### 1. Describe the data that you would need to collect to build a recommendation system to recommend student loan options for students. Explain why this data would be relevant and appropriate.

### 2. Based on the data you chose to use in this recommendation system, would your model be using collaborative filtering, content-based filtering, or context-based filtering? Justify why the data you selected would be suitable for your choice of filtering method.

### 3. Describe two real-world challenges that you would take into consideration while building a recommendation system for student loans. Explain why these challenges would be of concern for a student loan recommendation system.

# ALSO ...

## Editing this README
When you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.

## Roadmap
There are no plans for releases in the future.

## Contributing
I am open to contributions with improve the codes functionality and 'descriptiveness in the sense of education'.
One way you can help is add to this read me by describing how people can get started and make changes to the project.

## Support
No support is currently available for this project.

## Authors and acknowledgment
Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template, and to Seth who shared it with me.
We appreciate the help of AI ChatGPT tools to aid in rapid understanding of syntax for code we knew the purpose for, but that we did not a good grasp on syntax.
We also appreciate the educational support of all the professionals enabling a whole lot of learning through this challenge and the boot camp.
