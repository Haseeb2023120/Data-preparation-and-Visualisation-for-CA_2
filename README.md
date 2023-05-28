# Data-preparation-and-Visualisation-for-CA_2
![7217a37e-4d60-4610-8f24-f46fd9d13b70](https://github.com/Haseeb2023120/Data-preparation-and-Visualisation-for-CA_2/assets/133133400/52dc8a4a-785f-43e3-adf8-c5461146a113)
 Visualize the data
plt.figure(figsize=(10,8))
sns.heatmap(df.drop('Year', axis=1), cmap='coolwarm', annot=True, fmt=".1f")
plt.title('National House Construction Cost Index over Years')
plt.ylabel('Year')
plt.xlabel('Month')
plt.show()

 **Plotting line plots for each month**
plt.figure(figsize=(14,10))
for column in df.columns[1:]:
    plt.plot(df['Year'], df[column], label=column)
plt.legend()
plt.xlabel('Year')
plt.ylabel('Construction Cost Index')
plt.title('Construction Cost Index Over Years for Each Month')
plt.show()
![3eafa38f-623c-45ea-aff2-fcf1eddedfb8](https://github.com/Haseeb2023120/Data-preparation-and-Visualisation-for-CA_2/assets/133133400/8d8026ac-efc4-4a04-b1de-66d585415c63)

