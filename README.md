# PCMS

Pulse Count Monitoing System
Previously, in factories, like sugar and cement, there used to persons sittingnear the fast moving conveyor to count the no of cement and sugar bags generated or moved to godown from production. But there can be some error in counting and some companies were demanding that no of bags generated were not exactly going to the godown, their was mismatch. So, it led to develop a system particularly hardware devices to auttomatically capture the count of number of bags generated and went to godown. So, Hixaa Technologies Provate Limited built a hardware system and the part of showing the data of devices (silo for production and godown for godown) on the dashboard was done by me.

The dashboard was created using Thingsboard - An opensource IoT platform through MQTT Client protocol. The dashboard was realtime updating as soon as the count increases in the hardware system it shows the updates in dashboard as well.

There are 4 Silo devices (production devices attached) and 1 godown device (goddown device attached). All these devices data is shown on dashboard with LifeTimeCount and TodaysCount of each device.
