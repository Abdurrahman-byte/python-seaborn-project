Nothing much just a bunch of seaborn practice sessions, as a part of my machine learning journey in order to strengthen the foundation.
        So what is seaborn?
Seaborn is a python library for statiscal data visualization.It builds on matplotlib and integrate naturally with pandas Dataframes.
      Importing Seaborn:
open your jupyter notebook and create a cell and import the following:
-import pandas as pd
-import matplotlib as plt
-import seaborn as sns
The common alias for Seaborn is sns, just as pd  for pandas, plt for matplotlib and np for numpy.
       How to install Seaborn
to install seaborn in jupyter notebook cell enter:
*%pip install seaborn*
and then rerun the imports
and to check your Seaborn version enter:
*print(sns.__version__)*       

       Line plot
A line plot connects data points to help reveal how a value changes across an ordered variable such as time, study hours , or dates.  

Examples:
*sns.lineplot()*

when to use it:
To show a trend or progression.

Note:
One important distinction; a scatterplot shows individual relationships without connecting the points by default; lineplot in other words connects them to emphasize the pattern.

          Bar Plot
A barplot compares a numerical measurement across categories. By default, *sns.barplot()* estimates the mean for each category.

when to use it:
When you want to compare average exam score between groups, average revenues by product, or average rating by region.

Note:
Remember; a barplot shows an aggregate statistics by default, not every student's individual score.

            Count Plot
Use to obverse which category belongs to which

when to use it:
Counting students by gender, orders by status, or products by category.

Note:
Unlike *barplot()*, *countplot()* counts how often each category appears. it doesnt need a numerical y column

           Hist Plot
A histogram groups numerical values into intervals called bins and shows how many observation falls into each interval.

When to use it: To investigate whether values cluster in certain ranges, whether disribution is spread out, or whether it has a long tail.

           How to read it:
-The x-axis shows exams-score intervals.
-The y-axis shows the number of students in each intervals
-*bins=5* ask seaborn to divide the score range into five intervals.   

           BoxPlot
A boxplot summarizes the distribution of numerical data using quartiles, the median, whiskers. It can also pontential outliers.

When to use it: Comparing the spread of exam scores between groups, checking whether one group has more variability or investigating pontential outliers.

            How to read it:
-Line inside the box: median score
-Box: middle 50% of the scores, between the first and third quartiles.
-Whiskers: extend to value within the plot's whiskers rule.
-Points beyond the Whiskers: pontential outliers under 1.5 x IQR rule.

           Heat Map
A heatmap represents numerical values using colors.One common use is visualizing correlations between numerical columns.

            How to interpret correlation:
- Near +1: Strong positive linear relationship
- Near 0: Little or no linear relationship
- Near -1: Strong negative linear relationship            