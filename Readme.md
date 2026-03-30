Open Source Software Audit: MySQL 8.0

OSS Capstone Project - VITyarthi

This repository contains the practical component of the Open Source Software (OSS) audit project. It includes five automated Bash scripts designed to audit a Linux system and evaluate the footprint of the MySQL 8.0 database engine.

👤 Student Information

Name: Vaidehi Gupta

Registration Number: 24BCE10616

Slot: F11

University: VIT Bhopal University

🛠️ Chosen Software

Software: MySQL 8.0 (Community Server)

License: GPL v2 / Commercial Dual-License

Environment: Ubuntu 24.04 LTS (WSL 2)

📜 Script Descriptions

1. Script 1: System Identity Report (script1.sh)

Purpose: Establishes the identity of the auditor and the host environment. It extracts core system metadata to ensure the audit environment is valid and correctly licensed.

Concepts: Variables, Command Substitution ($()), formatting.

2. Script 2: FOSS Package Inspector (script2.sh)

Purpose: Checks if MySQL is installed on the local Linux path. It retrieves the version, license summary, and binary location of the software.

Concepts: if-then-else logic, command -v, string manipulation.

3. Script 3: Disk and Permission Auditor (script3.sh)

Purpose: Loops through critical system directories (/etc/mysql, /var/lib/mysql) to audit disk usage and file-level permissions, ensuring the software follows the Linux Filesystem Hierarchy Standard.

Concepts: for loops, du, ls -ld, awk.

4. Script 4: Log File Analyzer (script4.sh)

Purpose: Analyzes MySQL error logs to identify operational issues. It counts the occurrences of a specific keyword (e.g., "ERROR" or "WARNING") within the log file.

Concepts: while-read loops, counter variables, grep filters.

5. Script 5: Open Source Manifesto Generator (script5.sh)

Purpose: An interactive tool that collects user input to generate a personalized open-source philosophy statement, which is then saved to a permanent text file.

Concepts: read for user input, file redirection (>), string concatenation.

🚀 How to Run the Scripts

Follow these steps to execute the audit scripts on your Linux/Ubuntu system:

1. Clone the Repository

git clone
cd oss-audit-24BCE10616


2. Set Executable Permissions

Before running, you must grant execution rights to the shell files:

chmod +x *.sh


3. Run the Scripts

You can run each script individually using the ./ notation:

./script1.sh
./script2.sh
./script3.sh
./script4.sh
./script5.sh


📦 Dependencies

To ensure all scripts function correctly, the following packages should be installed on your Ubuntu system:

Bash Shell: Standard on most Linux distros.

MySQL Server: sudo apt install mysql-server

CoreUtils: (Includes ls, du, df, awk)

⚖️ License

The scripts in this repository are provided under the MIT License. The audited software (MySQL) is governed by the GPL v2 license.
