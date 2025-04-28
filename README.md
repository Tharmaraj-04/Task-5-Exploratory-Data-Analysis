# Data_Visualization-task-5
Visual | Code | Purpose | Summary Histogram (Univariate) | df['Age'].hist() | See age distribution | Skewed towards young people. Missing values present. Boxplot (Age by Pclass) | sns.boxplot(x='Pclass', y='Age', data=df) | Compare age distribution per class | 1st class passengers were generally older. Countplot (Survival by Gender) | sns.countplot(x='Survived', hue='Sex', data=df) | See survival rate by gender | Females had much higher survival rates. Heatmap (Correlation) | sns.heatmap(df.corr(), annot=True, cmap='coolwarm') | Check feature correlations | Fare and Pclass correlated; Age and Fare slightly correlated with survival. Pairplot (Multivariate) | sns.pairplot(df[['Survived', 'Age', 'Fare', 'Pclass']]) | See relationship between numeric variables | Fare is higher for survivors; age not strongly correlated. Scatterplot (Fare vs Age) | sns.scatterplot(x='Age', y='Fare', hue='Survived', data=df) | Relationship of fare, age, and survival | Survivors paid higher fares generally.

# Summary of Findings
Missing Data: Age and Cabin have missing values; need imputation or dropping.

Passenger Class: 1st class passengers survived more often.

Gender: Females had much higher survival rates.

Fare: Higher fare → higher survival.

Embarked Port: Passengers from Cherbourg (C) had higher survival.
