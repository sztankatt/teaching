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
6. Plot a barplot using the `sns.countplot()` function, which shows the number of passengers that embarked in each town.
**HINT** to plot a barplot like this use the command below:
```
bar0 = sns.countplot(data=..., x=...)
fig = bar0.get_figure()
fig.savefig('plots/barplot.png')
plt.clf()
```
7. Plot a histogram of the `fare` column using the `sns.histplot()` command and save it.
8. Plot a histogram of the `fare` column, but this time split it by `class`. 
**HINT** the command below splits by column. In the first line, you need to specify which column to split by (`col='...'`), and in the second line 
which variable to show (`x='...'`).
```
g = sns.FacetGrid(data=..., col='...')
g.map_dataframe(sns.histplot, x='...')
g.savefig('plots/split_histogram.png')
plt.clf()
```
9. Create a new column in the dataframe called `log_fare` which has the natural logarithm of the `fare`. **HINT** use the `np.log()` function.
10. Repeat exercises 8. and 9. using the `log_fare` column.
11. Drop `nan`s from columns `survived`, `age`, `fare`, `class`, `embark_town` and `who`.
12. Fit a multiple linear regression with those variables, and print the results.
13. Interpret the result of the linear regression. Which variables are important, and why?
