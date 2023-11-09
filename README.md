 ### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: To  configure  the Network server and end device for traferring data on the network
## Components required: end node stm 32 development kit , dragino LPS8, network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow 
 3. click on the add gateway 
4. click on the lora options , lora - frequency plan 
5. click on channel s and create a new channel after which you can add a new end device 
6. add the attributesin the end device as  shown below 
7.using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)



## OUTPUT 

While click on network layer:
![Screenshot (369)](https://github.com/Anusharonselva/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119405600/6126d72a-5594-48e3-9892-4901bb5ae97c)
Gateway created:
![Screenshot (370)](https://github.com/Anusharonselva/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119405600/df71b892-1ace-4076-bf73-855be21d345d)
General setting view of a gateway created:
![Screenshot (371)](https://github.com/Anusharonselva/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119405600/930904f4-e7db-49f1-8b86-4f6c346d591f)
Gateway overview:
![Screenshot (372)](https://github.com/Anusharonselva/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119405600/b5c00e06-0412-42c3-8469-aa74da083302)
Channel for the gateway is created and its general settings view:
![Screenshot (373)](https://github.com/Anusharonselva/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119405600/cb1cb8b7-7835-4f7e-9a3d-9d45a7349769)
Channel overview:
![Screenshot (374)](https://github.com/Anusharonselva/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119405600/8ce7fd59-de36-4324-bb74-4c5eaf1b2c7a)
Channel view with description:
![Screenshot (375)](https://github.com/Anusharonselva/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119405600/336ece35-270e-470c-a126-ad828a04bf23)
End device of the channel created:
![Screenshot (376)](https://github.com/Anusharonselva/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/119405600/9e647435-8b8d-4ebe-9e68-abe01d5f6a79)



## Results: 

  The Network server and end device for traferring data on the network has been accomplished.

