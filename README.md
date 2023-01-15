# A-GNN-APPROACH-TO-DETECTING-AUTOMOBILE-INSURANCE-FRAUD
Insurance claim fraud reduces earnings and causes significant losses in the vehicle insurance industry. As a result, various machine learning algorithms such as Nave Bayes, Bayesian, Network model, and others have been implemented to detect financial fraud; however, none of these approaches have been tested on a graph dataset. The goal of this study is to develop a Graph neural network for a node classification strategy to detect automobile insurance fraud. An automobile insurance dataset was pre-processed, and a comprehensive exploratory analysis was performed to reveal insights, the data was found to be imbalanced. The table dataset was transformed into a graph dataset to be used with the GNN model. The imbalance state of the graph dataset was rectified by sampling before utilizing it to create a model. Using an 80/20 approach, the graph dataset was divided into training and testing datasets. Training sets were used to train models, and testing sets were used to evaluate their performance. Precision, recall, and the F-measure evaluation technique is used to confirm that the model is fit.

Vehicle Insurance Fraud Detection Dataset

Source:https://www.kaggle.com/datasets/khusheekapoor/vehicle-insurance-fraud-detection

The dataset has 32 features in total, of which there are 25 category features, 6 ordinal features, and one class variable with the label "fraud" or "not-fraud." Only 923 records, out of its 15,420 total records are false.

For data transformation, each column in the relational table is categorised into one of the following three types:

Identity columns – columns that include user or transaction-specific identity data, such as IP addresses, phone numbers, and device identifiers. In the heterogeneous network, these column types are transformed into node types, and the entries in these columns act as nodes.

Categorical columns – columns that are associated with categorical characteristics, such as a user's age range or whether or not a given address is consistent with an address already on file. Numerical feature modification is applied to the items in these columns before they are used as node attributes in the homogeneous graph.

Numerical columns – columns with numerical characteristics, like the quantity of times a user has attempted a transaction. In the heterogeneous graph, the entries in this table are also used as node characteristics. The script makes the assumption that all table columns that aren't identity or category columns are numerical columns.
