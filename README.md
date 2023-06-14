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
