CODTECH_ADVANCE_TASK_1
File Integrity Checker
Personal Details
Name : Solanki Shankar : CODTECH IT Solutions ID : CT08FYC Domain : CYBER ECURITY AND ETHICAL HACKING Duration : 20/12/2024 to 20/1/2025 Mentor : Neela Santhosh Kumar

Overview
The File Integrity Checker is a Python tool designed to monitor and verify the integrity of files using hash functions. It allows users to detect file modifications, maintain a history of changes, and ensure data consistency.

Features
Multiple Hash Algorithms: Supports MD5, SHA1, and SHA256.
Modification Detection: Compares stored and current file hashes to identify changes.
History Tracking: Maintains a detailed history of file modifications, including timestamps and previous hash values.
Interactive CLI: User-friendly command-line interface with ASCII art logo.
JSON Storage: Saves file hashes and history in a JSON file for persistent monitoring.
Installation
Clone the repository:

git clone https://github.com/hipremsoni/CODETECH_ADVANCE_TASK_1.git
cd CODETECH_ADVANCE_TASK_1
Install dependencies:

pip install -r requirements.txt
Run the tool :

Python3 file_integrity_checker.py
Usage
Run the program:

python3 file_integrity_checker.py
Enter file paths: Provide one or multiple file paths to monitor, separated by commas.

// Example For Windows Path 
C:\\Example\\file.txt
//Exaple For Linux Path 
/home/kali/file.txt

Select a hash algorithm: Choose one of the supported algorithms (MD5, SHA1, SHA256).

Monitor for changes: The tool checks file integrity, stores hashes, and updates the history in hashes.json.

View history: Optionally, display the modification history for any file.

Screenshot
image

Example
Detecting Changes:
![image](https://github.com/user-attachments/assets/00b284ef-1ced-4581-ad61-850fe59a12e1)




u:\CODTECH INTERNSHIP\CODTECH ADV TASK\TASK 1\example_file.txt
Select a hash algorithm:
1. md5
2. sha1
3. sha256
Enter the number corresponding to your choice: 1
Selected algorithm: md5
Hash for u:\CODTECH INTERNSHIP\CODTECH ADV TASK\TASK 1\example_file.txt (md5): 62298bbc1b0affa31e5f31f1d8fed82f
Stored hash: b415b32cbf036c7af9bfba6f7fbaa8ef (Last checked: 2025-01-16 15:09:44)
WARNING: u:\CODTECH INTERNSHIP\CODTECH ADV TASK\TASK 1\example_file.txt has been modified using md5! (Stored: b415b32cbf036c7af9bfba6f7fbaa8ef, Current: 62298bbc1b0affa31e5f31f1d8fed82f)
Do you want to view the modification history of any file? (yes/no): yes
Enter the file path for which you want to view history: u:\CODTECH INTERNSHIP\CODTECH ADV TASK\TASK 1\example_file.txt        
Modification history for u:\CODTECH INTERNSHIP\CODTECH ADV TASK\TASK 1\example_file.txt (md5):
Previous Hash: b415b32cbf036c7af9bfba6f7fbaa8ef | Timestamp: 2025-01-16 15:10:18
File Structure
file_integrity_checker.py: Main Python script.
hashes.json: JSON file storing hashes and modification history.
requirements.txt: Dependencies for the project.
Dependencies
hashlib
os
json
pyfiglet
colorama
datetime
Acknowledgements
pyfiglet for ASCII art generation.
colorama for terminal text formatting.
