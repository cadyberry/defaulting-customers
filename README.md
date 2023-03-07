# defaulting-customers
This project uses a data set of  175,425 records to predict defaulting customers. Two classification and regression tree (CART) models were created and used to classify default status using four explanatory variables: interest rate, loan amount, installment, and term. One CART model does not account for misclassification costs (Naive model) and the other CART model (3.3x) does account for data-driven misclassification costs. 

 Baseline models were constructed. Accuracy, error rate, sensitivity specificity, Fβ scores and model costs were calculated for each model. Notable conclusions from analysis are as follows:


•	The 3.3x CART model can positively identify a defaulting customer better than the Naïve CART model (11.74%), with a sensitivity 6.24 times greater at 73.29%. 

•	The 3.3x CART model reduced the number of false negatives by 70%, from 20,050 (Naive model) to 6069 (3.3x model).

•	The 3.3x CART mode produced the greatest revenue at $455.11 per customer and a total revenue of $63,341,910.

•	Decision Tree rules:

        o	If interest rate is less than 11.75%, then an applicant is classified as non-default, with 37% support, and 64% confidence.

        o	If interest rate is greater than 17.12%, then an applicant is classified as default, with 27% support, and 72% confidence.

        o	If interest rate is less than 17.12%, but more than 14.23%, then an applicant is classified as default, with 16% support, and 61% confidence.

        o	If interest rate is less than 14.23% but the installment is more than $170.69, an applicant is classified as then default, with 17% support, and 55% confidence.

        o	If interest rate is less than 14.23% and the installment is less than $170.69 then an applicant is classified as non-default, with 2% support, and 56% confidence.
        
• The 3.3x CART model is the most profitable model for the bank. 
