
Business Case: The objective is to grasp how information can be effectively utilized to decrease the likelihood of losing money when offering loans to clients.
Financial Risk Detection Business Case: The objective is to grasp how information can be effectively utilized to decrease the likelihood of losing money when offering loans to clients. Introduction: This study aims to give you an idea of applying EDA in a real business scenario. In this study, apart from applying the techniques that we have learnt in the EDA module, we will also develop a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers. Business Understanding: The loan providing companies find it hard to give loans to the people due to their insufficient or non-existent credit history. Because of that, some consumers use it as their advantage by becoming a defaulter. Suppose you work for a consumer finance company which specialises in lending various types of loans to urban customers. You have to use EDA to analyse the patterns present in the data. This will ensure that the applicants capable of repaying the loan are not rejected. When the company receives a loan application, the company has to decide for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision: * If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company * If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company. The data given below contains the information about the loan application at the time of applying for the loan. It contains two types of scenarios: The client with payment difficulties: he/she had late payment more than X days on at least one of the first Y instalments of the loan in our sample, All other cases, All other cases when the payment is paid on time. When a client applies for a loan, there are four types of decisions that could be taken by the client/company):

Approved: The Company has approved loan Application
Cancelled: The client cancelled the application sometime during approval. Either the client changed her/his mind about the loan or in some cases due to a higher risk of the client he received worse pricing which he did not want.
Refused: The company had rejected the loan (because the client does not meet their requirements etc.).
Unused offer: Loan has been cancelled by the client but on different stages of the process. In this case study, you will use EDA to understand how consumer attributes and loan attributes influence the tendency of default.
Business Objectives: This case study aims to identify patterns which indicate if a client has difficulty paying their instalments which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc. This will ensure that the consumers capable of repaying the loan are not rejected. Identification of such applicants using EDA is the aim of this case study.In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.To develop your understanding of the domain, you are advised to independently research a little about risk analytics - understanding the types of variables and their significance should be enough). Dataset Details: This dataset has 3 files as explained below:

'application_data.csv' contains all the information of the client at the time of application. The data is about whether a client has payment difficulties.

'previous_application.csv' contains information about the client’s previous loan data. It contains the data whether the previous application had been Approved, Cancelled, Refused or Unused offer.

'columns_description.csv' is data dictionary which describes the meaning of the variables.

Approach Taken:

In Application dataset there are 307511 rows and 122 columns.
Columns that have missing values more than 40% are dopped as columns with that much of missing values may not be helpful to depict the insight. After dropping such columns, there are 73 columns in the dataset.
It can be seen for days columns; the values are in negative so we those were converted into positive values.
There are few columns having integer types but contains categorical data. Converting these columns into data type object is required to perform univariate and bivariate analysis properly. We checked columns having less unique values and converted those columns into object type.
Then outlier detection, univariate analysis, bivariate analysis, correlation analysis are performed.
Application data has been divided into two datasets one where TARGET=1 (client with payment difficulties) and one where TARGET=0 (Other clients).
For Previous Application data same analysis has been performed.
By using machine learning algorithms we bulid a model and evaluate it.
At the end Conclusion, Important insights are provided.

