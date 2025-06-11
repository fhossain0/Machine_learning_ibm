EDA data analysis (EDA) is an approach to analyzing data sets to summarize their main characteristics, ofthen with visual methods

# Why is EDA Useful? 
EDA allow us to get an initial for the data 
- This lets us determoine if the data amkes sense, or if further cleaning or more data is needed
- EDA helps to identify patterns and trends in the data these cna be just as import as findings from modeling

Some summary statistics :
Average, median, min, max Correletions, etc

Visualizations:
Histograms, scatter plots, box plots, etc

Data Wrangling :
Matplotlib, seaborn

sample= data.sample(n= 5, replace= True)
print(sample.iloc[:, -3:]) #### Positioning using index not not labels all rows and column from negetively three to all 

- There are many reasons to consider random samples from Dataframes
- For large data, a random sample can make computation easier
- We may want to over or under sample observations when outcomes are uneven

# Visualization Libraries 
Visualization can be in multiple ways 
- Matplotlib
- pandas(Via Matplotlib)
- Seabon
  - Statistically - focused plotting methods
  - Global Preferences incorporated by matplotlib
  - also Seaborn preferences are incorporated with matplotlib
 # Pandas Dataframes approach
 after importing matplotlib as plt 
 plt.plot(data.sepal_length, data.sepal_width, ls='', marker= '0', label= 'Sepal') this can be easy to to draw a simple graph
 plt.hist(Data.sepal_length, bins= 25) for histogrames easy to show

# Customize and objectorianted form of matplotlib syntax
- fig, ax= plt.subplots()
- ax.barh(np.arange(10)
-         , data.sepal_width.iloc(:10)) # iloc choosing based on index number not label

we can use tools to set position 
# set position of ticks and tick labels 
- ax.set_yticks(np.arange(0.4, 10.4, 1.0))
- ax.set_yticklabels(np.arange(1, 11))
- ax.set(xlabel= 'xlabel', ylabel= 'ylabel', title= 'Title') 
    


