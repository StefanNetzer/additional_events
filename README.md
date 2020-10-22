Add additional events per schedule line 

The clock - output plugin is an easy way to create an event scheduler. But, it does not provide events for each event, but only a generic on/off event.

With this change I have two values the schedule line # (variable schedule) and the event value (i.e. Temp).


I have changed the selector to an FormNumericBox, since this is more convienient to enter a value. 

Sensor
GPIO → Clock Event:	- None -
Day,Time 1:	All,00:00
Temp1:	0
Day,Time 2:	All,00:00
Temp2:	0

With this one gets two output Values

Output
Temp

and of cause two events, which I may evaluate in the rules

556164: EVENT: timer#Output=1.00
556261: EVENT: timer#Temp=10.00

With this enhancement it is easy to use ESP as an edge device for tons of use cases ( thermostat, irrigation systems )
