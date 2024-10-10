# Elastic-Stack-SIEM-Configuration-and-Management

## Objective

The SIEM lab aimed to configure and deploy Elastic Stack to collect and analyze log data for effective security event monitoring. The primary focus was on setting up Elastic Agents to gather logs from various sources and forward them to the SIEM. This hands-on experience provided a deeper understanding of log management, threat detection, and incident response within a Security Information and Event Management (SIEM) system.

### Skills Learned

- Advanced understanding of Elastic Stack and its components for Security Information and Event Management (SIEM).
- Ability to analyze and interpret security event logs to detect potential threats and anomalies.
- Proficiency in configuring Elastic Agents for log collection and forwarding data to a centralized SIEM platform.
- Development of critical thinking and problem-solving skills in monitoring, investigating, and responding to security incidents.
- Enhanced knowledge of log management, event correlation, and threat detection methodologies.

### Tools Used

- Elastic Stack for centralized log collection, analysis, and SIEM capabilities.
- Elastic Defend for endpoint protection and threat detection.
- Kali Linux VM for testing and simulating security events.
- Custom Elastic Stack rule configurations for detecting and responding to specific security threats and anomalies.

## Steps

- I initiated the process by creating an Elastic account and identifying the Elastic Defend integration within the Elastic Stack platform.
![1](https://github.com/user-attachments/assets/2627004d-b21b-4b9c-b6ac-44c5e841f526)

- At this stage, I configured the integration settings to ensure proper functionality and alignment with the required security monitoring objectives.
![2](https://github.com/user-attachments/assets/dd733752-611e-4cb3-bada-44a4ad42c293)

- Next, I installed and configured the Elastic Agent on my Kali Linux machine to enable log collection and forwarding to the Elastic Stack.
![3](https://github.com/user-attachments/assets/a7433f27-1510-440d-85c1-15a4a591629d)

- The Elastic Agent was successfully installed, establishing seamless log collection and integration with the Elastic Stack platform.
![4](https://github.com/user-attachments/assets/ff1b68b7-3663-4bcf-ae08-687fd2d9c3c2)

- I executed the command sudo systemctl status elastic-agent.service to verify the status of the Elastic Agent and confirm it was running correctly.
![5](https://github.com/user-attachments/assets/13e0e534-967a-4fee-8903-e1b5f832f277)

- I subsequently performed an Nmap SYN scan (nmap -sS) on my localhost to generate network activity for monitoring and analysis.
![6](https://github.com/user-attachments/assets/ee90ee05-bfb6-445c-bfe1-b60de769cba4)

- Next, I navigated to the logs in Elastic Defend to review and analyze the collected data from the scan and other system activity.
![7](https://github.com/user-attachments/assets/4d406df2-a9cc-4c9d-b0a0-2b2a4d079182)

- I then accessed the stream feature and conducted a search for process.args: nmap to filter and review the relevant log entries associated with the Nmap scan.
![8](https://github.com/user-attachments/assets/0e959509-bcd4-466d-93b8-8b0c9eec99a4)

- I then examined the details of one of the entries, which confirmed the detection of the Nmap scan executed earlier on my Kali machine.
![9](https://github.com/user-attachments/assets/cd7547b0-efb7-4f25-b718-09cc3d9cdc90)

- I then navigated to the dashboard and created a visualization, selecting "Count" for the vertical axis and "Timestamp" for the horizontal axis to represent the data over time.
![10](https://github.com/user-attachments/assets/c6761b47-a570-43ff-b1b8-6070b0e2beba)

- I then accessed the Security section, navigated to Alerts, and selected Managed Rules to review and configure the security alerting rules.
![11](https://github.com/user-attachments/assets/a3fdf600-b1fa-4e59-b8c3-de536ab90963)

- I then defined the query specifically for detecting Nmap scans to enhance the security monitoring capabilities within the system.
![12](https://github.com/user-attachments/assets/17569f4f-b44e-4d27-bcc8-545a5b59ff7e)

- I then selected the email action to ensure I receive notifications via email whenever an alert is triggered.
![13](https://github.com/user-attachments/assets/34020fe2-631a-4878-a4ea-64be0d7e8926)

- I then returned to my Kali machine and executed another Nmap scan to test the alerting action.
![14](https://github.com/user-attachments/assets/bf083e17-5b9d-4249-86aa-48e8db9a4cc0)

- Finally, I accessed the dashboard to review the activity and assess the results of the executed Nmap scan.
![15](https://github.com/user-attachments/assets/eafb9915-b988-4ac4-824c-31c900753964)

*Ref 1: Network Diagram*

