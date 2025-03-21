# NumPy
Python Libraries

Create a NumPy array of numbers from 1 to 10 and calculate the mean
import numpy as np

# Create a NumPy array
array = np.arange(1, 11)

# Calculate the mean
mean_value = np.mean(array)

print("Array:", array)
print("Mean:", mean_value)
2. Load a small dataset into a Pandas DataFrame and display summary statistics
import pandas as pd

# Create a small dataset
data = {
    'Name': ['Alice', 'Bob', 'Charlie','David', 'Eva'],
    'Age': [24, 27, 22, 32, 29],
    'Score': [85, 90, 88, 76, 95]
}

# Load the dataset into a DataFrame
df = pd.DataFrame(data)

# Display summary statistics
summary_statistics = df.describe()

print("DataFrame:\n", df)
print("\nSummary Statistics:\n", summary_statistics)
3. Fetch data from a public API using requests and print a key piece of information
import requests

# Fetch data from a public API
response = requests.get('https://api.coindesk.com/v1/bpi/currentprice.json')

# Check if the request was successful
if response.status_code == 200:
    data = response.json()
    # Print a key piece of information
    bitcoin_price = data['bpi']['USD']['rate']
    print("Current Bitcoin Price in USD:", bitcoin_price)
else:
    print("Failed to fetch data from the API")
4. Plot a simple line graph using Matplotlib
import matplotlib.pyplot as plt

# List of numbers
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Plot the line graph
plt.plot(numbers)
plt.title('Simple Line Graph')
plt.xlabel('Index')
plt.ylabel('Value')
plt.show()




