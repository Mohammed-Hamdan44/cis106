---
Name: Mohammed Hamdan
Class: CIS106 Fall 23
---

# Deliverable 2

## 1. What are the server hardware specifications (virtual machine settings)? 
![Q!](../deliverable2/Ubuntu%20Server%20VM%20Settings.png)

## 2. What is Ubuntu server log in screen? 
![Q2](../deliverable2/Ubuntu%20Server%20Log%20In%20Screen.png)

## 3. What is the IP address of your Ubuntu Server Virtual Machine?
127.0.0.1

## 4. How do you enable the Ubuntu Firewall?
sudo ufw enable

## 5. How do you check if the Ubuntu Firewall is running?
sudo ufw status

## 6. How do you disable the Ubuntu Firewall?
sudo ufw disable

## 7. How do you add Apache to the Firewall?
sudo ufw allow 'Apache'

## 8. What is the command you used to install Apache?
apt-get install apache2

## 9. What is the command you use to check if Apache is running?
sudo systemctl status apache2

## 10. What is the command you use to stop Apache?
sudo systemctl stop apache2

## 11. What is the command you use to restart Apache?
sudo systemctl restart apache2

## 12. What is the command used to test Apache configuration?
sudo apache2ctl configtest

## 13. What is the command used to check the installed version of Apache? 
apache2 -v

## 14. What are the most common commands to troubleshoot Apache errors? Provide a brief description of each command.
* sudo systemctl status apache2: This command provides the current status of the Apache service, including whether it is active, inactive, or encountering errors.
* sudo apachectl configtest: Verifies the syntax of your Apache configuration files without restarting the server. It helps identify syntax errors in your configuration.
* sudo tail -f /var/log/apache2/error.log: Displays the last few lines of the Apache error for monitoring errors as they occur.
* sudo tail -f /var/log/apache2/access.log: Checks Apache Access Log

## 15. Which are Apache Log Files, and what are they used for? Provide examples and screenshots.
* Error Log: The error log contains information about errors and issues encountered by Apache during its operation. This log is crucial for diagnosing and troubleshooting problems with the server. Example: sudo tail -n 20 /var/log/apache2/error.log
* Access Log: The access log records every request made to the Apache server, including information about the source IP address, requested URL, response status, and more. It is useful for analyzing traffic patterns and identifying potential security issues. Example: sudo tail -n 20 /var/log/apache2/access.log