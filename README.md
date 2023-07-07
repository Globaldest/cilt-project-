# cilt-project-
import matplotlib.pyplot as plt
import pandas as pd

# Create a dictionary with the dataset
data = {
    'Year': [2015, 2016, 2017, 2018, 2019, 2020],
    'Total Tourist Arrivals': [1263745, 1261222, 1200345, 1345678, 1567890, 694567],
    'Domestic Tourist Arrivals': [783456, 789123, 765432, 789012, 823456, 298765],
    'International Tourist Arrivals': [480289, 472099, 435913, 556666, 744434, 395802]
}

# Convert the dictionary to a Pandas DataFrame
df = pd.DataFrame(data)

# Set the 'Year' column as the index
df.set_index('Year', inplace=True)

# Create a line graph using the DataFrame
df.plot(kind='line')

# Add a title and axis labels
plt.title('Tourist Arrivals in Kumasi (2015-2020)')
plt.xlabel('Year')
plt.ylabel('Number of Tourist Arrivals')

# Display the plot
plt.show()
