# Predicting Health Care Costs

This project is from [Datacamp](https://www.datacamp.com), but the dataset was made available by [Keith Galli](https://www.youtube.com/watch?v=mpfU9n4MzBE) in his GitHub repository.

Here, I present my process for investigate and cleaning a dataset, as well as performing exploratory data analysis. I explain my conclusions and insights throughout the analysis.

## Tools I used:

- Jupyter Notebook (within VS Code)
- Python 3.12
- Pandas 2.2.3
- Seaborn 0.13.2
- Scikit-learn 1.5.2

## My biggest difficulties:

While cleaning the data, I encountered a problem with the `sex` column, where I needed to standardize the observations to _male_ and _female_. I overcame this issue by creating a map with a dictionary and using the `.replace()` method in the respctive column. _ChatGPT 4.0_ assisted with this solution, as well as with other syntax and debugging problems along the way.
