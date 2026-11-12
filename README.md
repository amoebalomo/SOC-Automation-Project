we will be building a home lab, but lets discuss it in a rough sketch on how it will look like using a website called draw.io

<img width="1360" height="680" alt="Screenshot 2026-11-07 173213" src="https://github.com/user-attachments/assets/c5bf789b-0bd7-490c-9268-fa46b0b2f595" />

And a small flowchart to understand the diagram better.

<img width="1362" height="678" alt="Screenshot 2026-11-07 173248" src="https://github.com/user-attachments/assets/f1c2d78c-72e9-4a07-a36e-9b238bcbf51b" />

We will be using this as a reference for our project.

Open a website and search Virtual box and download the latest version 

<img width="1361" height="723" alt="Screenshot 2026-11-08 163217" src="https://github.com/user-attachments/assets/ca1f61cf-e3e3-4908-be03-6326053b2a8b" />

Then alongside download windows 10 iso file

After that open your virtual box and click on new file. name it as "demo" and add the windows 10 iso image.

<img width="1365" height="722" alt="Screenshot 2026-11-08 165129" src="https://github.com/user-attachments/assets/ac2d788b-f9d0-411c-b88a-ebd00783ba3e" />

Then press the start button and wait for windows 10 to load and set it up for you

Then in windows 10 vm go to a browser and type Sysmon download. Make sure to extract that file.

After downloading it go to github and download a sysmonconfig.xml with raw coding and save as that file in downloads.

<img width="1359" height="737" alt="Screenshot 2026-11-09 170846" src="https://github.com/user-attachments/assets/c537fdcd-e413-47c2-ac8e-f0e19b18af4f" />

Then open Powershell and run the application as administrator.

<img width="1356" height="746" alt="Screenshot 2026-11-09 171147" src="https://github.com/user-attachments/assets/b19b2514-af26-4f3d-86cf-b4b02341653f" />

Check and make sure that the file directory of sysmon is downloaded through powershell. Now that our Sysmon is downloaded, we have to now install wazuh and create a new project.

<img width="1365" height="767" alt="image" src="https://github.com/user-attachments/assets/31bbe159-7f75-419b-b114-b21b75ffd23b" />

Click on Droplet icon make make arrangements for your own comforts. by selecting your region and make sure to select the package with 164gb space and 4tb sharing. and select Ubuntu as your OS. and create your own unique password since it will be sent publicly.

Now create your own firewall using the same application within.

<img width="1359" height="766" alt="Screenshot 2026-11-09 172920" src="https://github.com/user-attachments/assets/6358eb47-b2f8-4b6d-93bf-344a556b9cfd" />

create your own name and your own TCP option. and create your own ip address by going through a website and type "whatsmyipaddress" whic will enable and show your personal ip address which you can add in your selection.

<img width="1272" height="579" alt="Screenshot 2026-11-09 173312" src="https://github.com/user-attachments/assets/2a8866d0-16c9-4c72-9377-d05d4b56a14f" />

<img width="1364" height="764" alt="Screenshot 2026-11-09 173636" src="https://github.com/user-attachments/assets/0f990ceb-3d45-49c6-99f5-2b4ab7cbabe1" />

After that a option will appear which says to choose your own server and configuration. it is important to just press enter.

<img width="1359" height="765" alt="Screenshot 2026-11-09 173745" src="https://github.com/user-attachments/assets/2b856b71-de92-4940-a9c8-04e598a123e4" />

This is where it will actually start working and make sure to enter this specific code.

<img width="1365" height="765" alt="Screenshot 2026-11-09 173828" src="https://github.com/user-attachments/assets/e3adc6c5-97bb-48e5-8a1e-317444271e77" />

This will ensure that you have everything saved and if your open a website with your specialised IP address, it will lead to Wazuh.

Now we will configure Wazuh and Hive.

<img width="1351" height="746" alt="Screenshot 2026-11-11 161638" src="https://github.com/user-attachments/assets/4f38db04-7624-44a3-b3c9-845a77a161c6" />

Then you add your Personal IP address on listen_address. 

<img width="1355" height="767" alt="Screenshot 2026-11-11 162051" src="https://github.com/user-attachments/assets/d2761b28-63fd-4171-acc1-60b1e6d2bda0" />

now we have to stop our Cassandra and end our old service and start with our new service and rewrite it oncde more instead replacing it with "status".

<img width="1361" height="696" alt="Screenshot 2026-11-11 162851" src="https://github.com/user-attachments/assets/79f3aa0c-2b44-4d40-84df-42709c151a5c" />

v<img width="1345" height="717" alt="Screenshot 2026-11-09 174035" src="https://github.com/user-attachments/assets/c91fca58-5ff0-4cd1-b9b9-5664bf0d0c75" />

make sure you add your Hive IP on your host server, uncomment your http.port and then we start and enable the hive. And then we are shown with the Hive page.

<img width="1363" height="758" alt="Screenshot 2026-11-11 171024" src="https://github.com/user-attachments/assets/a397b44c-d4d5-4e40-be4d-2c6c0bed28c4" />

Then you go to Wazuh and add and agent, click the Windows as os option since we are working on windows. and add your public ip. And in the end it will show the number of agent and active agent too.

Now we will configure the Wazuh even more and send telemetry containing Mimikats. The configuration of Wazuh will be under program files x86 and we will use the file ossec.config and open the file and open it in notepad. in order to download and open Mimikats, you will have to go to settings and privacy and disable virus threat and protection.

And then add a separate folder where you can download Mimicats. Where next you have to extract all of the files from that folder.

<img width="1242" height="674" alt="Screenshot 2026-11-12 165241" src="https://github.com/user-attachments/assets/23335ba2-2bf0-4649-bee2-2841707a458e" />

Then open powershell and try running Mimicatz.

<img width="1365" height="767" alt="Screenshot 2026-11-12 170121" src="https://github.com/user-attachments/assets/f4d6aadf-f9d1-48f6-ba95-9144aec0023b" />

And configure ossec so we can start working. by opening Wazuh CLI and type the shown coding.

<img width="1360" height="765" alt="Screenshot 2026-11-12 171215" src="https://github.com/user-attachments/assets/9ebb16f3-72ad-45f2-9b56-e1d65093cb2d" />

<img width="1363" height="710" alt="Screenshot 2026-11-12 171638" src="https://github.com/user-attachments/assets/5f199957-bb31-4797-bed9-53fd22a99beb" />

<img width="1363" height="710" alt="Screenshot 2026-11-12 171638" src="https://github.com/user-attachments/assets/2de54da6-69e7-4915-a50f-fcac0d3998ca" />

And thats the way you fully set up a Wazuh properly.
