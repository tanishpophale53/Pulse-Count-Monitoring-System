# Pulse Count Monitoing System


Previously, in factories, like sugar and cement, there used to persons sitting near the fast moving conveyor to count the no of cement and sugar bags generating or moving towards godown from production. But there can be some error in counting and some companies were demanding that no of bags generated during production were not exactly going to the godown, their was mismatch. So, it led to develop a automated system to capture the count of number of bags moving on fast moving conveyor and going to godown. So, Hixaa Technologies Provate Limited built a hardware system and the part of displaying the realtime data of devices (silo for production and godown for godown) on the IOT dashboard was done by me.

The dashboard was created using Thingsboard - An opensource IoT platform through MQTT Client protocol. There are 4 Silo devices (production devices attached) and 1 godown device (goddown device attached). Each device (both silo and godown) was having raspberry pi zero 2W fitted in it which was connected to wifi and this was sending the realtime data generated to the sql database and then the thingsbard server was fetching the data from the database and showing the data of devices like LifeTimeCount of that device and TodaysCount of that device on the dashboard.



### Preview of Dashboard

![WhatsApp Image 2024-03-25 at 8 23 52 PM](https://github.com/tanishpophale53/PCMS/assets/71888416/4b20ef50-993f-4024-bc76-c0832ea32d98)


![WhatsApp Image 2024-03-25 at 8 23 52 PM (1)](https://github.com/tanishpophale53/PCMS/assets/71888416/a7dcd506-d64b-4971-9c62-5c1c908d492a)
