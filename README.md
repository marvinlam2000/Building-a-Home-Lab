# Detection Lab

## Objective
The Detection Lab project aimed to establish a controlled environment for simulating and detecting cyber attacks. The primary focus was to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test telemetry to mimic real-world attack scenarios. This hands-on experience was designed to deepen understanding of network security, attack patterns, and defensive strategies.

### Skills Learned

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

- Security Information and Event Management (SIEM) system for log ingestion and analysis. (Splunk)
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools to create realistic network traffic and attack scenarios.

## Steps
Step 1: Download Virtual Box onto user computer. User could verify download integrity by comparing the hash value provided on the website.
![Step 1 Download Virtual Box Snapshot jpg](https://github.com/user-attachments/assets/69e23cff-f8a3-47ec-b171-864256968c5c)

Step 2: Create and configure a Windows ISO image for Virtual Box to create user virtual machine.
![Step 2 Create and Configure Windows ISO image for Virtual Machine in Virtual Box jpg](https://github.com/user-attachments/assets/a22c3726-8577-4501-9312-9721c2b9c1f4)

Step 3: Download Kali Linux and configure settings. Creating Snapshots before implementing a change on the VM's.
![Step 3 Download Kali Linux and configure settings jpg](https://github.com/user-attachments/assets/9c27af42-ec45-483f-98d4-df090d8fa842)

Step 4: Create an account on Splunk in user VM.
![Step 4 Create Account on Splunk in your VM](https://github.com/user-attachments/assets/8ffbda9a-30cf-4559-8916-618e78532c0c)

Step 5: Install Sysmon64 and verify it is downloaded on the VM.
![Step 5 Install Sysmon64 and verify it is downloaded on VM jpg](https://github.com/user-attachments/assets/d2bb72d4-19a3-4065-9e1e-bbf34ae3b7b4)

Step 6: Create Snapshots on both VM and kali. Now change the default setting on both machines to Internal network instead of NAT. To protect the machines from your actual network.
![Step 6 change to internal network instead of NAT](https://github.com/user-attachments/assets/98f1ed29-b884-4988-8f6f-a831816ec1d6)

Step 7: Go into the VM and assign a static IP address and verify that the static IP is assigned by going to the command prompt.
![Step 7 assign static ip to vm](https://github.com/user-attachments/assets/9f265e82-fc76-4813-80ec-6eef1db68efb)

Step 8: Go to Kali and assign a static IP and verify that both machines are able to communicate with each other. User can verify that both machines can communicate with each other by pinging on the terminal. Take a snapshot once complete.
![Step 8 Assign Static IP to kali and verify commun](https://github.com/user-attachments/assets/9de78263-4108-4bc7-a28f-30fd18df3a1e)

Step 9: Go to terminal window in kali and type "nmap -A" and ping your virtual machine through the terminal in kali. Once finished use msfvenom command to create a malware. List out the payloads from msfvenom and choose a payload.
![Step 9](https://github.com/user-attachments/assets/81f79d0c-1653-4f61-b3f3-927cb62d1ce1)

Step 10: Generate our malware using meterpreter reverse tcp payload which is instructed to connect to the users local machine ip and port. And the file format will be in exe format.
![Step 10](https://github.com/user-attachments/assets/5deb255b-73e0-4ffb-9a23-34f4ba1ef2bb)

Step 11: Set payload on msf6 exploit to the payload that corresponses to the file created with the malware.
![Step 11](https://github.com/user-attachments/assets/510be439-9232-4b4e-8f3c-d4952e88ba4d)





