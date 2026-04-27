# Troubleshooting-Experience-Linux
<h3>My experience troublshooting issues within linux distros</h3>

- <b2> 1) I fail at my attempt to SSH into my linux server as shown by the "Connection timed out message"</b2>
- <b2> 2) I fail at my attempt to ping the server's IP address, which may mean my server's cutoff from the internet or may be unreachable.</b2>
    - <b2> I am able to reach the outside internet from my server via inputting the "sudo apt update" command and it returning available software packages for download.</b2>
- <b2> 3) Since I can access the internet, albeit one-way, it may possibly be an SSH issue so I check the status of my SSH server with cmd "systemctl status ssh" and it returns a "disabled" status</b2>
- <b2> 4) Since I can access the internet, albeit one-way, it may possibly be an SSH issue so I check the status of my SSH server with cmd "systemctl status ssh" and it returns a "disabled" status</b2>
- <b2> 5) I use "sudo" for admin privileges and enable the use of SSH with "systemctl enable ssh"</b2>
- <b2> 6) Just because it's installed doesn't mean its turned on, so I start the SSH server with cmd "systemctl start ssh"</b2>
- <b2> 7) And just because I think it may be on doesn't mean it is, so I verify full SSH functionality by again using cmd "systemctl status ssh" and attempting to SSH into my server and Voila!</b2>



 <p align="center">
    <img src="https://github.com/zay65/Troubleshooting-Experience-Linux/blob/59528e4b229b925fc8cc79daf72f363746033097/Troubleshooting%20SSH.png" alt="Sample Image"/>
  </p>


 
