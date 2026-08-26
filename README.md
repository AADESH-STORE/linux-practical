# 🐧 Linux Practical Examination Portfolio

* **Linux OS Version:** Ubuntu 22.04 LTS *(Update this with your system's version if different)*
* **Student Name:** [AADESH CHAUDHARI]
* **Roll Number:** [0004]

---

## 📂 Section A — File & Directory Management

### Q1. Basic File Operations
* **Commands used:** `mkdir LinuxExam`, `cd LinuxExam`, `touch student.txt course.txt result.txt`, `pwd`, `ls`
* **Conclusion:** Successfully initialized the sandbox examination workspace and baseline template target files.
![Q1 Output](screenshots/Q1%20ANS.png)

### Q2. File Management
* **Commands used:** `cp student.txt student_backup.txt`, `mv course.txt linux_course.txt`, `rm result.txt`, `mkdir Documents Backups Scripts`, `mv student_backup.txt Backups/`, `ls -R`
* **Conclusion:** Reorganized file layout architecture and moved system backup snapshots cleanly into specified target locations.
![Q2 Output](screenshots/Q2%20ANS.png)

### Q3. File Content Operations
* **Commands used:** `cat student.txt`, `cat linux_course.txt`, `head -n 3 student.txt`, `tail -n 2 student.txt`, `wc student.txt`
* **Conclusion:** Populated structured records, verified input via core filters, and printed precise tracking metadata metrics.
![Q3 Part 1](screenshots/Q3%20ANS%201%29.png)
![Q3 Part 2](screenshots/Q3%20ANS%202%29.png)

---

## 👥 Section B — Users, Groups & Permissions

### Q4. User Management
* **Commands used:** `sudo useradd student01`, `sudo passwd student01`, `id student01`, `grep student01 /etc/passwd`, `su - student01`, `whoami`
* **Conclusion:** Configured an isolated testing user container environment with proper default home access parameters.
![Q4 Output](screenshots/Q4%20ANS.png)

### Q5. Group Management
* **Commands used:** `sudo groupadd linuxbatch`, `sudo usermod -aG linuxbatch student01`, `groups student01`, `sudo useradd student02`, `sudo usermod -aG linuxbatch student02`, `grep linuxbatch /etc/group`
* **Conclusion:** Established unified group profiles to manage multiple local user permission layers simultaneously.
![Q5 Output](screenshots/Q5%20ANS.png)

### Q6. File Permissions
* **Commands used:** `touch project.txt`, `chmod 754 project.txt`, `ls -l project.txt`, `chmod 640 project.txt`, `sudo chown student01:linuxbatch project.txt`
* **Conclusion:** Applied precise octal bitmask permissions and correctly transferred user/group administrative weights.
![Q6 Output](screenshots/Q6%20ANS.png)

### Q7. Permission Challenge
* **Commands used:** `mkdir public private shared`, `chmod 777 public`, `chmod 700 private`, `chmod 770 shared`, `ls -ld public private shared`
* **Conclusion:** Verified complete isolation profiles ensuring public, locked, and team-shared compartmentalization states.
![Q7 Output](screenshots/Q7%20ANS.png)

---

## 🌐 Section C — Package Management & Services

### Q8. Package Management
* **Commands used:** `sudo apt update`, `sudo apt install apache2 -y`, `apache2 -v`, `sudo systemctl start apache2`, `sudo systemctl status apache2`, `sudo systemctl enable apache2`
* **Conclusion:** Updated repositories, deployed the HTTP web daemon service layer, and registered it into system boot hooks.
![Q8 Output](screenshots/Q8%20ANS.png)

### Q9. Apache Web Server Configuration
* **Commands used:** `cd /var/www/html`, `sudo nano index.html`, `sudo systemctl restart apache2`, `curl http://localhost`
* **Conclusion:** Built a customized homepage compiling individual verification markers and validated local rendering states.
![Q9 Output](screenshots/Q9%20ANS.png)

---

## 💻 Section D — Processes & System Administration

### Q10. Process Management
* **Commands used:** `ps aux`, `top`, `pidof apache2`, `ps -p <PID>`, `sudo systemctl stop apache2`
* **Conclusion:** Tracked background runtime execution queues and verified diagnostic service initialization/termination cycles.
![Q10 Output](screenshots/Q10%20ANS.png)

---

## 🔍 Section E — Searching, Filtering & Logs

### Q11. Search and Text Processing
* **Commands used:** `grep -i "pattern" students.txt`, `wc -l`, `sort students.txt`, `find . -name "*.txt"`
* **Conclusion:** Utilized robust regular expressions and pattern search tools to safely extract index logs from datasets.
![Q11 Part 1](screenshots/Q11%20ANS%201%29.png)
![Q11 Part 2](screenshots/Q11%20ANS%202%29.png)

---

## 🛜 Section F — Networking

### Q12. Linux Networking & Challenge
* **Commands used:** `hostname`, `hostname -I`, `ifconfig`, `route -n`, `ping -c 4 google.com`, `curl -I google.com`
* **Conclusion:** Checked socket device cards, traced the routing path gateway, and resolved the local HTTP socket problem.
![Q12 Part 1](screenshots/Q12%20ANS%201%29.png)
![Q12 Part 2](screenshots/Q12%20ANS%202%29.png)
![Q12 Part 3](screenshots/Q12%20ANS%203%29.png)
