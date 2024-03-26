# Pulse Count Monitoing System


Previously, in factories, like sugar and cement, there used to sit a person near the fast moving conveyor to count the no of cement and sugar bags generating or moving towards godown from production. But there can be some human error in counting and some companies were demanding that no of bags generated during production were not exactly going to the godown, their was mismatch. So, it led to develop a automated system to capture the count of number of bags moving on fast moving conveyor and going to godown. So, Hixaa Technologies Private Limited built a hardware system and the part of displaying the realtime data of devices (silo for production and godown for godown) on the IOT dashboard was done by me.

The dashboard was created using Thingsboard - An opensource IoT platform through MQTT Client protocol. There are 4 Silo devices (production devices) and 1 godown device. Each device (both silo and godown) is having raspberry pi zero 2W fitted in it which is connected to wifi and will send cientId, deviceID and count i.e LifeTimeCount as parameters. These three parameters will initially get store into sql database. The thingsboard server will check if the database has changed or not. If changed, then it will immediately update the entry of that device on the dashboard in realtime. Fetching of data is done using python and MySQL.

By analyzing the database, more parameters are created in order to show on dashboard related to silo and godown devices like TotalSiloCount, TotalGodownCount, TodaysSiloCount, TodaysGodownCount, TodaysDifference, TotalDifference, Total Silo, TotalGodown, TotalSilo/Godown.


## Glimpse of Dashboard

#### Parameters Abbrevation 

Total Silo - Total Silo devices
TotalGodown - Total Godown devices
TotalSilo/Godown - Total Silo/Godown devices

LifeTimeSiloCount - sum of count 
TotalSiloCount - sum of count of all silo devices from the day hardware system is attached
TotalGodownCount - sum of count of all godown devices from the day hardware system is attached
TotalDifference - difference between TotalSiloCount and TotalGodownCount

TodaysSiloCount - sum of count of today of all silo devices
TodaysGodownCount - sum of count of today of all godown devices
TodaysDifference - difference between TodaysSiloCount and TodaysGodownCount


![WhatsApp Image 2024-03-25 at 8 23 52 PM](https://github.com/tanishpophale53/PCMS/assets/71888416/4b20ef50-993f-4024-bc76-c0832ea32d98)


![WhatsApp Image 2024-03-25 at 8 23 52 PM (1)](https://github.com/tanishpophale53/PCMS/assets/71888416/a7dcd506-d64b-4971-9c62-5c1c908d492a)
