# Troubleshooting-Experience-Linux
<h3> My experience troublshooting issues within linux distros </h3>

<h2>SSH</h2>

Issue
- <b2> Unable to SSH into Linux server</b2>

Environment:
- <b2> Ubuntu 24.04 LTS server <b2>

Troubleshooting Steps:
1. Attempt to SSH into the server
2. Ping the server's IP address
     - <b2> I am able to reach the outside internet from my server via inputting the "sudo apt update" command and it returning available software packages for download</b2>
3. I check the status of my SSH server with cmd "systemctl status ssh" since my server isn't suffering from an internet connectivity issue
4. I enable the use of SSH with "systemctl enable ssh"  
5. I start the SSH server with cmd "systemctl start ssh" to verify that it is running
6. Double check SSH functionality by using cmd "systemctl status ssh" and attempting SSH login

Root Cause:

- <b2> Disabled SSH server  <b2>

Resolution:

- <b2> Enable, start, and check functionality of SSH <b2> 

Prevention:

- <b2> Document instruction in ticketing system for SSH issues as follows:<b2>
  - <b2> Ensure Internet connectivity is enabled within linux machine then move onto diagnosing SSH <b2>
    - <b2> If SSH still doesn't work despite internet connectivity, verify it's status with this command: "systemctl status ssh" <b2>
    - <b2> If SSH server is disabled, enable it with this command: "systemctl enable ssh" <b2>
    - <b2> If SSH server is enabled, start it with this command: "systemctl start ssh" <b2>
        - <b2> Attempt SSH login <b2>
    
    


 <p align="center">
    <img src="https://github.com/zay65/Troubleshooting-Experience-Linux/blob/59528e4b229b925fc8cc79daf72f363746033097/Troubleshooting%20SSH.png" alt="Sample Image"/>
  </p>


 
