## supervised-ML

## Project description:
### Predicting Credit Risk.

### Data retrieved from:
* LendingClub (2019-2020) Loan Stats https://resources.lendingclub.com/.

### Credit Risk Evaluator.ipynb

#### Data Preprocessing
* Training set was created from the 2019.
* Testing set was created from the 2020.
* Categorical variables hot encoded using pd.get_dummies().
* Testing data was ajusted to train data as categories were missing in the testing set.

#### Models Consideration
* Logistic Regression, and Random Rorests classifier were created and fited to the data and scored.
* Compared Model results on scaled Data (using StandardScaler). 
