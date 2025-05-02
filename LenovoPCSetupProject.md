Hello!

This is to cover a pc I got from a family friend.

My code must have been deleted due to my error, so here is what has happened so far:

- I looked into the PC, no GPU, so it runs on the CPU.
- 12GB of DDR3-1600 MHZ
- Couldn't get into the user's account and so I wiped the whole thing clean

The reset process was stuck on 22%, so I forced it to shut down, and then I powered it on. Now it is Windows setup for Windows 10.

I forgot to disconnect the internet to bypass user creation, but it's fine. I made sure to limit every bit of control Microsoft can have since it's a very old computer.

I got into the system and looked around
- created two system accounts to eventually test password resets with

I updated the system to a new software version, and it's been slow, but it's expected. I will "Submit a ticket" to resolve the issue by installing a new SSD when the system clears.
Then it will teach me how to clone the OS and then move the boot to the SSD (need the UEFI for that). It finally updated, on to the next Phase

---------------------------------------------------------------------------------------------------------------------------------------------
Componnets of the PC
1. Download and installed CPU-Z to the desktop
2. Opened it and looked at the various components.

CPU: AMD A10-7800
Motherboard: Lenovo Bantry CRB PCIE 3.0 (8.0GT/s)
Memory: 1 stick of 12gb DDR3 1600Mhz, another 1 stick of 4gb DDR3 1600MHz
No GPU, graphics through the A10

Potential Upgrades in the future: 
- Simple SSD 
- Upgrade Ram to a higher DDR3 speed
- potentially upgrade CPU FAN and CPU?

I don't want to risk the various components when I am treating this as a workstation.
------------------------------------------------------------------------------------------------------------------------------------------
Installing Users
1. Go to Settings -> account -> Family and other users
2. I skipped adding emails and what not and added 2 users (User1111) and (User2222) and my own account. The other two are standard accounts and 
cannot have admin permissions.
----------------------------------------------------------------------------------------------------------------------------------------
<h2> Setting up remote IT access </h2>

Here, I plan to use my gaming pc as "IT Support" and the Lenovo as the "corporate" users.

1. Installed Anydesk to allow remote access due to not having windows pro
2. went into the command prompt as admin and created s user "ITadmin" with password
3. Then created a local group named "Administrators and added the ITadmin to it.
4. created 3 seperate corporte accounts (
   - corp_user1 corp123! /add
   - corp_user2 corp123! /add
   - corp_user3 corp123! /add
5. I then created a folder and two folders in it C:\CorpShared\DepA
   - Gave corp_user1 and corp_user2 all access
   - Gave corp_user 3 omly read access through the properites tab
   - ITadmin has full access
6. Created another folder called ITadmin, and restricted all desktop-lab\users from being able to access it.
7. I was having trouble putting permissions as an administrator and then not having the access I gave myself
   - Went back and changed owner and selected "replace ownership with all subfolders" and etc. This allowed me to get into my "IT Only" folder and restrict all other users from accessing it.
8. I went on to make 3 seperate folders in DepA. a corp1 corp2 and corp3 folders. I then restricted the access so that only ITadmin and the right user can read and write their needed folder.
   - 
