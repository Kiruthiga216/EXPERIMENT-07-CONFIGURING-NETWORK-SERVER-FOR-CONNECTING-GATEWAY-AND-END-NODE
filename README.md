### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: 
To  configure the Network server and end device for transferring data on the network
## Components required: 
End node stm 32 development kit , Dragino LPS8, Network server 

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
    
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1bd434ca-1426-4102-8384-94473483543e)
 3. Click on the add gateway 
 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/47c2e08d-6598-4437-8b07-f213d6f3b8ac)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/e62ff028-99bc-485e-9808-fbb6e124f8b2)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/a2e3ae58-6402-49e8-8f96-679059c1842c)
4. Click on the lora options , lora - frequency plan 

5. Click on channels and create a new channel after which you can add a new end device
   
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1fb72be5-e48d-4cde-a329-0cfb0d29070f)

6. Add the attributes in the end device as  shown below 

 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/00bff30b-42fc-42d5-9540-285d270e41cb)
 
7.Using AT commands configure end device in serial port utility
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


<img width="1918" height="1199" alt="Screenshot 2025-11-24 083851" src="https://github.com/user-attachments/assets/c10047c4-e39e-4ae3-9cfc-b937c3dd2614" />

<img width="1651" height="985" alt="image" src="https://github.com/user-attachments/assets/46d34e72-2fd4-440d-a15a-97402ae0fa4d" />

<img width="1288" height="755" alt="image" src="https://github.com/user-attachments/assets/37c5df54-154e-42cd-8fe1-ea2ff97da181" />

<img width="1287" height="747" alt="image" src="https://github.com/user-attachments/assets/19c977bc-c169-4d58-a7eb-0a202c9e57d9" />

<img width="1647" height="976" alt="image" src="https://github.com/user-attachments/assets/4fb86efe-1792-4c7b-b6f9-e7d4c971265e" />

<img width="1651" height="975" alt="image" src="https://github.com/user-attachments/assets/c09e935f-641c-4ee0-bebb-11e4a464a77e" />


<img width="1648" height="913" alt="image" src="https://github.com/user-attachments/assets/01c77215-55a7-4c8e-bfb9-695e73de6a3a" />


<img width="1647" height="985" alt="image" src="https://github.com/user-attachments/assets/378ee74c-e0b5-4095-a89d-7b3ed7fb6cdb" />


<img width="1387" height="812" alt="image" src="https://github.com/user-attachments/assets/6575dc09-227f-4aa6-b992-60146b373f5b" />


<img width="1389" height="821" alt="image" src="https://github.com/user-attachments/assets/219939df-80ec-4b71-8dc4-3c571d108643" />


<img width="1919" height="1088" alt="Screenshot 2025-11-24 101823" src="https://github.com/user-attachments/assets/44967b30-b403-4224-9cb3-f5a094a73cb8" />


<img width="1918" height="1037" alt="Screenshot 2025-11-24 103114" src="https://github.com/user-attachments/assets/4020f011-9e6b-442c-976c-21bf3ef52ebe" />

<img width="1917" height="1026" alt="Screenshot 2025-11-24 095830" src="https://github.com/user-attachments/assets/f4b8e297-081e-4ea3-89e6-70e347da3051" />

<img width="1917" height="1029" alt="Screenshot 2025-11-24 101020" src="https://github.com/user-attachments/assets/f883c029-6ec8-47d3-8c6e-5fa8d3258b3e" />


<img width="1919" height="1033" alt="Screenshot 2025-11-24 103754" src="https://github.com/user-attachments/assets/acd0500b-2c20-43ae-a584-5a9ed68f8894" />

<img width="1919" height="1038" alt="Screenshot 2025-11-24 103806" src="https://github.com/user-attachments/assets/5db4e95a-0d16-4463-9100-1caea6c56eb3" />

<img width="1916" height="1032" alt="Screenshot 2025-11-24 095842" src="https://github.com/user-attachments/assets/de1f2857-3d57-4f8b-90f1-3588dd0b4ae3" />

<img width="1908" height="1027" alt="Screenshot 2025-11-24 095856" src="https://github.com/user-attachments/assets/99838ca9-8956-497f-a466-ffb76f0eba99" />

<img width="1919" height="1020" alt="Screenshot 2025-11-24 101421" src="https://github.com/user-attachments/assets/4fd9932c-d6b2-49f6-ad44-ea7cd10fab1b" />

<img width="1914" height="1032" alt="Screenshot 2025-11-24 101433" src="https://github.com/user-attachments/assets/f934e290-66cf-43a2-bed7-03e7191bfbf7" />

<img width="1918" height="1036" alt="Screenshot 2025-11-24 101009" src="https://github.com/user-attachments/assets/988cbdfe-ecfd-4451-b35f-442aef3bc900" />


<img width="1919" height="1036" alt="Screenshot 2025-11-24 103136" src="https://github.com/user-attachments/assets/b7a0e0bb-cdfa-4e5f-b90e-97a2941228bd" />
<img width="1919" height="1027" alt="Screenshot 2025-11-24 103259" src="https://github.com/user-attachments/assets/c65171ad-ebf6-4948-91df-9f24c8b14999" />

<img width="1915" height="1034" alt="Screenshot 2025-11-24 095923" src="https://github.com/user-attachments/assets/4fe6dbf5-78be-4289-b666-28938ba21cff" />

<img width="1912" height="1027" alt="Screenshot 2025-11-24 095938" src="https://github.com/user-attachments/assets/fa7ae2ed-b7d7-4964-bc56-4504f3ddc93e" />

<img width="1918" height="1030" alt="Screenshot 2025-11-24 100003" src="https://github.com/user-attachments/assets/f541157a-ef48-42ba-8602-8075f75b3178" />

<img width="1919" height="1035" alt="Screenshot 2025-11-24 100043" src="https://github.com/user-attachments/assets/be01dee4-6a36-4fa8-8171-073cebd69ee4" />



<img width="1919" height="1144" alt="Screenshot 2025-11-24 095341" src="https://github.com/user-attachments/assets/ed72c5eb-7f4b-4702-9429-ce44927be6a4" />




















## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
