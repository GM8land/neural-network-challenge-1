

## Module 18 Challenge: Student Loan Risk with Deep Learning
### Instructions:
You work at a company that specializes in student loan refinancing. If the company can predict whether a borrower will repay their loan, it can provide a more accurate interest rate for the borrower. Your team has asked you to create a model to predict student loan repayment.

The business team has given you a CSV file that contains information about previous student loan recipients. With your knowledge of machine learning and neural networks, you decide to use the features in the provided dataset to create a model that will predict the likelihood that an applicant will repay their student loans. The CSV file contains information about these students, such as their credit ranking.
Open the starter file in Google Colab and complete the following steps, which are divided into four parts:

- Prepare the data for use on a neural network model.

- Compile and evaluate a model using a neural network.

- Predict loan repayment success by using your neural network model.

- Discuss creating a recommendation system for student loans.

### Requirements
- Prepare the Data for Use on a Neural Network Model (15 points)
  - Two datasets were created: a target (y) dataset, which includes the "credit_ranking" column, and a features (X) dataset, which includes the other columns. (5 points)

  - The features and target sets have been split into training and testing datasets. (5 points)

  - Scikit-learn's StandardScaler was used to scale the features data. (5 points)

- Compile and Evaluate a Model Using a Neural Network (30 points)
  - A deep neural network was created with appropriate parameters. (10 points)

  - The model was compiled and fit using the accuracy loss function, the adam optimizer, the accuracy evaluation metric, and a small number of epochs, such as 50 or 100. (10 points)

  - The model was evaluated using the test data to determine its loss and accuracy. (5 points)

  - The model was saved and exported to a keras file named student_loans.keras. (5 points)

- Predict Loan Repayment Success by Using your Neural Network Model (25 points)
  - The saved model was reloaded. (5 points)

  - The reloaded model was used to make binary predictions on the testing data. (10 points)

  - A classification report is generated for the predictions and the testing data. (10 points)

- Discuss creating a recommendation system for student loans (30 points)
  For Question 1:

  - The response describes the data that should be collected to build a recommendation system for student loan options. (4 points)

  - The response explains why they think that data should be collected. (4 points)

  - The type of data described is appropriate for a recommendation system for student loan options. (2 points)

For Question 2:

  - The response chose a filtering method. (4 points)

  - The student justified the choice of their filtering method. (4 points)

  - The choice of filtering method was appropriate for the data selected in the previous question. (2 points)

For Question 3:

  - The response lists two real-world challenges with building a recommendation system for student loans. (4 points)

  - The response explains why these challenges would be of concern for a student loan recommendation system. (6 points)


### Discuss creating a recommendation system for student loans

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

### Grade: 100
### Grader Feedback: 
Great work Geoff!



You did an excellent job preparing the data for use in a neural network model. 



The datasets were correctly created, with the target set including the "credit_ranking" column and the features set containing the other columns. You also split the data into training and testing sets and used Scikit-learn's StandardScaler to scale the features, which was done efficiently, earning full marks in that section.



In compiling and evaluating the model, you created a deep neural network with appropriate parameters, used the right loss function, optimizer, and evaluation metric, and trained the model with a reasonable number of epochs. You evaluated the model using the test data and successfully determined the loss and accuracy. Additionally, you saved and exported the model correctly, completing this section well and earning full marks.



For the prediction section, you reloaded the saved model and used it to make binary predictions on the testing data. You also generated a classification report, demonstrating your understanding of how to evaluate the model’s performance on new data. This section was thoroughly completed, and you received full marks here as well.



In discussing the recommendation system for student loans, you provided a comprehensive response to all three questions. You identified the relevant data categories for the recommendation system, financial, academic, and demographic, and justified why this data would be essential. You appropriately chose content-based filtering for the model, clearly explaining why it was the best fit for the data you selected. Your response to the challenges was thoughtful, addressing potential issues like bias and dependency on academic profile data. This section was well-structured, and you showed strong reasoning throughout.



Overall, this was a phenomenal submission, and you earned full marks across all sections. The work was thorough, clear, and demonstrated a deep understanding of neural networks and recommendation systems. Please do give yourself a pat on the back.
Central Grader , Sep 12, 2024 at 6:32pm
