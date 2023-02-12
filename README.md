# CS361_Software_Engineering_I

This repository contains the source code for my personal project “Weather Forecast APP” as well as the microservice created for my partner’s project.

Communication contract
I will use REST API as the communication pipeline. My plan is to create a web-based microservices using node.js and deploy it to the OSU server. Then my partner can send http request to my microservice.
- 1.Clear instructions for how to REQUEST data from the microservice you implemented. Include an example call.

a. express_microservice_random_generator.js will be connected to port 80.  This file will listen at this port when the program is running.

b. my partner’s program will send http “GET” request to fetch the data from this file.
Example call:  my partner can send “http:// ip number: 80/user” to request the random user profile from my microservice.

- Clear instructions for how to RECEIVE data from the microservice you implemented

a.after my microservice gets the request from my partner,  it will call a public api to get the random user profile, then my program will do some modification on the data I get because I plan to send only necessary data to my partner, all unnecessary data will be excluded. 

b.there is a call-back function in get method. (get method belongs to an instance of express library) send () method will be used to send back the data which are needed by my partner.

- UML sequence diagram showing how requesting and receiving data work. Make it detailed enough that your partner (and your grader) will understand
![image](https://user-images.githubusercontent.com/72511949/218302645-7f98a0db-4849-4a91-bb1f-4fe94343d04d.png)

 
