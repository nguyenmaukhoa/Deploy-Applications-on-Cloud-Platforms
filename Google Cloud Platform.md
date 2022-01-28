# Deploy Applications on [Google Cloud Platform (GCP)](https://cloud.google.com/)

# 1. Setup an account
## 1.1 On the main page, click **Get Started for Free**
<img width="400" alt="Screen Shot 2022-01-24 at 11 55 30 AM" src="https://user-images.githubusercontent.com/42128166/150854893-02b19744-3586-4a97-a4ed-48e55c9a1aa4.png">

## 1.2 Login with your account or you can create a new one
<img width="400" alt="Screen Shot 2022-01-24 at 12 05 25 PM" src="https://user-images.githubusercontent.com/42128166/150856336-823847b3-cf8a-4129-a5d2-74230fb8042a.png">

## 1.3 Create new account
<img width="400" alt="Screen Shot 2022-01-24 at 12 14 59 PM" src="https://user-images.githubusercontent.com/42128166/150857651-d6431fff-90ab-4aab-86ca-eec48db834ed.png">

## 1.4 Account Verification
<img width="400" alt="Screen Shot 2022-01-24 at 12 33 07 PM" src="https://user-images.githubusercontent.com/42128166/150860153-9f47a0f3-8d2c-4368-9b92-dd796bf15fc6.png">

<img width="400" alt="Screen Shot 2022-01-24 at 12 36 38 PM" src="https://user-images.githubusercontent.com/42128166/150860642-87fec00d-2c2a-4492-98e1-9f9746bc56bc.png">

<img width="400" alt="Screen Shot 2022-01-24 at 12 44 22 PM" src="https://user-images.githubusercontent.com/42128166/150861690-fef1bd19-4ede-4a6a-8de8-899c25e51118.png">

# 2. Create a project
## 2.1 New Project
A project is automatically created when you log in for the first time

