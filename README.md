# PyBer Analysis Challenge 5

There are two obejctives of this module
1. Create a summary DataFrame that showcases the following for each city type:
    Total Rides
    Total Drivers
    Total Fares
    Average Fare per Ride
    Average Fare per Driver
2. Plot a multiple line graph that tells us about the fares for each city type over time.

# Addressinig Obejctive 1: Summary Dataframe
## Resources Used: 
Merged dataframe after combining city_data.csv and ride_data.csv.
## Steps:
      Created 5 new dataframes(line 991 onwards) that calculates the Total rides, total drivers, total fares, average fare per ride and average fare per driver.
          
      Created a final summary dataframe to include the values obtained from the step above.
            
      The formatting was set correctly as per the requirement on the final dataframe.

![alt text](https://github.com/29bharat/PyBer_Analysis/blob/master/analysis/Summary%20Dataframe.PNG)

## Analysis
  
       Looking at the summary, we can say that even though Urban Cities had significantly higher rides and drivers compared to Suburban and Rural cities, the average fare per ride and per driver is reamins the lowest amonst the three city types.
         
       Rural had the least number of rides(13 times less than Urban and 5 times less than Suburban) and drivers (approx 31 times less than Urban and 6 times less than Suburban)  yet tops with average fare per ride($10 more than Urban and $3.5 more than Suburban) and per driver(approx $39 more than Urban and $16 more than Suburban).
         
         
# Addressinig Obejctive 2: Multiline Plot
## Resources Used: 
Merged dataframe after combining city_data.csv and ride_data.csv.
## Steps:
      Renamed Columns and set Date as the index
        
      Created a new dataframe with just Date, City Type and Fare columns and set the index to datetime dtype
        
      Calculated the sum of Fare by grouping on City Type and created a new Pivot dataframe followed by filtering on the date as required.
        
      Plotted a multiline chart graph on tha data
      
![alt text](https://github.com/29bharat/PyBer_Analysis/blob/master/analysis/PyBerChallenge5.png)

## Analysis
  
       Looking at the multiline chart,we see that from March onwards, there was a spike in Urban in the Fares.
         
       Suburban saw better fare uptil March but dropped from mid-march to mid April.
         
       Rural pretty much remained consistent thorughout ranging between $0-500
