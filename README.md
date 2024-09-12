

# Student Loan Risk with Deep Learning


## Prepare the data to be used on a neural network model
### Step 1: Read the `student-loans.csv` file into a Pandas DataFrame. Review the DataFrame, looking for columns that could eventually define your features and target variables.   
### Step 2: Using the preprocessed data, create the features (`X`) and target (`y`) datasets. The target dataset should be defined by the preprocessed DataFrame column “credit_ranking”. The remaining columns should define the features dataset.
### Step 3: Split the features and target sets into training and testing datasets.
### Step 4: Use scikit-learn's `StandardScaler` to scale the features data.

## Compile and Evaluate a Model Using a Neural Network
### Step 1: Create a deep neural network by assigning the number of input features, the number of layers, and the number of neurons on each layer using Tensorflow’s Keras.
### Step 2: Compile and fit the model using the `binary_crossentropy` loss function, the `adam` optimizer, and the `accuracy` evaluation metric.
### Step 3: Evaluate the model using the test data to determine the model’s loss and accuracy.
### Step 4: Save and export your model to a keras file, and name the file `student_loans.keras`.

## Predict Loan Repayment Success by Using your Neural Network Model
### Step 1: Reload your saved model.
### Step 2: Make predictions on the testing data and save the predictions to a DataFrame.
### Step 4: Display a classification report with the y test data and predictions

## Discuss creating a recommendation system for student loans

**1. Describe the data that you would need to collect to build a recommendation system to recommend student loan options for students. Explain why this data would be relevant and appropriate.**

 - This model will need data in three main categories: 
    - Student Financial (payment history, credit rating/credit score, financial aid score, finance workshop score): This would be the most critical data to predict ability to pay. 
    - Student Academic Profile (stem degree score, gpa, ranking, time to completion): This data could help to provide a more complete picture- certain fields of study may have higher earnings potential, especially with STEM. Academic performance could also be a predictor of repayment behavior. 
    - Student Demographic (location): understanding cost-of-living in the student's area can also be relevant to loan decisions.

**2. Based on the data you chose to use in this recommendation system, would your model be using collaborative filtering, content-based filtering, or context-based filtering? Justify why the data you selected would be suitable for your choice of filtering method.**

- This model would primarily use content-based filtering. The data collected (credit ranking, GPA, financial aid, major) provides specific traits that can be matched with appropriate loan options. There are some context-based features such as alumni success and financial workshop scores that could contribute to the model's performance, but not enough for context-based filtering to be the primary.  

**3. Describe two real-world challenges that you would take into consideration while building a recommendation system for student loans. Explain why these challenges would be of concern for a student loan recommendation system.**

- If a loan decision is made uweighting too heavily on academic profile as part of the data, it could present a risk. There could be a potential lag in the student academic profile if circumstances change, such as a change of major, withdrawal/drops. There is also a dependency on the institution to provide data, which can add complexity.

- There are potential risks of bias with the model. Students from wealthier areas might receive better loan terms due to higher credit rankings or financial aid scores. This could lead to inequities where students from disadvantaged backgrounds receive less favorable recommendations.