![Screen Shot 2022-01-27 at 10 28 35 PM](https://user-images.githubusercontent.com/42128166/151483251-b3e22cde-9c5d-419c-a289-7af0774c8367.png)

To create a new one, click on **My First Project**, then choose **New Project**

![Screen Shot 2022-01-27 at 10 31 36 PM](https://user-images.githubusercontent.com/42128166/151483307-d53773d4-ca04-4201-baf6-7222d3cfb086.png)

Enter project name, then click **Create**

![Screen Shot 2022-01-27 at 10 32 56 PM](https://user-images.githubusercontent.com/42128166/151483329-6e0d574a-0130-4717-a9bb-ef4070578b8b.png)

## 2.2 Create Compute Engine API
Choose **Compute Engine**, then **VM Instances**

![Screen Shot 2022-01-27 at 10 51 20 PM](https://user-images.githubusercontent.com/42128166/151484303-bf7e386e-9c09-4a4e-b4df-42ebf07d377f.png)

Choose the recent project created

![Screen Shot 2022-01-27 at 10 53 35 PM](https://user-images.githubusercontent.com/42128166/151484543-2019ed41-4816-4522-8763-b63d59de3c0e.png)

Click **Enable**

![Screen Shot 2022-01-27 at 10 55 11 PM](https://user-images.githubusercontent.com/42128166/151484619-80e9ef00-f3b7-46ef-a1ef-b025d7cb74bc.png)

Choose **Create Instance**

![Screen Shot 2022-01-27 at 10 59 15 PM](https://user-images.githubusercontent.com/42128166/151485041-00a4f2b2-3a83-4513-b3b8-335f145b2fd5.png)

Leave all default, but **N1** for **Machine Configuration**

![Screen Shot 2022-01-27 at 11 02 12 PM](https://user-images.githubusercontent.com/42128166/151485319-0b713f81-1921-4e56-bd18-8c08e40a077c.png)

Click **Change** in **Boost Disk**

![Screen Shot 2022-01-27 at 11 04 22 PM](https://user-images.githubusercontent.com/42128166/151485614-3e670d33-d06a-4ca3-a852-b54b1a732194.png)

Choose configurations as below then click **Select**

![Screen Shot 2022-01-27 at 11 07 10 PM](https://user-images.githubusercontent.com/42128166/151485705-5671f0ca-0b6b-4af8-aef1-1fae9a1c44e6.png)

Finally, Click **Create** at the bottom

![Screen Shot 2022-01-28 at 11 25 43 AM](https://user-images.githubusercontent.com/42128166/151584098-77449f50-0c62-4f9a-9d26-cee0d7d2138d.png)

## 2.3 VM Configurations

To access the VM, and work on the terminal, click on **SSH**
(Click **Connect** if a pop-up window display)

![Screen Shot 2022-01-28 at 11 28 03 AM](https://user-images.githubusercontent.com/42128166/151584458-16744709-fd69-43f6-afb2-d8328d9b5b00.png)

First command: **sudo apt update**

![Screen Shot 2022-01-28 at 11 30 26 AM](https://user-images.githubusercontent.com/42128166/151584854-e67609dd-e621-4e68-a8cb-50e327d2f160.png)

Install **python pip**

![Screen Shot 2022-01-28 at 11 31 30 AM](https://user-images.githubusercontent.com/42128166/151585013-e9eadb2f-4f3a-4833-8c6b-da7d53ad9da1.png)

Install **numpy**

![Screen Shot 2022-01-28 at 11 34 42 AM](https://user-images.githubusercontent.com/42128166/151585553-e497724d-1f18-4830-99c9-1a9a59dfbc29.png)

Install **OpenCV**, headless version since we're working on the remote machine

![Screen Shot 2022-01-28 at 11 39 48 AM](https://user-images.githubusercontent.com/42128166/151586354-56dd24ca-f351-43e9-a3ee-455a7c725f9c.png)

Install **Streamlit** for the purpose of deploying the sample project

![Screen Shot 2022-01-28 at 11 41 58 AM](https://user-images.githubusercontent.com/42128166/151586679-469ddb88-2b97-40ff-8e9a-36e2615f3ff5.png)

## 2.4 Configure the sample project

We are going to use the **Face Detection Demo** from **Kromydas** on **GitHub**
https://github.com/kromydas/streamlit-demo-face-detect

Clone the project

![Screen Shot 2022-01-28 at 11 48 32 AM](https://user-images.githubusercontent.com/42128166/151587690-7c5a413d-6dd9-4796-b367-93c8ecc39ffc.png)

To run the application

Move directory to the project folder

![Screen Shot 2022-01-28 at 11 51 52 AM](https://user-images.githubusercontent.com/42128166/151588197-20ea56b6-c213-4514-bd79-b0c996c9a712.png)

Run Streamlit command with the character **&** to enable the project running background. So when we turn off the command line, the app is still running.

![Screen Shot 2022-01-28 at 11 52 43 AM](https://user-images.githubusercontent.com/42128166/151588309-39a4f5b2-b736-4c9f-bf92-b23ac01d3f31.png)

Click on the External URL: **http://34.125.206.176:8501**
This link doesn't work until we configure the firewall in the virtual machine

![Screen Shot 2022-01-28 at 12 00 04 PM](https://user-images.githubusercontent.com/42128166/151589475-b0e314d8-8db3-4201-bcc7-8fa66d387fd0.png)

## 2.5 Configure the Firewall rule

From additional options, choose **View Network Detail**

![Screen Shot 2022-01-28 at 12 02 58 PM](https://user-images.githubusercontent.com/42128166/151590064-a199d7fa-606b-45af-8e5c-4c9b3e9b5069.png)

Select **Firewall**, and choose **Create Firewall Rule**

![Screen Shot 2022-01-28 at 12 04 20 PM](https://user-images.githubusercontent.com/42128166/151590206-be81cb39-5fdd-46f0-9de4-1bdec19b39b6.png)

Enter rule name
![Screen Shot 2022-01-28 at 12 05 28 PM](https://user-images.githubusercontent.com/42128166/151590336-9b74fa70-b659-4306-84a7-125f401ff8bc.png)

Choose **Target**

![Screen Shot 2022-01-28 at 12 06 41 PM](https://user-images.githubusercontent.com/42128166/151590556-4b119672-fa65-4d68-99db-aa509488865c.png)

Enter **0.0.0.0/0** as the IP. This means we allow connections from anywhere on the internet

![Screen Shot 2022-01-28 at 12 07 34 PM](https://user-images.githubusercontent.com/42128166/151590649-cba792d1-2e9b-4112-9a9e-a9881dca078e.png)

For Protocols, choose **TCP** and enter **8501**

![Screen Shot 2022-01-28 at 12 08 58 PM](https://user-images.githubusercontent.com/42128166/151590896-d3bcfac6-9cd6-49cc-a44a-0180b7dfbf57.png)

Click **Create** button afterall

![Screen Shot 2022-01-28 at 12 10 02 PM](https://user-images.githubusercontent.com/42128166/151591083-57c3e562-1c90-4152-adcf-4cfe00d751e7.png)

## 2.6 Check the sample project

Go back to the browser and refresh the page **http://34.125.206.176:8501**

The project now displayed correctly

![Screen Shot 2022-01-28 at 12 11 35 PM](https://user-images.githubusercontent.com/42128166/151591314-b9b4571f-ae4b-40c1-8b25-9aaf6c2574b3.png)

Go ahead and upload an image to test the application

![Screen Shot 2022-01-28 at 12 14 05 PM](https://user-images.githubusercontent.com/42128166/151591659-56a65681-4edf-45ec-96fd-496ada5f0d51.png)

we have configured and deploy the sample project successfully

## 2.7 Stop the project

Choose **VM Instances** and click **Stop** in the additional options

![Screen Shot 2022-01-28 at 12 19 40 PM](https://user-images.githubusercontent.com/42128166/151592689-27786f69-59ad-4b5f-82b2-53935fe2e609.png)


