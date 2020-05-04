# Household-Energy-Consumption
## Introduction
A regional home developer is looking to develop analytics for a new set of electrical sub-metering devices used for power management in smart homes. Installing these sub-meters could be a big step towards the developer's goal of offering highly efficient smart homes that provide owners with power usage analytics.

We're provided with a very large data set that contains 47 months of energy usage data from these devices. Our goal is to analyze this data to determine what kind of analytics and visualizations can be created that would empower smart home owners with greater understanding and control of their power usage.

In this project, we will begin by exploring some visualizations of the data and then build predictive models that will demonstrate to our client how the data can be used to help a home owner to make decisions about altering power consumption.

## Visualization
### Background: Household Energy Consumption 2007-2010
In the time period of 2007-2010, energy used by water heater and AC has increased every year, whereas energy used by kitchen and laundry room has gradually decreased.

![image](https://user-images.githubusercontent.com/57699414/80930401-98f0e880-8d70-11ea-9543-3583a2900d2c.png)


### Historical Energy Consumption Overview

![image](https://user-images.githubusercontent.com/57699414/80930815-20d7f200-8d73-11ea-85bc-f9a05e22bb57.png)

- The power consumption of kitchen is much less frequent than laundry room and water heater/AC. But when it's in use, it has high peaks.
- The power consumption of laundry room has the most variation.
- The power consumption of water heater/AC has the least variation but the most frequency.


### Daily & Weekly Power Consumption

<p float="left">
   <img src="https://user-images.githubusercontent.com/57699414/80933395-cb0a4680-8d80-11ea-8ae4-4edf35d90082.png"
	height="300" width="350" />
   <img src="https://user-images.githubusercontent.com/57699414/80933786-43bdd280-8d82-11ea-9bda-68f1f80585b9.png"
	height="300" width="400" />
</p>

We randomly selected Jan 9th, 2008 as an example:
- The power consumption in the kitchen has a peak in the early morning, possible due to home owners making breaksfast.
- The power consumption of laundry room has regular intervals of every 2 hrs, which is likely due to the cycle of finishing and starting a new load of laundry.
- Water heater and AC are used in the morning when home owners are getting up and showering, and then between 2pm-10pm when children and parents are returning home.


