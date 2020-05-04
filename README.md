# Household-Energy-Consumption
## Business Problem
A regional home developer is looking to develop analytics for a new set of electrical sub-metering devices used for power management in smart homes. Installing these sub-meters could be a big step towards the developer's goal of offering highly efficient smart homes that provide owners with power usage analytics.

We're provided with a very large data set that contains 47 months of energy usage data from these devices. Our goal is to analyze this data to determine what kind of analytics and visualizations can be created that would empower smart home owners with greater understanding and control of their power usage.

In this project, we will begin by exploring some visualizations of the data and then build predictive models that will demonstrate to our client how the data can be used to help a home owner to make decisions about altering power consumption.

<br/><br/>
## Visualization
### Background: Household Energy Consumption 2007-2010
In the time period of 2007-2010, energy used by water heater and AC has increased every year, whereas energy used by kitchen and laundry room has gradually decreased.

![image](https://user-images.githubusercontent.com/57699414/80930401-98f0e880-8d70-11ea-9543-3583a2900d2c.png)


<br/><br/>
### Historical Energy Consumption Overview

![image](https://user-images.githubusercontent.com/57699414/80930815-20d7f200-8d73-11ea-85bc-f9a05e22bb57.png)

- The power consumption of kitchen is much less frequent than laundry room and water heater/AC. But when it's in use, it has high peaks.
- The power consumption of laundry room has the most variation.
- The power consumption of water heater/AC has the least variation but the most frequency.


<br/><br/>
### Daily & Weekly Power Consumption

<p float="left">
   <img src="https://user-images.githubusercontent.com/57699414/80933395-cb0a4680-8d80-11ea-8ae4-4edf35d90082.png"
	height="300" width="350" />
   <img src="https://user-images.githubusercontent.com/57699414/80933786-43bdd280-8d82-11ea-9bda-68f1f80585b9.png"
	height="300" width="400" />
</p>

For daily analysis, we randomly selected Jan 9th, 2008 as an example:
- The power consumption in the kitchen has a peak in the early morning, possible due to home owners making breaksfast.
- The power consumption of laundry room has regular intervals of every 2 hrs, which is likely due to the cycle of finishing and starting a new load of laundry.
- Water heater and AC are used in the morning when home owners are getting up and showering, and then between 2pm-10pm when children and parents are returning home.
<br/><br/>

For weekly analysis, we randomly selected Jan 8th-14th:
- Home owners use the kitchen much more frequently on Sunday.
- The usage of laundry room has spikes on weekend and in the middle of the week.
- The usage of water heater and AC doesn't have much variation throughout the week.
<br/><br/>


### Decomposition-Seasonal Trend

<p float="left">
   <img src="https://user-images.githubusercontent.com/57699414/80935458-efb6ec00-8d89-11ea-961f-9f68cba3b2e3.png"
	height="250" width="250" />
   <img src="https://user-images.githubusercontent.com/57699414/80935483-137a3200-8d8a-11ea-87dc-87b749ae25d3.png"
	height="250" width="250" />
   <img src="https://user-images.githubusercontent.com/57699414/80935498-22f97b00-8d8a-11ea-8508-a43eedf11fe2.png"
	height="250" width="250" />
</p>

- All three sub-meterings have obvious seasonal trends but no significant overall upward or downward trend.
- Kitchen:
Power uage has an upward trend since the third quarter of 2007 and then starts to drop in the second quarter of 2008, which seems to coincide with the timeline of Star energy saving campaign. There's obvious seasonality where the usage is low throughout summer and fall and peaks at the end of the year, which might be due to the holidays.
- Laundry room:
Power usage significantly increased in 2008 and starts to decrease in the second quarter of 2009. The first peak is in the beginning of the year, followed by the second peak in the beginning of spring.
- Water-heater and AC:
The usage doesn't have much fluctuation until the second quarter of 2009; it drops to the lowest point in summer 2009 and starts an upward trend. It shows a seasonl trend where the consumption is lower in summer, which might be due to the fact that people ususally spend less time at home during summer.
<br/><br/>

## Forecast From Linear Regression Model

![image](https://user-images.githubusercontent.com/57699414/80935812-9cde3400-8d8b-11ea-9b90-bd6016b66400.png)

- The forecast of kitchen power consumption is much less frequent compared to laundry room, water heater and AC; it also has the lowest watt per hour on average.
- The predicted power consumption of laundry room has the most variation between 0-40 watt per hour.
- The predicted power consumption of water heater and AC has the least variation between 5-20 watt per hour but the most frequency, indicating a more constant usage.








