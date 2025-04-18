<h1>Hello, welcome to the <u>CREATING A LAN</u> project!</h1>

<h2> Goals</h2>

1. Cable Management of the extra Ethernet, power cables, and HDMI cables
2. Create a pre-LAN chart of all devices and their connections (Via Packet Tracer)
3. Connect the Wireless Router to the internet and configure it
4. Connect the switch to the gaming pc and lab pc and configure it
5. Document the changes and lessons learned
6. Start using Wireshark to see what is happening


<h2> Network Equipment Purchased:</h2>

![image](https://github.com/user-attachments/assets/320d7727-94d3-4950-bce0-8966e3f68647)

N300 Wifi Router 2.4G 300Mbps




![image](https://github.com/user-attachments/assets/df14cdc4-55c2-4f2a-8b0a-d750711f1e01)


<br>
<br>
------------------------------------------------------------------------------------------
<br>

NETGEAR 5-Port Gigabit Ethernet Easy Smart Managed Essentials Switch (GS305E)


<br>
<br>


<h3> Cable Management</h3>

Before I can even start, I need to clean my "workstation," which has double the number of cables now.
Because of the temporary environment, I decided to use masking tape, which is easy to use and take off when needed.
I managed the 3 power cables (PC1, PC2, Monitor) together and had to first take it closer to PC2 since its a closed case and on the bottom of my desk. It was tricky getting it to be as tight as possible, as the other 2 cables came up and formed a Y shape when they connected to the monitor and PC1.

Due to there only being a double outlet, I have a surge protector that has combined all 3 power cables. I cannot have both PC's running simultaneously due to the sheer demand of power. So now, there is also the switch power cable, and two USB ports in the other outlet (this outlet has two USB cables (3.0, I think). These are managed to follow the shape of the desk then route through the back of a small hole in the router and then go their persepctive ways.

I also added an HDMI Splitter to ease the process of not removing cables and having the risk of damaging something.


<h1>Here is what the System looks like before</h1>

![image](https://github.com/user-attachments/assets/3faeb49d-306f-4158-9fb4-12c1c9460bb2)

<br>
<br>
<br>
<h1> now it looks like</h1>

![image](https://github.com/user-attachments/assets/0d459703-4f6f-4a9e-8d70-0bb5bd24a3e3)

![image](https://github.com/user-attachments/assets/8e0eceaf-7717-48d5-9b7c-c8d67f5ff758)




<h1> Setting up  the router</h1>

Okay, first, I had to clean the area where the router would go. I have cats, and there were little pieces of litter in the area.

I then had to cable manage the numerous devices present by the TV. I brought all the wires to an open shelf in the TV stand. Makes it easier to access them and not get eaten up by the cats

Time to start configuring

1. I connected the Cat 6 UDP Ethernet cable to the wall port and plugged it into the router. I then plugged the existing cable into LAN PORT 1 and connected the end to my gaming PC.

Now I am following the manual for the router
1. Connected to the wifi connection
2. Went to 192.168.0.1 on my browser, but this did not work
   **Solution** I went to settings -> Network and Wifi -> and clicked on the router connection. I then looked at the Default Gateway, which was 192.168.10.1
4. I am in the router now
   <br>
   ![{EC62EB27-40AD-4D13-9873-EC933D5F60CF}](https://github.com/user-attachments/assets/4c8ba3a2-3d6d-4fb8-a6a7-8de35e76b61f)\

5. Changing the Settings
   a. Changed the password to access the router itself
   b. Changed the Wifi name and password, and changed the encryption to WPA2-PSK
   c. Due to not having access to the router I have it set to DHCP
   d. I changed bandwidth to 40MHZ from 20MHZ. Since my connections are wired and the living room connections are wireless, there won't be any interference or blockage
   

