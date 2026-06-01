Automated Nmap Recon Tool

A simple Bash-based automation tool for performing reconnaissance using Nmap in Kali Linux.

This script automates:

full TCP port scanning
service/version detection
NSE script scanning
structured text report generation

The goal of this project is to simplify repetitive reconnaissance tasks during labs, CTFs, and authorized security testing.

Features
Full 65535 TCP port scan
Automatic extraction of open ports
Service and version detection
NSE script scanning
Single structured report output
Simple Bash implementation
Lightweight and beginner-friendly
Requirements

Install required packages:

sudo apt install nmap -y
Usage

Clone the repository:

git clone https://github.com/Mahidinesh0/recon

cd repo-name

Give execution permission:

chmod +x recon.sh

Run the script:

./recon.sh <target-ip>

Example:

./recon.sh 192.168.1.40

Example Workflow

The script performs the following steps:

1. Full TCP Port Scan
2. Extract Open Ports
3. Service Detection
4. NSE Script Scan
5. Report Generation
Example Output
[+] Starting scan on 192.168.1.40
[+] Running full port scan...
[+] Running service scan...
[+] Running NSE script scan...
[+] Report saved as report.txt
Report Structure

The generated report.txt contains:

target information
open ports
service detection results
NSE script results
executed Nmap commands

Example:


Nmap Recon Report:

Target: 192.168.1.40

Open Ports:
22,80,443
Challenges Faced

During development, several issues were encountered:

broken Bash scripts caused by Markdown copy/paste
Windows line ending problems (CRLF)
extracting ports reliably from Nmap output
handling unexpected scan results

This project also helped improve understanding of:

Bash scripting
process automation
Nmap workflows
output parsing
Disclaimer

This tool is intended only for:

educational purposes
labs
CTF environments
authorized security testing

Do not scan systems without proper permission.

Future Improvements

Possible future upgrades:

HTML report generation
UDP scanning support
service-specific NSE automation
CVE enrichment
JSON/XML export
multi-target scanning
