Introduction

This data set was created by TouringPlans.com specifically to give programmers and statisticians who may be interested in working with them someday some actual data they have compiled to practice on. Initially it was provided to students at the University of Central Florida in 2017. Because a friend of mine is one of the creators of TouringPlans.com, he graciously provided this to me to explore as well.

A total of four data sets were provided, each consisting of wait time data for one of the four Walt Disney World theme parks (Magic Kingdom, Epcot, Hollywood Studios, and Animal Kingdom) for a particular time period. I have chosen to use the Magic Kingdom ("MK") data set for this project.

To keep the project scope from getting away from me, before importing the set into R, I did some cleaning on it--specifically, I narrowed the date range down to the most recent two complete years for which data was provided (2015 and 2016) and removed some columns that were included but had no data.

For each data, the standby wait time in minutes ("SPOSTMIN") of some specific attractions in the park (list of attractions was notprovided to me) was recorded several times a day.


Data Dictionary

Main Variables
	SPOSTMIN	Standby Posted Wait Time (in minutes)	numeric
	WGT	Weight of Wait Time (Geometric Decay)	numeric
	DATE	Park Day (not actual date stamp of the wait time, since some are after midnight)	Excel Date
	TIMEPART	Time of Day	Excel Time

Pricing Variables
	WDW_TICKET_SEASON	Walt Disney World Single Day Price Type	alphanumeric

Day Variables	
	DAYOFWEEK	Day of Week	numeric
	DAYOFYEAR	Day of Year (1 to 366)	numeric
	WEEKOFYEAR	Week of Year (1 to 52)	numeric
	MONTHOFYEAR	Month of Year (1 to 12)	numeric
	YEAR	Year	numeric
	SEASON	Seasonal Category (Fall, Winter, Thanksgiving, etc.)	alphanumeric
	HOLIDAYPX	Proximity to Holiday (2-directional) (in days)	numeric
	HOLIDAYM	Holiday Metric (1 to 5 ranking)	numeric

School Schedules
INSESSION	Percentage of Schools in Session	numeric

Other Key Variables	
	NEWNESS	Rank of attraction staleness	alphanumeric
	SUNSET_WDW	Time of Sunset in Orlando	Excel Time
	WDWMINTEMP_MEAN	Average minimum daily temperature	numeric

Park Hours
	IAHOURS	Total Opening Hours for Islands of Adventure	numeric
	UFHOURS	Total Opening Hours for Universal Studios	numeric
	MKHOURS	Total Opening Hours for Magic Kingdom	numeric
	HSHOURS	Total Opening Hours for Disney Hollywood Studios	numeric
	AKHOURS	Total Opening Hours for Animal Kingdom	numeric

Capacity Variables
	CAPACITYLOST_MK	Total hourly capacity lost on that park day (due to attraction closures)	numeric
	CAPACITYLOSTWGT_MK	Total hourly capacity lost on that park day, weighted by attraction popularity	numeric


