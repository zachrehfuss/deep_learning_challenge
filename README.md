# deep_learning_challenge

What is Located in this Repository
- Located in this repository you will find three jupyter
notebooks and a folder titled Models. The Jupyter notebook
titled "Starter_Code" houses the code I created to run my 
first model and preprocessing the data. The jupyter notebook
titled "AlphabetSoupCharity_Optimization" houses the code I 
created to tinker with my model and run different versions of
the neural network. The final jupyter notebook titled
"Running_files" houses code that will show a summary of how to
recreate each of my models and the various versions of it that
I ran. All hidden layers in the models were using the relu
relu activation function and all of the output layer use a 
sigmoid function as they are binary classifiers. I did not
tinker with how I compiled the data and the models were all
trained with 50 epochs. In the Models folder you will find
all of the h5 files for my models with the summary displayed.

How this Code was created
- My instructor Thomas helped debug an issue I was running
into with my X and y variables not being able to be scaled.
He also showed me how to use tensorflow to read H5 files.
I used the Xpert learning assistant to fix my syntax
for finding a cutoff and how to replace the value 
in the dataframe.

Model Report

Overview
I was tasked to create a model that predicts whether or not applicants who are funded by our company would be successful. Once I had created the model, I wanted to maximize its accuracy by running it through multiple optimizations to try and be as accurate as possible. 
Results
Data Preprocessing
The variable that was the target of my model was whether or not the applicant was successful. This was the dependent variable that relied on the rest of the variables to determine its outcome.
The features of my model were 43 variables which included, the type of application, total cost of the loan, income bracket of the applicant, and what the money is being used for. 
The variables that should be removed are the name and EIN columns as the names of the applicants and how they are identified are not relevant.

Training and Evaluating Model
I ultimately landed on 34 neurons, 4 layers, and I used relu as my activation functions for all of my hidden layers. I landed on these settings as I had previously tried multiple different combinations of neurons, some greater than 34 and some less than 34. I tried increasing layers to 5 and decreasing it to 3 but this was the best combination for the model. The accuracy for the model came in at 72.9%. I was unable to achieve the target model performance of 75% and ultimately it was my 2nd attempt at optimizing the model that was the best. 
Summary
Overall the model came very close to the target goal. I think the model could reach the 75% if a keras tuner was used or if more time was spent tinkering with the makeup of the model. A logistic regression model may be better suited to handle this data as it is used as a binary classifier as well and works really well with data like we used to train our model. As this model currently exists, I would not use it as being unable to accurately predict if at least 3 out of every 4 applicants will be successful is too risky in my opinion. 
