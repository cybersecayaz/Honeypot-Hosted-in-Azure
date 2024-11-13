# T-Pot Honeypot Deployment on Azure Cloud

## Objective
The **T-Pot Honeypot Deployment** project aimed to deploy an advanced honeypot in the Azure cloud environment to simulate vulnerable systems and detect potential cyber threats. This project provided hands-on experience in configuring Linux systems, network settings, and cloud security. It also enhanced my expertise in threat detection through active monitoring and analysis of honeypot data, allowing me to observe how attackers exploit vulnerabilities to compromise systems.

### Skills Learned
- **Proficiency** in Linux OS and command-line interface for configuration and administration.
- **Advanced knowledge** of VM deployment and network configuration within Azure Cloud.
- **Understanding of network security principles** and protocols, including TCP/IP, SSL/TLS, and SSH.
- **Experience configuring access controls** to secure network traffic in Azure.
- **Expertise in implementing robust security measures** to protect sensitive information and mitigate security risks in cloud environments.

### Tools Used
- **T-Pot honeypot** for simulating vulnerable systems and capturing attack data.
- **Azure Cloud Platform** for deploying and managing the honeypot environment.
- **Linux OS** as the foundation for T-Pot deployment and configuration.
- **PuTTY** for remotely managing the Azure Linux VM via SSH, allowing installation and configuration of T-Pot.

## Steps

### Step 1. Configured and Deployed the VM in Azure Cloud
- Created a new **virtual machine (VM)** on Azure, selecting a **Linux-based image** as the operating system to run the T-Pot honeypot.
- Configured the VM’s settings, including the network interface and storage, to ensure it is ready for honeypot deployment.

**Screenshot 1: VM Deployment in Azure**  
**Ref 1:** Screenshot showing the virtual machine setup and configuration process within Azure.  
![image](https://github.com/user-attachments/assets/2c755366-bcf7-4d10-a20e-c708ace0506b)


### Step 2. Set Up Security Group
- Configured the **security group** to manage inbound and outbound traffic to the VM.
- Allowed all IPs to access the VM by opening a wide range of ports (IP 1 - 65535), simulating an environment vulnerable to attack.

**Screenshot 2: Security Group Configuration**  
**Ref 2:** Screenshot of the Azure security group configuration with port settings to allow access from all IP addresses.  
![image](https://github.com/user-attachments/assets/9617c2c6-5e86-4e1c-840e-58b30fef780e)


### Step 3. Installed T-Pot Honeypot Using PuTTY
- Connected to the newly created Azure VM using **PuTTY**, a terminal emulator, to access the **Linux command-line interface (CLI)**.
- Installed **T-Pot honeypot software** from the Github repository on the VM using the terminal commands. PuTTY allowed remote interaction with the VM, ensuring the honeypot was set up properly.

**Screenshot 3: Installing T-Pot via PuTTY**  
**Ref 3:** Screenshot of the terminal showing the installation of the T-Pot honeypot using PuTTY.  
![image](https://github.com/user-attachments/assets/186a2aa6-5dc3-4872-a608-eb2501317bf0)


### Step 4. Analyzed the Traffic Based on the Dashboard T-Pot Has
Once T-Pot was installed and running, I used T-Pot dashboards such as **Attack Map** and **Elasticvue** to actively monitor the network traffic and attacks on the honeypot system.

- **Attack Map** provided a real-time visual representation of attack attempts, showing the geographic location of attackers and their IP addresses. This helped in understanding where the threats were coming from globally.

**Screenshot 4: Attack Map Displaying Real-Time Geographic Distribution of Attacks**  
**Ref 4:** Screenshot showcasing the Attack Map dashboard, visualizing the geographic locations of incoming attack attempts, providing insights into the global spread of threats targeting the honeypot.
![image](https://github.com/user-attachments/assets/771e50c5-b949-4607-85b8-e2f5268f3371)
  
- **Elasticvue** allowed me to view and analyze the data stored in the Elasticsearch database, where attack logs and information about the interactions with the honeypot were stored. I could see detailed insights about the attack attempts, including targeted IP addresses and types of malicious activity.

**Screenshot 5: Elasticvue Displaying Detailed Attack Logs and Interaction Data**  
**Ref 5:** Screenshot showing the Elasticvue dashboard, providing in-depth analysis of attack logs and interactions with the honeypot, including targeted IP addresses and attack types.
![image](https://github.com/user-attachments/assets/4765e6ee-2362-4836-83ed-b9d78daeb6ee)


**The dashboard provided real-time insights into:**
- The types of attacks being attempted.
- The location of the attackers.
- Which honeypots were being targeted the most.
- The nature of the attack attempts (e.g., brute-force, exploitation, etc.).
- The targeted usernames and passwords.

I analyzed this data to understand attacker behaviors and tactics, which can help refine the honeypot configuration for more accurate threat detection and better simulation of a real-world attack surface.

**Screenshot 6: T-Pot Home Menu with Attack Map, Elasticvue, and Other Dashboards**  
**Ref 6:** Screenshot showcasing the T-Pot home menu with the Attack Map, Elasticvue, and other integrated dashboards, that allow for a holistic view of real-time attack data and system performance.
![image](https://github.com/user-attachments/assets/00094c93-52f7-4562-91d1-4c6135cb8b92)


