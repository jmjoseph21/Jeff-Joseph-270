# Jeff-Joseph-270
1.- 
The first plot shows the total number of cases of COVID-19 (past plus current) in the United States at any given day since the start of the pandemic.
In order to produce the plot, we first need to group the data by date and find the cumulative number of cases each day.
The second step is to find the number of cases reported each day and from that we can generate the rolling average of new cases per 7 day periods.

2.- 
We first filter the data to be at the appropriate date, in this case up to 2021-01-17. We then group by date and sum th enumber of cases to find the cumulative number of cases. We again make use of the lag function to find the number of cases reported that specific day. We then proceeed to find the 7 day average number of cases. To find the 14-day change we do  7-day average cases on 2021-01-17 minus 7-day average number of cases on 2021-01-03 and divide all of it by the former. 
We follow similar process to generate the corresponding numbers for deaths and hospitalizations. 

3.- 
We first filter the data as described above in order to reject any data post 2021-01-17 and contain informationonly up to that point. Then we group the data by state while summing the number of cases over all days in the new dataset. 
To obtain the average in the last 7 days for each state, we proceeded as follows:
- Group the data by state and date and sum the total number of cases.
- Make use of lag function to find number of new cases for each day in the data.
- The find the 7-day average number of new cases at each point in the data.
- Lastly, filter the data to se what the average number of new cases is for the last 7 days in each state. 
