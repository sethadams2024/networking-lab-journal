
# networking-lab-journal
This is a journal to log the various networking projects, labs, and certification learning I am doing daily.

Ultimate Goals of my journal:
- Get into networking
- Break into the IT field.
- Show the knowledge I have gained, my mistakes, and much more.

Day 1
- I was able to purchase some items from a garage sale:
  1. D-Link DIR-615 Okayless N router. It has 4 LAN ports and wireless connectivity.
  2. Device of Cat 5e. I needed another cable to use the D-Link and my PC with Ethernet.
  3. A new Type C hub that offers Ethernet connectivity for my Surface Pro 7. I did not have one with my other version.
  4. A NetGear Base Station VMB3000. I now understand that this is useless unless I make huge changes to its items.
 
  Here are my Plans for the upcoming weeks
  - Take out the insides of the NetGear and put a Raspberry Pi in it to detect my internet traffic by hiding it as another device.
  Connect the D-Link, configure it in different ways, and learn about what it can do. I also saw that I could flash something onto it to make it more powerful.
  - I am also a Master's student in Information Science, and that is a higher priority.
  - I am also studying for A+ certification, and doing Cisco's "Network Technician" Badge course.
 

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Setting up the D-Link**
- Plugged the main Ethernet into it:
- Plugged LANN1 into my gaming pc to configure it
      - Interestingly enough, it started working immediately. I don't understand why yet.
- Ok, I cannot access the configuration menu and need to reset the thing. The device says not to change the password, but the previous owner did otherwise.
- Figured it out, held the reset for 15 seconds with my new screwdriver set "Mechmax" highly recommend for small screws and smaller needed tools.
- After configuring it as a Dynamic IP, the system is up. Due to being very old, I am maxed at roughly 94 Mbps.

Configuring various settings
- I had to update the time, so I found how to set the NTP (Network Time Protocol) to time.google.co,m and it connected!
- Have to update it, which means I need to save the config before updating

UPDATE:
THAT WAS THE WORST MISTAKE I HAVE EVER MADE. I bricked the router and cannot access it at all. I have tried just about everything, and nothing is working to get it back online

TLDR: I bricked and killed my first router on the first day. 


Now that it's dead, basically, I am going to open it and see the parts of it. I will put screenshots in the wiki!
Update: It has been taken apart. That is it for Day 1!

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Day 2
- Today, I was very busy with other priorities. But I made progress nonetheless.
- I finished the RAM chapter of A+, now onto BIOS tomorrow. I need to read around 20 pages a day if I want to be ready by June 17.  Actually, with my honeymoon, I need to push it to July
- I also bought new network equipment. I bought a NETGEAR 5-Port Gigabit Ethernet Easy Smart Managed Essentials Switch (GS305E). This time I will not brick it!
- I got a N300 Wifi Router 2.4 GHz Easy Setup. Up to 300Mbps. It's not great, but I still want to try setting it up in my bedroom.
- Side note: Want to slowly upgrade my old gaming PC with parts during this journey. Stay Tuned. On to day 3!

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Day 3 04.13.25
I redid my RAM quiz and got 10/10. I wonder why I answered these questions a different way. 

I completed the Udemy Firmware section. On to the book now. I never realized that the UEFI was an updated BIOS; I thought it was just a BIOS. I also didn't know about POST, Boot passwords, and how the power good wire for the CPU to start BIOS (UEFI)

I have other items to do, I shall return.
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Day 4 4.14.25

Mark this day as the day I change and become full-on into this networking thing

A+: Finished Firmware Section and now learning Motherboards
Cisco Network Technician Course: Learning about setting up home networks
Master's Class: I am starting tomorrow for Module 3
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
Day 5 4.15.25

Didn't get to do much, but I started chipping away at module 3 on my Master's!
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Day 6 4.16.25
Got the (new) PC from a family friend, now I will try to get into the OS and start learning. It is taking forever to reset.
Finally reset, now just organizing my desk for two PC's. 
I think it might be best to look into VirtualBox and even a ticketing service, and make fake tickets and organize my thoughts as I learn.
------------------------------------------------------------------------------------------------------------------------------------------------
Day 7 (1 week) 4.17.25
Network equipment came in last night, and now I am in the process of setting it up.
- Due to having two PC's and now 2 HDMI cables, 2 power cables, and 2 Ethernet cables. I had to use some tape to tie it together and cable manage. 
- I will start configuring the equipment tomorrow. Please look at the "Creating a LAN" Project folder.
- I decided to turn from my Udemy course and follow Professor Messor when it comes to learning A+
 
[Creating my LAN Project](/CreatingALAN.md)
------------------------------------------------------------------------------------------------------------------------------------------------
Day 8 4.18
- Set up the switch and the Wifi Router (now a dumb AP).
- Working on Defensive Security Intro from TryHackMe (completed)
- Build a home network module in the "Network Tech" cisco learning academy course
------------------------------------------------------------------------------------------------------------------------------------------------
Day 9 4.19
- I completed module 3 of my Advanced Programming Class for my Master's and am about halfway through.
- Started going full into Professor Messor and the textbook. I watch the videos, take notes of items I do not know, then skim and document anything new as I go.
- I finished the "Defensive Security Intro" for Try Hack Me, now on to "What is networking
- Considering taking the coursecareers IT Support course.
--------------------------------------------------------------------------------------------------------------------------------------------
Day 10 4.20
- Just about wrapped up Section 1 of 1101. I am about 20 pages from the end of the book
- I plan on watching the study sessions over the past 3 years after I finish Module 2, so I can start practicing.
- I want to get a thumb drive to install Linux on, so that I can dual-boot the Lenovo workstation pc.
- Have not found a ticketing platform yet. I will also install VirtualBox soon to test it out.
  My main priorities right now:
  1. Pass my master class
  3. Pass Core 1 and 2 of A+. A+ will help me in the right direction for the lab pc.
