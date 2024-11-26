## Demonstration-of-a-DoS-Attack

**Introduction**

This document demonstrates a Denial of Service (DoS) attack using the Metasploit framework on Kali Linux. The goal of this attack is to overwhelm a target machine or service with traffic, rendering it unavailable.

## Tools and Setup

- **Operating System**: Windows 11 (host) and Kali Linux (penetration testing).
- **Metasploit Framework**: Used for executing the DoS attack.
- **Target**: Hypothetical IP address or machine.
-----

## Steps to Execute a DoS Attack

**1. Update the System**
   
Before beginning, ensure that your system packages are up-to-date. This step is crucial for maintaining the latest versions of Metasploit and other tools.

Run the following command in the terminal:

**sudo apt update**

   ![image](https://github.com/user-attachments/assets/d9b96216-702d-4b35-9bd1-7d7959a3bfca)


## 2. Start Metasploit
   
Open the terminal and launch the Metasploit framework by typing `msfconsole`.

   ![image](https://github.com/user-attachments/assets/41a1db46-1515-43be-a566-2e777cf76bdc)

## 3. Search for a DoS Module
   
Use the command **`search flood`** to find a suitable DoS module.

   ![image](https://github.com/user-attachments/assets/a528a3d1-3a45-4fae-a3a7-e49d9f0a805b)

## 4. Configure the DoS Module
   
Use the following commands to configure the module for the attack:

- `use auxiliary/dos/tcp/synflood`
  
- `set RHOSTS <target_ip>`
  
- `set RPORT <target_port>`

  ![image](https://github.com/user-attachments/assets/d0efc1ae-4f90-4cd4-875f-f3184fc63bc8)

  ![image](https://github.com/user-attachments/assets/f4b7f9a9-c8d2-4ba5-aba7-f8b8c324c9cc)


## 5. Launch the Attack
   
Run the module using the **`run` command**. This initiates the DoS attack against the specified target.

 ![image](https://github.com/user-attachments/assets/4251c9b0-44aa-499f-87f6-fe5170631668)

 ## Results
 
The attack generates a large volume of SYN packets, overwhelming the target's resources. As a result, the target service may become unresponsive. This showcases the impact of a DoS attack in a controlled environment.

![image](https://github.com/user-attachments/assets/7250896b-bce3-4dbf-ad16-8d3fda901a7b)

![image](https://github.com/user-attachments/assets/523ef806-fb1b-451d-bc76-f255d0521a74)

![image](https://github.com/user-attachments/assets/f78b6494-fe06-4a57-910b-1623bf53f087)

![image](https://github.com/user-attachments/assets/e2a9724b-9e05-4106-a4e2-285ff4232954)






 





