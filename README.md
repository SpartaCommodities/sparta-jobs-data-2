# Data Exercise

The goal of this exercise is to implement a script that reads the csv document provided, analyze, and clean the data from outliers.

The document provided has all the calculated values to gather the delivery price of gasoline in the ARA (Europe) to NY route, called RBOB, for 6 different months. The document contains one work week of data.

Document link:

The important columns of the document are:

- generated_on: This column contains the date of the calculation of the data, usually we make a calculation per route/month every 15 minutes, but this can not be allways true due to a changes of some prices or errors on the backend.
- display_name: This columns contains the name of the route, in this document we have only included RBOB, that is the route we need to analyse.
- load_month: This column contain the month for the one we are calculating the prices. Currently we calculate the current month, and 5 in the future. This document that was generated at the end of September you will be able to see calculations for Sep'21, Oct'21, Nov'21, Dec'21, Jan'22, Feb'22.
- dlvd_price: The final price of delivery, the value we need to analyse and clean.

After being able to read and plot the data, in a meeting with the stakeholders, they have marked which are the clear outliers in the data, and ask you to being able to detect them in real time, and remove them before are sent to the backend to plot the historics.
![plotted data for the text](https://i.imgur.com/1Mzc1bU.png)

## The work to be done for this exercise is:

1. Create a script that can read the data secuentially, and solve any format problems that could appear.
2. Plot the data to find the outliers
3. Iterate the read script to detect the outliers and save the data cleaned in a separated csv.

To give your answer, create a repository in any platform you feel confortable with and share it with us. Over that solution we will discuss in a pair-programming about the solution chosen, the thoughts to reach that solution, and a possible improvement.
