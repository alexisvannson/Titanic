# Titanic Survival Prediction

## Objective
The goal of this project is to build predictive models to determine the survival of passengers on the Titanic. The models are trained on a dataset that includes various features such as age, sex, passenger class, and more. The final work is in [titanic_updated.ipynb](https://github.com/alexisvannson/titanic-survival-prediction/blob/main/titanic_updated.ipynb).

## The Dataset
The dataset used in this project is the Titanic dataset, which contains information about the passengers on the Titanic, including whether they survived or not. The dataset can be downloaded from [Kaggle](https://www.kaggle.com/c/titanic/data).

### Columns in the Dataset
- `PassengerId`: Unique identifier for each passenger
- `Survived`: Survival (0 = No, 1 = Yes)
- `Pclass`: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- `Name`: Name of the passenger
- `Sex`: Gender of the passenger
- `Age`: Age of the passenger
- `SibSp`: Number of siblings/spouses aboard the Titanic
- `Parch`: Number of parents/children aboard the Titanic
- `Ticket`: Ticket number
- `Fare`: Passenger fare
- `Cabin`: Cabin number
- `Embarked`: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Project Structure
1. **Data Loading and Exploration**
   - Load the dataset using Pandas.
   - Display the first few rows of the dataset to understand its structure.

2. **Data Preprocessing**
   - Convert categorical variables (`Sex` and `Embarked`) into numerical values.
   - Handle missing values in the `Age`, `Fare`, and `Embarked` columns by filling them with median values.

3. **Correlation Study**
   - Drop columns that are not useful for correlation: `Name`, `Ticket`, `Cabin`.
   - Calculate the correlation matrix for the dataset using the Pandas command: `dataframe.corr()`.
   - Visualize the correlation matrix.
   - Analyze the correlation to identify which variables have the least correlation with the survival status.

4. **Building the Neural Network**
   - Split the dataset into training and testing sets.
   - Define a neural network architecture using a deep learning library such as PyTorch.
   - Train the neural network using the training set.
   - Evaluate the neural network using the testing set.

## Usage
1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/titanic-survival-prediction.git
    cd titanic-survival-prediction
    ```
2. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter Notebook:
    ```bash
    jupyter notebook titanic.ipynb
    ```

### Usage

1. Clone the repository:
    ```sh
    git clone https://github.com/alexisvannson/titanic-survival-prediction.git
    cd titanic-survival-prediction
    ```

2. Create a virtual environment and activate it:
    ```sh
    python -m venv titanicpred
    source titanicpred/bin/activate  # On Windows use `titanicpred\Scripts\activate`
    ```

3. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```
4. Run the Jupyter Notebook:
    ```bash
    jupyter notebook titanic.ipynb
    ```

