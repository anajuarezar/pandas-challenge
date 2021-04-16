# pandas-challenge
Pandas homework

Heroes of Pymoli

We begin in GitBash, where we activate the environment using the command: source activate PythonData. Once it is activated, we open Jupyter Notebook with that command. 

Once we have it open, we mush begint by importing the dependancies and setup: pandas as pd and numpy as np. After that, we import the resources we are going to use. In this case, 
we must import it using a save path and then open it as a csv file.

When this is set, we can begin. The first part of the homework is having the players count. For this we use the function nunique(), we use this because we need to count the players and given that they can buy several things, they will appear more than one. So we use unique() in order to count only the unique values.
After this, comes the Purchase analysis, for this we use the nunique to finde the games count, sum() to add the how much they made by adding the prices, mean() to find the average and count() to find the purchases. 
We then make a dataframe by using the dictionary method. We will only use it for this part, just because I wanted to show that it can be used. We must also give the dataframe the appropiate format, to do this we first need to make the column float numbers, once we have this we use .format and its code to format it. 

We can now begin with the gender demographics analysis. To begin, we need to group our data by gender, for this we use groupby and the column "Gender". We repeat the previous process using our grouped data to count the players by gender. To make the dataframe we are using concat, to concatenate the data que made. Once this is done, we begin the Purchase analysis by gender following the previous proceess as well. However there is new data we must obtain: Average Purchase Total per Person by Gender. We obtained this calculation by using by the sum of what each gender spent divided by the total of each gender to find what each gender spent per person. 

After we obtained all the information, we use concatenate to create the dataframe and the .format property. 


We begin the age demographic analysis. To obtain this we used loc to slice the original dataframe in order to work with the information we need only. We also drop the repeated data. After, we use bins to separate the ages into specific age groups. Later, we used groupby to make the age groups. We use count() to find the number of players of each age gropup and the percantage they represent. Finally, we make out dataframe and give it the format we want. 

We move to the purchase analysis by age. Since we used loc data in the past analysis and in this one we need all the information, we must use the bins and the groupby again. Later on, we follow the same procedure we used in the Purchase analysis by gender. We make the dataframe and give it the format we need. 

We go on to the Top spender analysis. To begin, we group the data by the players. In order to do this, we had to sort the data by the players id and group the data so we could find how much each player spent. Once this was done we did the usual calculations and built the dataframe. This time we had to sort the dataframe in a descending way to find the buyer who spent the most. Later we gave the dataframe the data we needed. It was important to do this AFTER the sorting because the $ sign would prevent us from sorting correctly.
To find the most profitable games and the most popular, we had to group the data by the item name and id; as well as slice the data by item related informatios, this way we only have the information we need. Once this is done we, make the usual calculations and make the dataframe. Later on, we sort by Purchase Count, since we have to format at this point. We created another column with the Item Price and Total Purchase value that we won't give the format so we can use it to sort the dataframe. We give the dataframe the format we need and sort it by the Purchase count. We print the columns that are formated.
Finally we must sort by Total Purchase value to find the most profitable games. Here is where we use the extra columns that weren't formated because they don't have the dollar sign. Thus finishing the homework 
