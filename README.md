<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Installation Steps</h2>

![1](https://github.com/user-attachments/assets/46d8175a-5938-4da4-9396-41ef69260017)


<p>
The first step in installing OSTicket was to utilize Microsoft Azure (virtual machine). Begin by setting up your virtual machine.
</p>
<br />

![2](https://github.com/user-attachments/assets/ad859a96-3ffe-47a8-9d96-4b58b87dfe3d)

<p>
Next, open up your Remote Desktop Connection application (Windows Application) and begin by entering your virtual machine's IP address to establish the remote connection.
</p>
<br />

![3](https://github.com/user-attachments/assets/6fb47020-021d-4c27-a151-620afbe3532e)

<p>
Once you establish a connection to your virtual machine, you will want to head into Control Panel > Programs and select " Turn Windows features on or off." Once in, select Application Development Features and turn on "CGI."
</p>
<br />

![Capture](https://github.com/user-attachments/assets/37f250d9-3c2e-4ad8-b6eb-7fa3619b4248)

<p>
From the “osTicket-Installation-Files” folder, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi) & Rewrite Module (rewrite_amd64_en-US.msi) 
</p>
<br />

![image](https://github.com/user-attachments/assets/5c02c8ee-513e-4028-9ffa-4b80b690b7ea)

<p>
Locate your C: drive folder and create a new folder called "PHP."
</p>
<br />

![image](https://github.com/user-attachments/assets/24419361-b5ed-4708-a329-ed5ab7818ed0)

<p>
Extract the "php" folder located in the OSTicket-Installation folder into your newly created PHP folder located in the C: drive.
</p>
<br />

![5](https://github.com/user-attachments/assets/d680d6d2-fe36-4e26-bff7-50822994e3b8)

<p>
Install both VC+redlist x86exe & My SQL 5.5.62 from your OSTicket Installation Folder
</p>
<br />

![7](https://github.com/user-attachments/assets/6175a48e-b62d-4409-a12e-10b97f5a962c)


<p>
Open up the Internet Information Services (IIS) Manager, please be sure to run it as ADMINISTRATOR. 
</p>
<br />

![image](https://github.com/user-attachments/assets/eb533f0c-b700-4747-bd24-f8a0c7f4268a)

<p>
In the (IIS) open up the PHP manager and click on "REgister new PHP version" then locate your created PHP folder in your C: drive.
</p>
<br />

![image](https://github.com/user-attachments/assets/fb718c35-fe4a-43d8-a769-1fd9f6597c8d)

<p>
In your (IIS) Stop and Start the server
</p>
<br />

![image](https://github.com/user-attachments/assets/83fc1e05-60c0-4d0d-a412-df6fc2d47498)

<p>
Head back to the OSTicket Installation Folder and click on this folder and extract the files.
</p>
<br />

![image](https://github.com/user-attachments/assets/72c76a12-80be-4307-870d-72cfef981206)
<p>
Open Windows C: > inetpub > wwwroot, once you have done this copy the "upload" folder from your recently extracted file and paste it into wwwroot.
</p>
<br />

![image](https://github.com/user-attachments/assets/a1ee137b-585f-4a8f-bbac-7aa5ac03c00d)

<p>
  Once it has copied onto the wwwroot folder, rename the "upload" folder to "osTicket."
</p>
<br />

![image](https://github.com/user-attachments/assets/fb718c35-fe4a-43d8-a769-1fd9f6597c8d)

<p>
Repeat: In your (IIS) Stop and Start the server
</p>
<br />

![image](https://github.com/user-attachments/assets/ae107b94-2f69-4627-90c9-b4c0addbea1a)
<p>
Head to Sites > Default Web Site > osTicket, click on Browse.
</p>
<br />

![15](https://github.com/user-attachments/assets/73b878e0-3f40-4851-992c-85dda9d14141)


<p>
Congratulations! You have now installed OsTicket.
<br />
