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
 ![iotserver](https://github.com/user-attachments/assets/e4d28d24-fb9e-479a-a799-8ba658dfddd5)

 3. click on the add gateway 
![Screenshot 2024-10-26 112441](https://github.com/user-attachments/assets/3cc58d88-ead8-4d8c-9681-7848ce8edd40)

![Screenshot 2024-10-26 104858](https://github.com/user-attachments/assets/57aeb725-e752-4113-ab8a-7546af3abf76)
4. click on the lora options , lora - frequency plan 
5. click on channel s and create a new channel after which you can add a new end device 
![Screenshot 2024-10-26 105220](https://github.com/user-attachments/assets/dcd8ded9-677e-48c6-a4f7-485caf52f603)

6. add the attributesin the end device as  shown below 
![image](https://github.com/user-attachments/assets/e7636f9f-1fd7-4b6a-8a74-97ac4d2f5d28)

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
![image](https://github.com/user-attachments/assets/988c40cf-b4c9-49e4-84e7-8b923dbc498a)



## Results: 

  The Network server and end device for traferring data on the network has been accomplished.

