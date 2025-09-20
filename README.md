# System Health Check

**Author:** Ivaylo Atanassov  

## Description
Python script that generates a comprehensive system health report for your computer. It collects CPU, memory, disk usage, system uptime, network connectivity, response time, and Windows service status (if applicable). The output is displayed in the terminal with color-coded warnings and saved to a timestamped log file.

---

## Features

-  System information (OS, architecture, hostname)  
-  CPU usage and hardware details  
-  Memory usage with high usage warnings  
-  Disk usage with low-space warnings  
-  Network connectivity tests to Google and Cloudflare  
-  Response time measurement to google.com  
-  Windows service status checks (Windows only)  
-  Color-coded terminal output with clean log file output  
-  Error handling for inaccessible disks, network failures, and missing services  

---

## Installation

 1. Ensure Python 3 is installed:  
python --version
2. Install required packages:  
   pip install psutil
## Usage
1. Clone the repository:  
    - git clone https://github.com/your-username/system-health-check.git
2. Navigate to the project folder:  
   - cd system-health-check
3. Run the script:  
   - python system_health_check.py

Logs are automatically saved in the Logs folder with a timestamped filename.

## Sample Output
Computer Name: DESKTOP-01  
Operating System: Windows 11  
CPU Usage: 23%  
Memory Usage: 8.1GB used / 16GB total  
C:\ Usage: 120GB used / 250GB total  
Google DNS: Connected  
Windows Update: STOPPED  
Windows Defender Firewall: Running  
...

## Notes
- Windows service checks run only on Windows systems.
- Network tests may fail if firewalls block certain ports.
- The script was developed with AI assistance but reviewed, refined, and integrated by the author. All logic and formatting were manually verified.

## License
This project is licensed under the MIT License.
