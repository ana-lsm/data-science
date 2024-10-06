# Predicting Health Care Costs

This project is from [Datacamp](https://www.datacamp.com), but the dataset was made available by [Keith Galli](https://github.com/KeithGalli/Regression-Example) in his GitHub repository.

Here, I present my process for investigating and cleaning a dataset, as well as performing exploratory data analysis (EDA). I explain my conclusions and insights throughout the analysis.

## Tools I used:

- Jupyter Notebook (within VS Code)
- Python 3.12
- Pandas 2.2.3
- Seaborn 0.13.2
- Scikit-learn 1.5.2

## My biggest difficulties:

While cleaning the data, I encountered a problem with the `sex` column, where I needed to standardize the observations to _male_ and _female_. I overcame this issue by creating a map with a dictionary and using the `.replace()` method in the respective column. _ChatGPT 4.0_ assisted with this solution, as well as with other syntax and debugging problems along the way.

## Dataset summary and our goals for this project

#### insurance.csv

| Column     | Data Type | Description                                                              |
| ---------- | --------- | ------------------------------------------------------------------------ |
| `age`      | int       | Age of the primary beneficiary.                                          |
| `sex`      | object    | Gender of the insurance contractor (male or female).                     |
| `bmi`      | float     | Body mass index, a key indicator of body fat based on height and weight. |
| `children` | int       | Number of dependents covered by the insurance plan.                      |
| `smoker`   | object    | Indicates whether the beneficiary smokes (yes or no).                    |
| `region`   | object    | The beneficiary's residential area in the US, divided into four regions. |
| `charges`  | float     | Individual medical costs billed by health insurance.                     |

Our goal is to use the `insurence.csv` dataset to train a regression model that predicts health care costs in the `validation_dataset.csv`.

To achieve this, we will perform some EDA to understand which variables influence the response variable we are trying to predict: `charges`.
