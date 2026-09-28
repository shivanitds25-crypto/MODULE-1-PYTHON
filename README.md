# MODULE-1-PYTHON
import pandas as pd

# Read demographic data from CSV file
df = pd.read_csv("demographic_data.csv")

# Display first 5 records
print("Demographic Data:")
print(df.head())

# Calculate average values
print("\nAverage Population:", df["Population"].mean())
print("Average Literacy:", df["Literacy"].mean())
print("Average Income:", df["Income"].mean())

# Find state with highest population
highest = df.loc[df["Population"].idxmax(), "State"]

print("\nState with Highest Population:", highest)
