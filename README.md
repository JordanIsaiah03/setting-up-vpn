# Vitual Private Network (VPN)
<p align="center">
<img width="732" alt="Screenshot 2025-04-03 at 12 59 05 PM" src="https://github.com/user-attachments/assets/dbf1f869-a11c-4223-93cb-b0d3423b4301" />


</p>

<h1>VPN - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of using a VPN.<br />

<h2>Environments and Technologies Used</h2>

- A VPN (Proton VPN)
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>STEPS INCLUDED</h2>

- STEP 1 - Locate Local IP
- STEP 2 - Setting Up VM Using Azure
- STEP 3 - Locating IP Through VM (Canada Central)
- STEP 4 - Connecting to VPN Through VM
- STEP 5 - Locating IP Through VPN (Japan)

<h2>Installation Steps</h2>

STEP 1 - Locate your own personal IP address by going to "www.whatismyipaddress.com" which will be able to show you your local IP address. We will use this later as well. See EXAMPLE 1A below.

EXAMPLE 1A
<p>
<img src="https://i.imgur.com/qDgu5K6.png)" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Next we will set up a virtual machine on Azure. 
  
</p>
<br />

STEP 2 - Go to www.portal.azure.com and find Virtual Machines. See Example 2A looking at the Virtual Machine set up page. 

EXAMPLE 2A
<p>
<img width="1448" alt="Screenshot 2025-04-03 at 1 07 59 PM" src="https://github.com/user-attachments/assets/74340ffa-d59b-4749-91ec-72d962b812d7" />

</p>
<p>

Creating the Virtual Machine on Example 2B the VM as “Canada Central” and select that for the REGION as well. Ensure the other items are selected as shown in EXAMPLE 2B & 2C.

EXAMPLE 2B
<p>
<img width="848" alt="Screenshot 2025-04-03 at 10 40 45 PM" src="https://github.com/user-attachments/assets/7d579dd0-c284-456f-b213-f73fccf1bb35" />
<img width="1149" alt="Screenshot 2025-04-03 at 1 33 40 PM" src="https://github.com/user-attachments/assets/f639c0ab-bc6a-422a-98df-d95d71d915bd" />

</p>
<p>

For the Username and Password you can create your custom information, make sure you put it in notes just in case you forget it.
  
</p>
<br />

EXAMPLE 2C
<p>
<img width="792" alt="Screenshot 2025-04-03 at 1 41 26 PM" src="https://github.com/user-attachments/assets/d74fe576-b49d-4b9e-bc39-dba96b56bb8f" />

</p>
<p>

Select the “Networking” tab towards the top of the page and view EXAMPLE 2D inputs to match. 
  
</p>
<br />

EXAMPLE 2D
<p>
<img width="1062" alt="Screenshot 2025-04-03 at 10 45 52 PM" src="https://github.com/user-attachments/assets/42bfc6c2-18cb-44f9-bca6-56453a4b4541" />

</p>
<p>

Then select “Review and Create”, once it passes validation select “Create” at the bottom. 
  
</p>
<br />

NEXT: At the Virtual Machine we find that the IP to the Virtual Machine is “20.63.77.73”. See EXAMPLE 2E

EXAMPLE 2E

<p>
<img width="1112" alt="Screenshot 2025-04-03 at 10 50 52 PM" src="https://github.com/user-attachments/assets/3677d923-7a51-42ac-956c-16b43b73db98" />

</p>
<p>


STEP 3 – Log into VM & find IP Address

When we look up the IP address for this VM through www.whatismyipaddress.com we see that this VM is showing the location for Toronto, Canada (EXAMPLE 3C).
  
</p>
<br />

<p>
<img width="1192" alt="Screenshot 2025-04-03 at 11 18 54 PM" src="https://github.com/user-attachments/assets/ceb2ada8-9094-452b-b8ec-637fff63deb9" />
</p>
<p>

STEP 4 – CONNECTING TO VPN (Free Version)

Using the local computer go to protonvpn.com and create a free account. Once you are logged into your account, copy the URL from the Proton VPN website (EXAMPLE 4A) and then paste the URL to the VM web browser. 

  
</p>
<br />

EXAMPLE 4A
<p>
<img src="https://i.imgur.com/orO2O5y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Once you have logged into your Proton VPN account on the VM, you will select “Downloads” and choose to download the “Windows” version. Once the application Proton VPN is installed we will log in using the credentials we used when setting up a free account on Proton VPN. Then connect to the VPN through the installed app. See EXAMPLE 4B when this steps are completed.  
  
</p>
<br />


EXAMPLE 4B
<p>
<img width="1470" alt="Screenshot 2025-04-03 at 11 47 35 PM" src="https://github.com/user-attachments/assets/73d70800-0d25-455a-85fe-c34e62426dd4" />

</p>
<p>

On the left hand side of the VPN you can select a country where you want your VPN to be, the image below shows the VPN being connected to an IP in Japan. See EXAMPLE 4C
  
</p>
<br />

EXAMPLE 4C
<p>
<img width="1470" alt="Screenshot 2025-04-03 at 11 48 09 PM" src="https://github.com/user-attachments/assets/a2b84925-d927-4a98-a703-8685a2c4a0b9" />


</p>
<p>

Next we will look at the IP again using the VM browser now that we have connected the VPN to Japan. The website www.whatismyipaddress.com shows yet another IP address using the VPN from Japan. This is quite amazing.
  
</p>
<br />

EXAMPLE 4D
<p>
<img width="1191" alt="Screenshot 2025-04-03 at 11 48 50 PM" src="https://github.com/user-attachments/assets/fc6dc398-bb72-4751-9d63-5d77eae34f85" />
</p>
<p>

Looking at this exercise we see that we have utilized 3 different IP addresses just from your local computer to connect to the internet.
Home IP (USA): 137.103.51.136
Virtual Machin IP (Canada): 20.63.77.73
Virtual Machin IP VPN (Japan) 37.19.205.206
  
</p>
<br />
If you no longer need the VM, ensure to remove it from the Asure account for unwanted charges.

END OF TUTORIAL
