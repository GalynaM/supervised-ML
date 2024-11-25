## Project predicts whether a loan from LendingClub will become high risk or not

### Using Supervised Mashine Learning project classifies the risk level of given loans using Logistic Regression Model and Random Forest Classifier

### Data retrieved from:
* LendingClub (2019-2020) Loan Stats https://resources.lendingclub.com/.

### Libraries used
* pandas, numpy
* sklearn: StandardScaler, LogisticRegression, RandomForestClassifier, GridSearchCV

### Project Location
* Credit Risk Evaluator.ipynb
  
### Project Description
#### Data Preprocessing
* Training set was created from the 2019 loans.
* Testing set was created from the 2020 loans.
* Categorical variables was encoded using pd.get_dummies().
* Before encoding
* ![image](https://github.com/user-attachments/assets/7cc5b1a3-ad2f-465f-88ef-341692e8d168)
* After encoding
* ![image](https://github.com/user-attachments/assets/636cbefd-06a2-46c9-a04d-8b0aecfd2dde)
* To create train set, target feature was separated.
* Testing data was ajusted to train data as categories were missing in the testing set.

#### Models Consideration
* Predictions on what type of Model will perform better:
  - LR will do worse on unscaled data because features values range is too wide;
  - Random Forest (RF) being an ensemble-based learning algorithm should do better as it will form number of trees to get clearer model and weighs certain features more important than others.
* Logistic Regression, and Random Rorests classifier were created and fited to the data and scored.
  - LR scored 0.547.
  - RF scored 0.644.
  - As we predicted RF scored better than LR on unscaled data.
* Compared Model results on scaled Data (using StandardScaler).
  - LR perfromed better on scaled data as it was expected - 0.66 comparing to 0.575
  - RF scored less on scaled data - 0.56 vs 0.648, so as expected it did not improve, but event went lower.
