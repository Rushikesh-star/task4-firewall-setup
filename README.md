Task 4 - Firewall Setup and Testing (UFW on Kali Linux)

Objective
Configured and tested basic firewall rules using UFW (Uncomplicated Firewall) on Kali Linux to allow and block specific traffic.

Steps Performed

1. Installed UFW

    sudo apt install ufw

   UFW installed successfully for managing firewall rules easily.

3. Checked Firewall Status

    sudo ufw status numbered

   Initially firewall was inactive.

5. Enabled Firewall

   sudo ufw enable

   Firewall activated and set to start automatically on system boot.

7. Blocked a Specific Port (Example: Telnet - Port 23)

   sudo ufw deny 23

   This rule blocks all inbound connections on port 23.

9. Tested Block Rule

   Tried to connect to the blocked port locally/remotely. Connection failed as expected.

11. Allowed SSH (Port 22)

    sudo ufw allow 22

    This rule allows secure remote login to the system.

13. Removed Test Rule

    sudo ufw delete deny 23

    Restored firewall to its original state after testing.

Screenshots

Included screenshots showing:

Installation of UFW

Firewall status before and after enabling

Rules added and deleted

Summary

Using UFW, I was able to easily control network traffic by adding rules to block or allow specific ports. This helps improve system security by preventing unauthorized access.

Tools Used

Kali Linux
UFW (Uncomplicated Firewall)

