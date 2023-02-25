Save everything in a `mock_exam_1.py` file. 

Before starting the exercises: load `pandas`, `numpy`, `seaborn`  and `statsmodels.formula.api` the same way like in the homeworks.

Import pyplot using the `import matplotlib.pyplot as plt` command.

### Exercises 

1. Load the dataset 'titanic' using the command `sns.load_dataset()` and save it the `df` variable.
2. Print the columns of the data-frame, as well as the first few rows with the `head()` command, and some summary statistics with the `info()` command.
3. Use the `assign()` command to add a new column to `df` called `embark_country` and set it to: `England` if `embark_town` is `Southampton`, `France` if `embark_town` is `Cherbourg`
and `Ireland` if `embark_town` is `Queenstown`.
4. Using the `value_counts()` command calculate how many passengers embarked the Titanic in each town.
5. Create a folder to store the images, the same way as in class.
6. Plot a barplot using the result of the previous exercise - to plot the number of passangers by embarkment town.
HINT: to plot and save a barplot use:
```
bar0 = sns.barplot(data=...)
fig = bar0.get_figure()
fig.savefig('plots/barplot.png')
plt.clf()
```
