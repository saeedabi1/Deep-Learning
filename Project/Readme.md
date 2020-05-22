
Profit maximization from LendingClub  investment.

From Wikipedia: “LendingClub is a US peer-to-peer lending company, headquartered in San Francisco, California.[3] It was the first peer-to-peer lender to register its offerings as securities with the Securities and Exchange Commission (SEC), and to offer loan trading on a secondary market. LendingClub is the world's largest peer-to-peer lending platform.”
 
Lending Club is a company that matches borrowers who are looking for a loan and  investors who lend money and make a profit from return. Borrower submit an application, providing necessary info, like  loan amount, employment info, financial history, loan purpose and etc.. Lending Club evaluates borrower’s credit report information and assigns an interest rate to the loan.
Approved loans are listed on the Lending Club website. Then  investors can select recently approved loans.
My Goal: I will build a model that will predict if a borrower will pay back his/her loan or not based on historical data from Lending Club? As an investor, I would like to maximize my profit selecting loans that will give me the maximum profit.
LendingClub DataSet from Kaggle: https://www.kaggle.com/wordsforthewise/lending-club

I decided to collect only loans from 2018 since we need to use most current data for loan prediction.
After preprocessing and normalizing data, I came up with 87 features . 
This dataset is highly imbalanced:
    Positive: 96.52% 
    Negative  3.48%
We have small fraction of negative samples.
We  want to have the classifier heavily weight the negative examples. You do this by passing Keras weights for every class through a parameter. These will push the model to "pay attention" to samples from an underrepresented class.

I tried to play with different number of layers and different hyperparameters.
The best accuracy(72% ) using  3 hidden layers.
Resampling using SMOTE  did not improve accuracy.

 
