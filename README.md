# Project Name
Lending Club Loan Risk Analysis



## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information


## Business Understanding
The case study id for a consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:

If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company

If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company

The data given below contains information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

When a person applies for a loan, there are two types of decisions that could be taken by the company:

Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:

Fully paid: Applicant has fully paid the loan (the principal and the interest rate)

Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 

Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)


### Business Objectives
This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. 

Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 

If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment. 

To develop your understanding of the domain, you are advised to independently research a little about risk analytics (understanding the types of variables and their significance should be enough).

In this case study, EDA is used to understand how consumer attributes and loan attributes influence the tendency of default.

### Data Understanding

The dataset contains the complete loan data for all loans issued through the time period 2007 t0 2011.


## Conclusions

#### Higher Interest Rate and Longer Term together contributes towards default of loan. Lending Club(LC) should try to give lower interest rate with longer term or Higher Interest Rate with Shorter Term.

#### LC should be cautious approving new loans with applicants having more than 50% of Revolving Credit Utilization.
#### LC should recalculate the DTI column after including the current loan installment and mortgage payment amount.
#### LC should consider the Purpose of the Loan, State and ZipCode before approving. Specific location and purpose have higher Default Rate.
#### Combination of 8 attributes (i.e. delinq_2yrs, inq_last_6mths, pub_rec_bankruptcies,int_rate,revol_util,revol_bal,installment,dti) indictates towards High Risk of Default.



## Technologies Used
Python 3.9
Libraries: 
numpy
pandas
matplotlib
seaborn
warnings
scipy
warnings.filterwarnings("ignore")


## Acknowledgements

- Sandip Mahato as Partner


## Contact
Created by [@sghoshca] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->