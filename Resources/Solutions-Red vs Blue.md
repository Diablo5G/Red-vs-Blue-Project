<img align="left" width="420" height="210" src="https://github.com/Diablo5G/Red-vs-Blue-Project/blob/Master/Resources/Red-teaming-blue-teaming-1.jpg">

# Unit Red vs. Blue Team Project 

Red Team vs. Blue Team scenario,
As the Red Team, we will attack a vulnerable VM within your environment, ultimately gaining root access to the machine. 
As Blue Team, we will use Kibana to review logs taken during their Day 1 engagement. We'll use the logs to extract hard data and visualizations for report.


### Lab Environment

The Hyper-V Manager to access the nested machines:

- **ELK machine credentials:** The same ELK setup that we created in Project [ELK-Stack-Project](https://github.com/Diablo5G/ELK-Stack-Project).
    - Username: `vagrant`
    - Password: `vagrant`
    - IP Address: `192.168.1.100`

- **Kali:** A standard Kali Linux machine
    - Username: `root`
    - Password: `toor`
    - IP Address: `192.168.1.90`

- **Capstone:** Filebeat and Metricbeat are installed and will forward logs to the ELK machine. 
   - IP Address: `192.168.1.105`


<img align="left" width="80" height="70" src="https://github.com/Diablo5G/Red-vs-Blue-Project/blob/Master/Resources/redblue.jpeg">

#### Submission File

[Project 2 Report](https://github.com/Diablo5G/Red-vs-Blue-Project/blob/Master/Resources/Project%202%20-%20Red%20Team%20Assessment%2C%20Analysis%20n'%20Hardening%20of%20a%20Vulnerable%20System.pdf)

#### Interview Questions Domain : Network Security

##### Faulty Firewall
"Suppose you have a firewall that's supposed to block SSH connections, but instead lets them through. How would you debug it?"

We can debug after performing a generic sweep of the network, which we can dig deeper into specific hosts we find. (The tools for performing generic TCP port scans such as SuperScan, Nessus, or NetScanTools Pro.) Configuring firewalls to look for potentially malicious behavior over time such as the number of packets received in a certain period of time, and have rules in place to cut off attacks if a certain threshold is reached, such as 10 port scans in one minute or 100 consecutive ping (ICMP) requests. Most firewalls and IDSes/IPSes can detect such scanning and cut it off in real-time.


##### Unsecured Web Server
"Suppose you find a server running HTTP on port 80, despite compliance guidelines requiring encryption in motion. What do you do?"



---



