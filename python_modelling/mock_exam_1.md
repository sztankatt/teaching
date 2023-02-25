Save everything in a `mock_exam_1.py` file. 

Before starting the exercises: load `pandas`, `numpy`, `seaborn` and `statsmodels.formula.api` the same way like in the homeworks.

### Exercises 

1. Load the dataset 'titanic' using the command `sns.load_dataset()` and save it the `df` variable.
2. Print the columns of the data-frame, as well as the first few rows with the `head()` command, and some summary statistics with the `info()` command.
3. Add a new column to `df` called `embark_country` and set it to: `England` if `embark_town` is `Southampton`, `France` if `embark_town` is `Cherbourg`
and `Ireland` if `embark_town` is `Queenstown`.
4. Using the `value_counts()` command calculate how many passengers embarked the Titanic in each town.
5. 
