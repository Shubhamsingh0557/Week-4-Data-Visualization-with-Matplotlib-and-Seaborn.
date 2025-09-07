# Week-4-Data-Visualization-with-Matplotlib-and-Seaborn.

# Matplotlib-
  * Matplotlib is a fundamental, versatile plotting library for Python.
  * It provides a low-level, command-style interface that gives you fine-grained control over every aspect of a plot.
  * Think of it as the foundational tool for creating static, interactive, and animated visualizations in Python.
  * It's a core Python library for creating simple visualizations.
  * You can make line plots, bar charts, scatter plots, histograms, and pie charts.
  * It gives full control over plot elements like labels, colors, and styles.


# Key Concepts-
  * Pyplot:This is a module within Matplotlib that provides a state-based interface. It automatically creates figures and axes for you as you call plotting functions (like plt.plot(), plt.scatter()). It's the simplest way to get started.
  * Figures and Axes: A Figure is the top-level container for all plot elements. You can have multiple Axes (plots) within a single Figure. The Axes are where the data is actually plotted. This object-oriented approach is more powerful for creating complex layouts.
  * Basic Plots: Matplotlib is excellent for creating a wide variety of standard plots:
      * plt.plot(): A line plot, ideal for showing trends over time or continuous data.
      * plt.scatter(): A scatter plot, used to show the relationship between two numerical variables.
      * plt.bar(): A bar chart, used for comparing discrete categories.
      * plt.hist(): A histogram, for visualizing the distribution of a single numerical variable.

# Example-

    import matplotlib.pyplot as plt
    plt.plot([1, 2, 3], [4, 5, 6])
    plt.title("Line Plot")
    plt.show()

# Seaborn-
  * Seaborn is a high-level, statistically-focused plotting library built on top of Matplotlib.
  * It simplifies the creation of complex and aesthetically pleasing plots, especially for exploring relationships within datasets.
  * Seaborn's strength lies in its ability to integrate with Pandas dataframes, making it a go-to choice for exploratory data analysis.
  * Built on top of Matplotlib, but easier and more stylish.
  * Great for statistical plots and working with Pandas DataFrames.
  * Supports heatmaps, pairplots, boxplots, violin plots, and more.

# Key Concepts-
  * Aesthetic Styling: Seaborn comes with built-in themes and color palettes that make your plots look professional and clean with minimal effort. It handles aspects like grid lines, backgrounds, and color schemes automatically.
  * Dataset-Oriented: Seaborn functions often take an entire dataframe as an input, along with columns to specify which variables to plot. This is a more intuitive and concise way of creating plots compared to Matplotlib's column-by-column approach.
  * Advanced Plots: Seaborn excels at creating complex statistical visualizations:
      * Heatmaps (seaborn.heatmap): Excellent for visualizing matrices of data. The intensity of color represents the value of a variable, making it easy to identify patterns in correlation matrices or tabular data.
      * Pair Plots (seaborn.pairplot): This is a powerful tool for exploring relationships between multiple variables in a dataset. It creates a grid of scatter plots for each pair of variables and a histogram for each individual variable on the diagonal.
      * Violin Plots (seaborn.violinplot): A more informative alternative to a box plot, combining a box plot with a kernel density estimation of the data's distribution.
      * Joint Plots (seaborn.jointplot): Shows the relationship between two variables, along with their individual distributions in a single plot.

# Example-

    import seaborn as sns
    df = sns.load_dataset('iris')
    sns.pairplot(df, hue='species')
    