- Finished Section 1 of 1101, I got about 12.5% out of the possible 15% on the quizzes at the end of each chapter. On to networking, which is 20%. I think my biggest challenge is port #'s, but I need to study them on Anki
- Completed "WHAT IS NETWORKING" by tryhackme
  
---------------------------------------------------------------------------------------------------------------------------------------------
Day 11 4.21
- Passed Module 3 of my R class
- Started the CourseCareers IT Support course. I am excited to learn the different parts that I would use in entry-level IT.
---------------------------------------------------------------------------------------------------------------------------------------------
Day 12 4.22
- Started my journey into hardware and the networking portions of the Course Careers (around 25% done)
- Downloaded VirtualBox. [Installing Virtual Box on Surface Pro](/Installing_Virtual_Box.md)


  ![image](https://github.com/user-attachments/assets/b11e0cc7-bbcf-4443-ab38-bb463ae5447c)

-----------------------------------------------------------------------------------------------------------------------------------------------
Day 13 4.23

I started the lab section of CourseCareers. I installed and worked on virtual machines (through remote desktop) inside Azure!

I also installed Wireshark to see all the types of traffic involved.
![image](https://github.com/user-attachments/assets/92dbce8f-597e-41b2-a5c3-5b7cc9690a47)

![image](https://github.com/user-attachments/assets/627e1270-48a1-4e7e-b352-5cd88bcbe2f0)


![{C5CE4058-17DF-4E8F-8D43-DFBAEB04361E}](https://github.com/user-attachments/assets/633621d2-cd36-4405-8088-094a6d4b0bd4)
<br>
<br>
<br>
-------------------------------------------------------------------------------------------------------------------------------------------
Day 14 4.24

Started working on module 4 of my master's class

Installed and created my ticketing system with osTicket. I had to use the virtual machine's web server 172.0.0.1. It took going into multiple file systems, configuring access, and many items to get it up and working properly.

I also finished Module 5: Communication Principles of the Networking basics in the Network Technician course from Cisco.


![{93766C3E-9DD6-425F-A07B-B7656D6E8866}](https://github.com/user-attachments/assets/a748e17d-2fe0-4723-a0f5-d26019182c95)


![{2CBC338F-2122-43DA-B17B-C4122B65307D}](https://github.com/user-attachments/assets/98a95fa4-abd0-474b-9890-dd550a5808d1)

-----------------------------------------------------------------------------------------------------------------------------------------\

Day 15 4.25

- Finished the VPN lab with Proton VPN. I created a virtual machine and tested the IP difference once the vpn was activated, etc.
- Completed the CIA Triad section of the security principles free module on TryHackMe.
-------------------------------------------------------------------------------------------------------------------------
Day 16 4.26

- Worked on A+ certification and completed module 4 of my master's class.
--------------------------------------------------------------------------------------------------------------------
Day 17 4.27
- Finished and started module 3 (hardware) of A+. I have started taking practice exams as I go deeper into the course.
----------------------------------------------------------------------------------------------------------------------
Day 18 4.28

- I continued the 3.0 hardware section. I am wondering if I should go for N+ instead of CCNA, as many locations around me want N+. Getting the triad is crucial.
--------------------------------------------------------------------------------------------------------------------
Day 19 4.29

- Now, should I go from A+ to Sec+? Sec+ opens more doors, and I am learning networking from the Cisco Networking Academy. I can then go back to N+ later.
I am almost done with module 3 of A+.
-------------------------------------------------------------------------------------------------------------------
Day 20 4.30
I have finished Module 3 and Module 4 of 1101 and am now on to troubleshooting. I think I will take Core One in mid-June, as I need to complete it as soon as possible.
- I also redid my resume to include some projects. 
-----------------------------------------------------------------------------------------------------------------
Day 21 5.1

- Did not accomplish much except complete week 5 of my class and did a+
--------------------------------------------------------------------------------------------------------------
Day 22 5.2
- Decided to start doing labs on my lab computer. I went on to create some [roll access](/roleaccess.md)
- Worked on CourseCareers active directory.

  ## Day 24 will not exist, getting married.
------------------------------------------------------------------------------------------------------------
Day 23 5.3
- Continued into module 5 of CompTIA Messer videos
----------------------------------------------------------------------------------------------------------
Day 26 5.6 
- Finished the Messer videos!
- On to practice tests for the next month
--------------------------------------------------------------------------------------------------------------
Day 27 5.7
- Going to do practice test 1 today and cover what went wrong. ONLY GOT 5 WRONG! 3rd time is the charm
- I completed the career course, and I am now just going to run through it again and prepare for the final exam.
-----------------------------------------------------------------------------------------------------------
Day 28 5.8
- Took test #2 (attempt 2) and got a 95! But it included parts that are not on the exam (TFTP) is port 69.
- 
