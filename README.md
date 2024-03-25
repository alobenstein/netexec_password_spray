This script tests username and password combinations against a variety of protocols, including SMB, SSH, RDP, and WinRM, to verify if users have logins on a different IP address, or if passwords have been reused. This allows for individuals to assess their or their client's cybersecurity posture, in a streamlined and automated fashion. The data findings will be printed to the terminal and exported to a CSV file, which can be transferred to Windows and viewed using Excel. The default behavior of the script (when no flags are used) is to go line by line and print and export only successful authentication attempts.

This script is intended solely for authorized penetration testing engagements within environments where you (the user) has explicit permission to conduct tests. Before executing this script, confirm that you possess the necessary authorization. The creator of this script accepts no responsibility for misuse of this script and strongly advises against any unauthorized use. Do not use this script without sufficient prior authorization, understanding, and forethought. Password spraying attacks can result in account lockouts and other security consequences, which can compromise cyber security and cause damages to business operations.

Prerequisites: NetExec must be installed on your Debian/Kali machine. You must create a file with the list of IPs, usernames, and passwords that will be tested. The username and password combinations should be on the same line in users.txt and in passwords.txt, unless -a flag is used to test every username with every password.

Usage: ./netexec_credential_spray.sh [-a] [-v] [-s] -a: Test every username with every password. -v: Verbose mode. Print debug statements. -s: Suppress success messages.
