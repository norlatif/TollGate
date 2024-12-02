# Introduction
This application simulates the system for congestion tax in Gothenburg along with the associated fee calculations for vehicles.
![Tax Logo](https://drive.google.com/uc?id=1-uqBf7fWfUvjGIMZ5U8597KQFFkO0ISL)


# Software Specification/Requirements
![Tax Gateway](https://drive.google.com/uc?id=13OjyBg3dn9C7K4C_NCyEndGQLaWqedo_)
Each passage through a toll station in Gothenburg costs 9, 16, or 22 kronor depending on the time. 
The maximum amount per day and vehicle is 60 kronor.

| Time                | Amount |
|---------------------|--------|
| 06:00–06:29         | 9 kr   |
| 06:30–06:59         | 16 kr  |
| 07:00–07:59         | 22 kr  |
| 08:00–08:29         | 16 kr  |
| 08:30–14:59         | 9 kr   |
| 15:00–15:29         | 16 kr  |
| 15:30–16:59         | 22 kr  |
| 17:00–17:59         | 16 kr  |
| 18:00–18:29         | 9 kr   |
| 18:30–05:59         | 0 kr   |

- Congestion tax is levied on vehicles passing a toll station Monday to Friday between 06:00 and 18:29. 
- No tax is levied on Saturdays, public holidays, days before public holidays, or during the month of July. 
- Certain vehicles are exempt from congestion tax.
- A vehicle passing multiple toll stations within 60 minutes is only taxed once.
  - The amount to be paid is the highest amount of those passages.
- "Backa exemption": A vehicle pays the congestion tax if it passes both a control point and a payment station within a period of 30 minutes. 
	- The order it passes them doesn't matter. 
![Tax control point](https://drive.google.com/uc?id=1N8uu582LuRO9amn-cMx-1D7KJUjkHp3d)
