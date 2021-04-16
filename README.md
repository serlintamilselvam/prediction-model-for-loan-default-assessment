# Prediction model for loan default assessment

### DataSet

Data available at <a href="https://drive.google.com/file/d/1Bgvky1gxY-bQqiRUX3-GOBGwezhU0tba/view?usp=sharing">Google Drive.</a>

## Implementation in Python:

1. Prediction model is developed using Gradient Boosting classifier. The conceptual idea behind this classifier is to pick an algorithm and make tweaks to it with various regularization schemes, this process improves the learning ability of the model in a gradual and additive fashion. This classifier is particularly effective at classifying complex dataset such as Banking and Financing.

2. The results predicted by model on the probability a customers will default on their loan repayment is accurate ~76% of the time (this is validated against a pre-defined validation dataset fed into the model during the train/test phase).

3. Model identified a potential set of customers who maintains a significant account balance and has regular intervals of credit transactions on their account, has high probability of loan repayment. The customers with less account transactions and maintains a very low account balance for a significant time before the loan request date, has a high probability of loan defaulting. The model is also capable of adjusting the prediction parameters of its features based on the future dataset fed into it.

4. In total 21 features are extracted from the provided dataset which yields maximum accuracy from model. The features are as follows:
<ul>
	<li>Total number of credit transactions</li>
	<li>Average amount credited to the account</li>
	<li>Total number of debit transactions</li>
	<li>Average amount debited from the account</li>
	<li>Requested loan amount</li>
	<li>Total amount of all credit transactions</li>
	<li>Days between loan request and account transactions</li>
	<li>Current balance in the customer’s account</li>
	<li>Loan request date</li>
	<li>Total amount of all debit transactions</li>
</ul>

5. The idea behind choosing these particular features is to train the prediction model on the bank’s existing customers transactional behavior and their loan outcomes, So that any potential loan seekers can be evaluated and risk-assessed primarily based on their transactional history.

### Accuracy
The accuracy of the model is 76%

## Contributors:

1. <a href="https://github.com/BhuvaneshRavi" target="_blank">Bhuvaneshwaran Ravi</a>
2. <a href="https://github.com/serlintamilselvam" target="_blank">Serlin Tamilselvam</a>