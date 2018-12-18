# Project Status.
# generator_auto_start

This Repository only started and is not compleetb yet<br>
This repository will have att the details of how I have build an Remote controllable Generator Auto start capability.<br>
I wanted to have the capability to start my Petrol Generator when we have Power outage at my hous.<br>
Sins we now have regular Load shedding in South Africa it has become a real problem to keep my webservers up and running<br>
I needed a system to auto start an electric start Petrol Generator when the City power goes down as my UPS can only keep the servers running for a short while.<br>
I desided to split the implimentation in two.<br>
One to start the Generator and the other to stop the Generator.<br>
This repository will only have the Generator start documentation.<br>
The Generator stop details will be holed in the following repository. https://github.com/antonjan/automatic_power_transfer_system <br>
I wanted to modes.<br>
One to autostart when ever the City Power is down.<br>
Two Only Start the generator when I give a command remotely via Wifi TCP connection.<br>
## Generator Requerments.
To Start a Petrol Generator you need to consider the following.<br>
1) Chock need to be pulled when generator is could and the starter needs to be activated untill engin starts and the Chocke must be released to it run postion.
2) Detect if Generator is cold or warm to identify if chock need to be pulled.<br>
3) A warm start mite only need an Half chocke setting to start on some Generators no Choke.
4) Detect if Generator is running.
5) There is other factors like oile level and temprature but this is normely monitored by the generator ist self.

## Automatically start when City Power is down.

Lets look at the Coled Start option first.<br>
1) Check Generator Temprature and check ists coled start.<br>
2) Pull chocke to maximum with Magnetic Actuator.<br>
3) Close relay for Starter and on position key and monitor output voltage for (Predefined Time, Must be configurable EG 900ms)
4) if Voltage rises then deactive Chock Actuator to disable chock disconnect Starter relay but keep on relay on.
5) if Voltage did not rise then deactivate starter relay but keep on relay to on position. Waite for about 3 Seconds and then gotostart with one<br>
## Start only with TCP Command via Mobile APP.


## Read exsiting Status of power and Generator via Mobile APP.

## Stop Generator remotely via Mobile App. 
