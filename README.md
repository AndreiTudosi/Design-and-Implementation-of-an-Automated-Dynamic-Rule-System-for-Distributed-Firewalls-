# Design-and-Implementation-of-an-Automated-Dynamic-Rule-System-for-Distributed-Firewalls-


Firewall Log Analyzer
This script allows you to analyze firewall logs and automatically block IP addresses that trigger specific events. It interacts with the pfSense firewall API to create firewall rules based on the logged events.

Requirements

Python 3.x
Required packages: re, requests, time, urllib3
pfSense firewall with API enabled

Installation

Clone the repository:
git clone https://github.com/your-username/your-repository.git

Install the required packages:
pip install requests

Configuration
Before running the script, make sure to configure the following variables in the code:

api_url: The URL of the pfSense firewall API.
api_log_url: The URL to fetch the firewall logs.
api_username: Your pfSense API username.
api_password: Your pfSense API password.
interval: The time interval (in seconds) between log checks.

Usage
Run the script:
python firewall_log_analyzer.py
The script will continuously monitor the firewall logs and check for specific events.
If an event is detected, the script will block the corresponding IP address by creating a firewall rule.
The blocked IP address will be recorded along with a timestamp and automatically unblocked after 24 hours.


Contributing
Contributions are welcome! If you find any issues or have suggestions for improvement, please feel free to open an issue or submit a pull request.

License
This project is licensed under the MIT License.


![image](https://github.com/AndreiTudosi/Design-and-Implementation-of-an-Automated-Dynamic-Rule-System-for-Distributed-Firewalls-/assets/136599367/8845b15c-85eb-433f-8310-03b7e7071f34)

Results of GET command for firewall rules

![image](https://github.com/AndreiTudosi/Design-and-Implementation-of-an-Automated-Dynamic-Rule-System-for-Distributed-Firewalls-/assets/136599367/cb3f65e2-e461-43b1-b869-406d79fc626c)

Results after running the GET command for Snort logs

![image](https://github.com/AndreiTudosi/Design-and-Implementation-of-an-Automated-Dynamic-Rule-System-for-Distributed-Firewalls-/assets/136599367/5a08d9c3-c808-4dae-a55e-339f8c69e839)

Results after running the POST firewall rule

![image](https://github.com/AndreiTudosi/Design-and-Implementation-of-an-Automated-Dynamic-Rule-System-for-Distributed-Firewalls-/assets/136599367/2bf32197-4e69-4e2c-ace9-85db664014f7)

Successfully firewall rule creation

![image](https://github.com/AndreiTudosi/Design-and-Implementation-of-an-Automated-Dynamic-Rule-System-for-Distributed-Firewalls-/assets/136599367/c25cef5e-c3d0-4499-9d24-fc3134b66158)

LOIC interface
