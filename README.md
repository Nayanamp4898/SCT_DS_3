task 3
build a decision classifier whether a customer will purchase a product or service based on their demographic and behavioral data

Steps:
Preprocess Data:

Convert categorical variables into numerical format.
Handle missing or irrelevant data if any.
Split Data:

Divide the dataset into training and testing sets.
Train a Decision Tree Model:

Use the DecisionTreeClassifier from sklearn.
Visualize the Decision Tree.

Key Features and Conditions:
Duration:

The most critical factor is the call duration (duration):
Short calls (duration ≤ 561 seconds) are often associated with customers who are less likely to buy.
Longer calls (duration > 561 seconds) significantly increase the likelihood of purchase.
Age:

Younger customers (e.g., age ≤ 20) and much older customers (e.g., age > 70) tend to be less likely to buy.
Middle-aged customers, particularly between 30–60 years, have a higher likelihood depending on other factors.
Previous Contact and Outcome:

Customers with a successful prior campaign outcome (poutcome) are more likely to buy, especially if they've been contacted recently (pdays ≤ 22).
If previous campaigns have been unsuccessful or if the customer has never been contacted, they are less likely to buy.
Marital Status:

Marital status can influence purchase behavior:
For some branches, married customers show higher purchase likelihood, depending on other factors.
Other Influences:

Features like pdays, month, and campaign frequency have smaller but noticeable impacts in the decision tree.
General Conclusion:
Customers are more likely to buy if:

The call duration is long (indicating interest or engagement).
They have a positive history with previous campaigns.
They are contacted in a timely manner following previous interactions.
Customers are less likely to buy if:

The call is short.
They have not been successfully engaged in past campaigns.
They fall into specific age ranges (e.g., very young or elderly).
