# Linux Practical Examination

## Student Details
- Name: AADESH CHAUDHARI 
- Roll Number: 004
- Course Name: AWS & DevOps 

## Linux Version
- Operating System: Ubuntu
- Kernel Version: `uname -r`
- Distribution Details: `cat /etc/os-release`

## Practical Work Summary

### 1. Apache Web Server Configuration
- Found the Apache document root.
- Created a custom `index.html` file.
- Added the required student details and the text `Linux Practical Examination`.
- Restarted Apache.
- Accessed the webpage using browser and `curl`.

Commands used:
```bash
grep -i DocumentRoot /etc/apache2/sites-available/000-default.conf
sudo nano /var/www/html/index.html
sudo systemctl restart apache2
curl -i http://localhost/

2. Process Management
•	Displayed all running processes.
•	Viewed processes in real time using `top`.
•	Found the PID of Apache.
•	Displayed Apache process details using its PID.
•	Stopped Apache and verified that it stopped.
•	Started Apache again and verified its status.
Commands used:

ps -e
top
pidof apache2
ps -p <PID> -f
sudo systemctl stop apache2
sudo systemctl status apache2
sudo systemctl start apache2
sudo systemctl status apache2


3. Search and Text Processing
•	Created `students.txt` with at least 10 student records.
•	Used `grep` to search for matching names or patterns.
•	Used case-insensitive search with `grep -i`.
•	Counted matching records.
•	Sorted student records.
•	Used `find` to locate `.txt` files inside the `LinuxExam` directory.
Commands used:

cd LinuxExam
nano students.txt
grep 'a' students.txt
grep -i 'a' students.txt
grep -c 'a' students.txt
sort students.txt
find . -type f -name "*.txt"


4. Networking
•	Displayed the system hostname.
•	Displayed the IP address.
•	Displayed network interfaces.
•	Displayed the routing table.
•	Tested connectivity using `ping`.
•	Accessed a webpage using `curl`.
•	Found the IP address of a domain name.
•	Displayed listening ports.
Commands used:

hostname
ip addr
ip link
ip route
ping google.com
curl https://example.com
nslookup google.com
ss -tuln


Screenshots
•	All screenshots included in this repository are from my own execution.
•	Each screenshot shows the command entered and the output generated on my system.
Result / Conclusion
All required Linux practical tasks were completed successfully. The Apache server was configured, processes were managed, text searching and filtering were performed, networking commands were tested, and results were verified using terminal output and screenshots.
Repository Information
•	GitHub Repository: 
•	Submitted To: Examiner
